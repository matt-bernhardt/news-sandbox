# Sandbox Drupal application built with Drupal-Composer

[![Build Status](https://travis-ci.org/matt-bernhardt/news-sandbox.svg?branch=master)](https://travis-ci.org/matt-bernhardt/news-sandbox)

This is an attempt to build a Drupal 8 application on the [Drupal-Composer](https://github.com/drupal-composer/drupal-project)
base project, which can then be deployed to a cloud provider.

## Deploy

This is our aspirational deploy process

```
git clone https://github.com/matt-bernhardt/news-sandbox.git /var/www/foo
cd /var/www/foo
composer install
```

At this point, the web server would be serving our application from
`/var/www/foo/web`

## Post-deploy steps

Hopefully this section can go away...

## Updating

After initially deploying the application, your local operations team will
need to keep up with core, theme, and module updates as they come out.

I need to write documentation for how to do this...

## Open questions

- The database, if there are any initial conditions, needs to be populated.
- Secrets need to be managed. Most likely this will come via `.env` files.
- Containerization? AWS? Where, exactly, is this going to be deployed?
