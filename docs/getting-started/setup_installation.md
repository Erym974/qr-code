# Getting Started

## Import project

You need to clone the repository on your computer.

You can use : 

```bash
git clone https://github.com/webmix/qr-code.git
```

## Environment variables

Basic template for the .env file : 

Please reaplace all %VALUE% by your value.

```bash

CORS_ALLOW_ORIGIN='^https?://(localhost|127\.0\.0\.1)(:[0-9]+)?$'

###> symfony/webapp-pack ###
MESSENGER_TRANSPORT_DSN=doctrine://default?auto_setup=0
###< symfony/webapp-pack ###

###> symfony/framework-bundle ###
APP_ENV=dev
APP_SECRET= %YOUR APP SECRET KEY%

DATABASE_URL="mysql://%MYSQL_USERNAME%:%MYSQL_PASSWORD%@%MYSQL_HOST%:%MYSQL_PORT%/%MYSQL_DATABASE_NAME%?serverVersion=8.0&charset=utf8mb4"

###> symfony/messenger ###
MESSENGER_TRANSPORT_DSN=doctrine://default
###< symfony/messenger ###

###> symfony/mailer ###
MAILER_DSN=%YOUR MAILER DNS%
###< symfony/mailer ###

###> stripe ###
SECRET_STRIPE=%YOUR STRIPE TOKEN%
WEBHOOK_STRIPE=%YOUR STRIPE WEBHOOK TOKEN%
###< stripe ###

###> TimeZone ### 
APP_TIMEZONE="Europe/Paris"
###< TimeZone ###

###> Socket ###
SOCKET_TOKEN=%RANDOMLY SOCKET TOKEN%
SOCKET_PORT=%PORT YOUR WANT TO USE FOR SERVER%
###< Socket ###


###> lexik/jwt-authentication-bundle ###
JWT_SECRET_KEY=%RANDOM PRIVATE KEY%
JWT_PUBLIC_KEY=%RANDOM PUBLIC KEY%
JWT_PASSPHRASE=2bbec748f00942c63e16b8f2fa39bb92
###< lexik/jwt-authentication-bundle ###

```