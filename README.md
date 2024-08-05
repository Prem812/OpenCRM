# Open crm

## Screenshots

### Dashboard

![Open CRM light-dashboard screenshot](screenshots/dashboard-light.png "Open CRM dashboard light screenshot")
![Open CRM dark-dashboard screenshot](screenshots/dashboard-dark.png "Open CRM dashboard dark screenshot")

### Accounts

![Open CRM light-accounts screenshot](screenshots/accounts-light.png "Open CRM accounts light screenshot")
![Open CRM dark-accounts screenshot](screenshots/accounts-dark.png "Open CRM accounts dark screenshot")

### Contacts

![Open CRM light-contacts screenshot](screenshots/contacts-light.png "Open CRM contacts light screenshot")
![Open CRM dark-contacts screenshot](screenshots/contacts-dark.png "Open CRM contacts dark screenshot")

### Leads

![Open CRM light-leads screenshot](screenshots/leads-light.png "Open CRM leads light screenshot")
![Open CRM dark-leads screenshot](screenshots/leads-dark.png "Open CRM leads dark screenshot")

### Deals

![Open CRM light-deals screenshot](screenshots/deals-light.png "Open CRM deals light screenshot")
![Open CRM dark-deals screenshot](screenshots/deals-dark.png "Open CRM deals dark screenshot")

### Products

![Open CRM light-products screenshot](screenshots/products-light.png "Open CRM products light screenshot")
![Open CRM dark-products screenshot](screenshots/products-dark.png "Open CRM products dark screenshot")

<!-- [![Tests](https://github.com/frikishaan/tiny-crm/actions/workflows/run-tests.yml/badge.svg?branch=main)](https://github.com/frikishaan/tiny-crm/actions/workflows/run-tests.yml) -->

This is a small sized Open-source CRM application for medium size business to handle Customer relationship it is created by Prem Sagar Shah using the [Filament PHP](https://filamentphp.com/).

## Technologies

-   PHP (Laravel)
-   Filament PHP

## Local Installation

1. Clone the repository

```
git clone https://github.com/Prem812/OpenCRM.git
```

2. Run the following commands -


Change Directory

```
cd OpenCRM
```


install php dependencies

```
composer install
```


install JavaScript dependencies

```
npm install
```


build assets

```
npm run build 
```


Setup Configuration

```
cp .env.example .env
```


Verify your Database Connection

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=tiny_crm
DB_USERNAME=root
DB_PASSWORD=
```

Generate Key

```
php artisan key:generate
```


Migrate and Seed Database

```
php artisan migrate:fresh --seed
```


Optionally, you can create the dummy data by running the seeder as -

```php artisan db:seed
```


Run the project on your local machine

```
php artisan serve
```

## Need assistance for creating new pages?


you can go through filaments doucumentation or create using these commands:

-  firstly you should create a model with migration table

```
php artisan make:model model_name -m
```

-  it will create a new model in your project with your model name and it will also create a new migration table in your project modify the migration table as what you need

-  run the command 

```
php artisan migrate
```

for resource

```
php artisan make:filamentresource Model_NameResource --generate --view
```

and there you go

for more information go through the [documentation](https://filamentphp.com/docs/3.x/panels/installation)


If you need help customizing this application or want to create your own application like this, contact me on [LinkedIn](https://www.linkedin.com/in/prem-sagar-shah-267921174/).
