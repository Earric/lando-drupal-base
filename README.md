# lando-drupal-base
Use this to create a local [Drupal](https://www.drupal.org/) site using [Lando](https://lando.dev/).

Drupal 10.1.4
Drush 12.2.0

Download the source to the directory of your choosing and execute the following commands.
```
lando start
lando drush site:install --db-url=mysql://drupal10:drupal10@database/drupal10 -y
```