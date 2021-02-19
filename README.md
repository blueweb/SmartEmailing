# SmartEmailing

Easy way to interact with SmartEmailing API from PHP

## Installation

The best way to install this component is using [Composer](http://getcomposer.org/):

```sh
$ composer require blueweb/smartemailing
```

Then it is required to add the following lines to config.neon:

```
parameters:
	smartemailing:
		username: <smartemailing_username>
		token: <smartemailing_api_token>

services:
	- Blueweb\SmartEmailing(%smartemailing.username%, %smartemailing.token%)
```

## Usage

```importContact($contactlists, $properties, $customfields, $purposes, $settings)```

Insert a new contact into SmartEmailing lists. `$contactlists`, `$properties`, `$customfields`, `$purposes` and `$settings` are arrays.



