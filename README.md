Build a Babel Fish with Machine Learning Language Services
=========================================

This repository contains necessary resources for AWS re:Invent 2018 workshop AIM313. In this readme you will find detailed instructions for each phase of the workshop.

<img src="img/flow1.png" />


Setup
-----

To build your own Babel Fish you will need to accomplish four phases. Each of them will add new functionality to your Babel Fish and will use different AI service from AWS portfolio.

<a href="https://www.onet.com"><img src="/img/button1.png" width="200"></a>
[![Get Started](img/button1.png&s=200)](./instructions/1-voice-user-interface.md)

Skills can be built either by implementing ``AbstractRequestHandler`` classes
or by using skill builder's ``request_handler`` decorator. More information
on this can be checked in the [documentation](https://alexa-skills-kit-python-sdk.readthedocs.io/en/latest/REQUEST_PROCESSING.html#request-handlers).

This sample skill shows how to implement ``AbstractRequestHandler`` class
and register the handler classes explicitly in the skill builder object.
The code for this implementation is under [lambda/py](lambda/py) folder.

For the sample skill using the ``decorators`` approach, check
[skill-sample-python-helloworld-decorators](https://github.com/alexa/skill-sample-python-helloworld-decorators).

Additional Resources
--------------------

### Community

-  [Amazon Developer Forums](https://forums.developer.amazon.com/spaces/165/index.html) : Join the conversation!
-  [Hackster.io](https://www.hackster.io/amazon-alexa) - See what others are building with Alexa.

### Tutorials & Guides

-  [Voice Design Guide](https://developer.amazon.com/designing-for-voice/) -
   A great resource for learning conversational and voice user interface design.

### Documentation

-  [Official Alexa Skills Kit Python SDK](https://pypi.org/project/ask-sdk/)
-  [Official Alexa Skills Kit Python SDK Docs](https://alexa-skills-kit-python-sdk.readthedocs.io/en/latest/)
-  [Official Alexa Skills Kit Docs](https://developer.amazon.com/docs/ask-overviews/build-skills-with-the-alexa-skills-kit.html)
