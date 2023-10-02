# lando-drupal-base
Use this to create a local [Drupal](https://www.drupal.org/) site using [Lando](https://lando.dev/).

* Lando 3.18.0
* Drupal 10.1.4 (drupal/recommmended-project)
* Drush 12.2.0

## Setup
Download the source to the directory of your choosing and execute the following commands.
```
lando start

Wait a while...

lando drush site:install --db-url=mysql://drupal10:drupal10@database/drupal10 -y
```

## Customizations
### Composer
The `web-root` has been changed from `web/` to `docroot/`.

The following config has been added in order to allow the build process to complete on Windows.
```
"process-timeout": 0
```
