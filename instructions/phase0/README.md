Build a Babel Fish with Machine Learning Language Services
=========================================

This repository contains necessary resources for AWS re:Invent 2018 workshop AIM313. In this readme you will find detailed instructions for Phase 0.

<img src="../../img/flow0.png" />


Phase 0: Environment setup
-----

Clone this repository to your local machine or download `zip` file with its content.

Sign into the AWS Console and choose `eu-west-1` (Irleand) region. Click the link below to launch CloudFormation stack in your AWS account. It will configure your environment with resources necessary to run this workshop.

<a href="https://console.aws.amazon.com/cloudformation/home?region=eu-west-1#/stacks/new?stackName=babel-fish-app&templateURL=https://s3-eu-west-1.amazonaws.com/babel-fish-reinvent/cfn-babel-fish.yaml"   target="_blank" rel="noopener noreferrer"  ><img src="../../img/button-launch-stack.png" width="140"></a>

Move through the wizard (`Next`, `Next`, `Next`), on `Review` page acknowledge that CloudFormation might create IAM resources and click `Create`. Wait a few moments until status changes from `CREATE_IN_PROGRESS` to `CREATE_COMPLETE`.

On `Stacks` page click stack name to view `Stack Detail` page and expand `Resources` section. In `Logical ID` column find the following two items and copy their `Physical ID` values for later use:

* `CognitoIdentityPool` - `Physical ID` is the created Identity Pool ID.
* `DataBucket` - `Physical ID` is the created S3 bucket name.

Use S3 service in the AWS Console to open the created bucket and create `input` and `output` folders in it.

Update your local JavaScript app `babel-fish.js` and replace placeholders with correct configuration data:

1. Provide your S3 bucket name in line 3.
1. Provide your Identity Pool ID in line 4.

Please note that created Lambda functions use `Python 3.6` by default and while it's absolutely not a problem to use other programming languages to develop this solution only `Python` is actively supported during this workshop.

**Once you're finished with this phase please wait for speakers to present the next one before moving forward.**

<a href="../../README.md"><img src="../../img/button2.png" width="200"></a>
<a href="../phase1/README.md"><img src="../../img/button3.png" width="200"></a>
