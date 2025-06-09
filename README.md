# Human Resource Information System (HRIS)

A comprehensive Human Resource Information System built with CodeIgniter 4, featuring modern UI components and interactive features.

## Features

- User Authentication and Authorization
- Employee Management
- Leave Management
- Attendance Tracking
- Payroll Management
- Department Management
- Position Management
- Document Management
- Reports Generation
- Settings Management

## Technologies Used

### Framework and Core Technologies
- CodeIgniter 4 (PHP Framework)
- PHP 8.1 or higher
- MySQL/MariaDB

### Frontend Libraries
- Tabler Core (UI Framework) - Version 1.0.0-beta21
- jQuery - Version 3.7.1
- SweetAlert2 - Version 11.15.10 (for beautiful alerts and notifications)
- SweetAlert2 Borderless Theme - Version 5.0.26

### Development Tools
- PHPUnit for testing
- Faker for generating test data
- VFSStream for virtual filesystem testing

## Project Structure

The project follows a typical MVC (Model-View-Controller) architecture with the following components:

- **Controllers/** - Contains the application's business logic
- **Models/** - Database models and data handling
- **Views/** - User interface templates
- **Config/** - Application configuration files
- **Services/** - Business logic services
- **Validations/** - Form and data validation rules
- **Enums/** - Enumeration classes
- **Rules/** - Custom validation rules
- **Libraries/** - Custom libraries
- **Traits/** - Reusable PHP traits
- **Filters/** - Request/Response filters
- **Database/** - Database migrations and seeds
- **Helpers/** - Helper functions
- **Language/** - Internationalization files

## What is CodeIgniter?

CodeIgniter is a PHP full-stack web framework that is light, fast, flexible and secure.
More information can be found at the [official site](https://codeigniter.com).

This repository holds a composer-installable app starter.
It has been built from the
[development repository](https://github.com/codeigniter4/CodeIgniter4).

More information about the plans for version 4 can be found in [CodeIgniter 4](https://forum.codeigniter.com/forumdisplay.php?fid=28) on the forums.

You can read the [user guide](https://codeigniter.com/user_guide/)
corresponding to the latest version of the framework.

## Installation & updates

`composer create-project codeigniter4/appstarter` then `composer update` whenever
there is a new release of the framework.

When updating, check the release notes to see if there are any changes you might need to apply
to your `app` folder. The affected files can be copied or merged from
`vendor/codeigniter4/framework/app`.

## Setup

Copy `env` to `.env` and tailor for your app, specifically the baseURL
and any database settings.

## Important Change with index.php

`index.php` is no longer in the root of the project! It has been moved inside the *public* folder,
for better security and separation of components.

This means that you should configure your web server to "point" to your project's *public* folder, and
not to the project root. A better practice would be to configure a virtual host to point there. A poor practice would be to point your web server to the project root and expect to enter *public/...*, as the rest of your logic and the
framework are exposed.

**Please** read the user guide for a better explanation of how CI4 works!

## Repository Management

We use GitHub issues, in our main repository, to track **BUGS** and to track approved **DEVELOPMENT** work packages.
We use our [forum](http://forum.codeigniter.com) to provide SUPPORT and to discuss
FEATURE REQUESTS.

This repository is a "distribution" one, built by our release preparation script.
Problems with it can be raised on our forum, or as issues in the main repository.

## Server Requirements

PHP version 8.1 or higher is required, with the following extensions installed:

- [intl](http://php.net/manual/en/intl.requirements.php)
- [mbstring](http://php.net/manual/en/mbstring.installation.php)

> [!WARNING]
> - The end of life date for PHP 7.4 was November 28, 2022.
> - The end of life date for PHP 8.0 was November 26, 2023.
> - If you are still using PHP 7.4 or 8.0, you should upgrade immediately.
> - The end of life date for PHP 8.1 will be December 31, 2025.

Additionally, make sure that the following extensions are enabled in your PHP:

- json (enabled by default - don't turn it off)
- [mysqlnd](http://php.net/manual/en/mysqlnd.install.php) if you plan to use MySQL
- [libcurl](http://php.net/manual/en/curl.requirements.php) if you plan to use the HTTP\CURLRequest library
