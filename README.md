# basic-symfony-docker-template

## Setup
1. Update git credentials in php/Dockerfile
1. Run: `docker compose up -d --build`
1. Run: `docker compose exec php bash`
1. Run: `symfony check:requirements`
1. Run: `symfony new .`
1. Verify site is operational at http://localhost
1. Run: `composer require twig doctrine`
1. Run: `composer require --dev maker ormfixtures fakerphp/faker`
1. Run: `cp .env .env.local`
1. Change: DATABASE_URL="mysql://root:secret@database:3306/symfony_docker"

composer require --dev symfony/maker-bundle

## Test Suite
1. composer require --dev symfony/test-pack

1. composer require --dev vimeo/psalm
1. ./vendor/bin/psalm --init