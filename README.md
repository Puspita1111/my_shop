Aimeos logo

Total Downloads Latest Stable Version License Open issues

  

⭐ Star us on GitHub — it motivates us a lot! 😀

Aimeos GitHub stats

Aimeos - THE Laravel ecommerce platform
Aimeos is THE ultra-fast, cloud-native and API-first e-commerce platform! You can install it within 5 minutes and can adapt, extend, overwrite and customize anything to your needs.

Aimeos Laravel demo

Features
Aimeos is a full-featured e-commerce package:

JSON REST API based on jsonapi.org
GraphQL API for administration
Perfect fit for AWS, Google, Azure and Kubernetes based clouds
Multi vendor, multi channel and multi warehouse
From one to 1,000,000,000+ items
Extremly fast down to 20ms
For multi-tentant e-commerce SaaS solutions with unlimited vendors
Bundles, vouchers, virtual, configurable, custom and event products
Subscriptions with recurring payments
100+ payment gateways
Full RTL support (frontend and backend)
Block/tier pricing out of the box
Extension for customer/group based prices
Discount and voucher support
Flexible basket rule system
Full-featured admin backend
Beautiful admin dashboard
Configurable product data sets
Completly modular structure
Extremely configurable and extensible
Extension for market places with millions of vendors
Fully SEO optimized including rich snippets
Translated to 30+ languages
AI-based text translation
Optimized for smart phones and tablets
Secure and reviewed implementation
High quality source code
... and more Aimeos features

Supported languages:

English German French Spanish Dutch Italian Portuguese Danish Finnish Swedish Norwegian     Polish Hungarian Russian Ukrainian Croatian Slovenian Romanian Czech Serbian Slovak Estonian Latvian     Turkish Arabic Persian     Chinese Japanese Indonesian Vietnamese Burmese Korean

Check out the demos:

Aimeos frontend demo
Aimeos admin demo
Headless distribution
To build a single page application (SPA) respectively a progressive web application (PWA), the Aimeos headless distribution is the right choice with API-only and JWT authentication pre-configured:

⭐ Aimeos headless distribution

Integrate into existing applications
You already have an existing Laravel application and want to add a shop to your web site? Install the Aimeos composer package for Laravel and add e-commerce to your existing application in minutes:

⭐ Aimeos Laravel package

Standalone application
Requirements
Installation
Frontend
Backend
Customize
Multi-vendor
License
Links
Requirements
The Aimeos shop distribution requires:

Linux/Unix, WAMP/XAMP or MacOS environment
PHP >= 8.0.11
MySQL >= 5.7.8, MariaDB >= 10.2.2, PostgreSQL 9.6+, SQL Server 2019+
Web server (Apache, Nginx or integrated PHP web server for testing)
If required PHP extensions are missing, composer will tell you about the missing dependencies.

If you want to upgrade between major versions, please have a look into the upgrade guide!

Installation
To install the Aimeos shop application, you need composer 2.2+. On the CLI, execute this command for a complete installation including a working setup:

wget https://getcomposer.org/download/latest-stable/composer.phar -O composer
php composer create-project aimeos/aimeos myshop
You will be asked for the parameters of your database and mail server as well as an e-mail and password used for creating the administration account.

In a local environment, you can use the integrated PHP web server to test your new Aimeos installation. Simply execute the following command to start the web server:

cd myshop
php artisan serve
Note: In an hosting environment, the document root of your virtual host must point to the /.../myshop/public/ directory and you have to change the APP_URL setting in your .env file to your domain without port, e.g.:

APP_URL=http://myhostingdomain.com
Frontend
After the installation, you can test the Aimeos shop frontend by calling the URL of your VHost in your browser. If you use the integrated PHP web server, you should browse this URL: http://127.0.0.1:8000

Aimeos frontend

Backend
The Aimeos administration interface will be available at /admin in your VHost. When using the integrated PHP web server, call this URL: http://127.0.0.1:8000/admin

Aimeos admin backend

Customize
Laravel and the Aimeos e-commerce package are extremely flexible and highly customizable. A lot of documentation for the Laravel framework and the Aimeos e-commerce framework exists. If you have questions about Aimeos, don't hesitate to ask in our Aimeos forum.

For more details about Aimeos Laravel integration, please have a look at its repository.

Multi-language
For shops which offers multiple languages, just add this line to your ./myshop/.env file:

SHOP_MULTILOCALE=true
Then, the language will be added to the routes automatically. You can set up the available languages in the "Locale > Locale" panel of the Aimeos admin backend.

Multi-vendor
To enable multi-vendor features, add this settings to the ./myshop/.env file:

SHOP_MULTISHOP=true
If you want to allow vendors to register themselves as sellers, set this option in the ./myshop/.env file too:

SHOP_REGISTRATION=true
By default, newly registered sellers have administrator privileges in the backend for their own site. For a more limited access to the backend, you can change the permission level to "editor" in the ./myshop/.env file:

SHOP_PERMISSION=editor
You can change the permissions associated to "admin" or "editor" by adding your own version of the JQAdm resource configuration to the "admin" section of your ./config/shop.php file.

License
The Aimeos shop system is licensed under the terms of the MIT and LGPLv3 license and is available for free.

Links
Web site
Documentation
Forum
Issue tracker
Composer packages
Source code
