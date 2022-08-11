# How to contribute to Azure-Servicebus-PHP?

Hello there, thank you for reviewing our contribution notes. In this contributors information document you will learn why this project got started, how the library is being developed and what is being expected from you when you would like to participate in the development.

## Why was this project created?

During an application modernization and cloud migration project of a PHP application, we couldn't replace the existing [RabbitMQ] message broker with [Azure Service Bus] because there was not a suitable PHP library package available on [Packagist], even though there are several good ones for usage in Laravel.

## Development scope

[Azure Service Bus], or ASB, offers cloud-scale messaging solutions where scalability, high-availability, reliability, and security are important factors to decouple your application integrations.

The following functionalities need to be provided by this library:

1. Queues: sending messages to and reading from a single queue
2. Topics: providing queue functionality for publisher/subscriber situations, well suited for event based projects
3. Namespaces: providing logical grouping of queues and topics

## Development workflow and requirements

This library offers support for PHP 7.4 and 8.0. At the time of starting this project, Linux App Services don't support 8.1 yet and Windows App Services are no longer maintained and have the latest PHP version set to 7.4, even though it is now no longer possible to create a Windows App Service for PHP.

I apply Test-Driven Development practices to create this library, because it allows me to experiment ideas quickly and keeps the code clean and on target.

- PHP: 7.4 and 8.0
- PHPUnit: 9.5

## How you can help?

Developing this solution by myself takes a while, especially since I'm spending my spare time to work on it. If you see a typo in the documentation or an error in the code, please fix the issue and submit a [pull request].

If you have a need for a framework free PHP library for [Azure Service Bus], and you have some time to spare, feel free to extend functionality, remove technical debt or improve the code.

Lastly, if you use this library, let us know how it solves your problems. Positive feedback is nice, but if the onboarding process is too complex, the features are not working as expected or things are broken in your environment, [create an issue]! The sooner a defect is reported, the faster it can be solved.

[Azure Service Bus]: https://azure.microsoft.com/en-us/services/service-bus/
[create an issue]: https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue
[Packagist]: https://www.packagist.org
[pull request]: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request
[RabbitMQ]: https://www.rabbitmq.com
