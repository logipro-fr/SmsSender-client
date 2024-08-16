# Sms Sender Client

A PHP component to use Sms sender' API within your PHP project.

**Sms sender** allows you to send SMS messages using the API.

## Feature

### Available Methods

**Sms sender client** provides one public method :
* `sendSms(string $messageText, string $receiverPhoneNumber)`: Sends an SMS with the specified `messageText` to the given `receiverPhoneNumber`. Returns a boolean indicating success.


## Installation

```shell
composer require logipro/SmsSender-client
```

## To contribute to Sms Sender Client 
### Requirements:
* Docker
* Git
* A bash shell

### Unit tests
Run unit tests with:

```shell
bin/phpunit
```

### Integration tests
Run integration tests with:

```shell
bin/phpunit-integration
```
**integration tests can only be run if you have a running [Sms Sender](https://github.com/logipro-fr/Sms.git) instance**

### Quality
#### Some indicators:
* PHP CodeSniffer (PSR12)
* PHPStan level 9
* Test coverage = 100%
* Mutation Score Indicator (MSI) = 100%


#### Quick check with:
```shell
./codecheck
```


#### Check coverage with:
```shell
bin/phpunit --coverage-html var
```
Then, view the coverage report in your browser at 'var/index.html'.


#### Check infection with:
```shell
bin/infection
```
Then, view the infection report in your browser at 'var/infection.html'.