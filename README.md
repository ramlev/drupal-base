# Composer base Drupal 10 base installation

This project template provides a fast kickstart to a new Drupal site.

## Installation

I assume you know basic Composer and PHP skills.

`composer create-project ramlev/drupal-base:dev-develop --no-interaction YOUR_DIR`

After that, you can setup your LAMP or whatever based webserver. I normally use DDEV.

With that, you can do something like this.

```bash
cd YOUR_DIR
ddev config

## press enter to everything
ddev start

## Wait until it's up and running

## Install the default site
ddev drush si -y

## Change admin user password
ddev drush upwd admin test

Now you can login with `admin` / `test`
```

## Available contrib modules

* admin_toolbar
* adminimal_theme
* module_filter
* pathauto
* redirect
* simple_sitemap
* token
* twig_tweak
* ultimate_cron
* drush

And some modules, only added with "dev"

* devel
* ray_debugger
* phpstan

## Add even more features

You can add more contribs and so on like normally

```sh

## Go into your dir
cd YOUR_DIR

## Add the search_api contrib module, or whatever needed.
composer req drupal/search_api
```

Go into Drupal admin and enable whatever modules and / or themes you need.

Happy hacking

Hasse Ramlev Wilson

Ramlev.dk
