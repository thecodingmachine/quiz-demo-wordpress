Quiz demo: Mouf + Wordpress
===========================

This repository contains a PHP Quiz demo application, running on Wordpress.

You can access the website by browsing http://demoquiz-wordpress.mouf-php.com

It is part of a wider demo, showcasing how to deploy on **same code** in many different environments.

The quiz code is stored in the [`thecodingmachine/quiz-module`](https://github.com/thecodingmachine/quiz-module) package.
It contains a [generic PSR-7 compatible controller](https://github.com/thecodingmachine/quiz-module/blob/master/src/Controllers/QuizController.php).
Using Mouf and a set of appropriate packages, the controller can then be deployed in a set of different environments:

- Mouf/Splash ([demo](http://demoquiz.mouf-php.com/)) ([code](https://github.com/thecodingmachine/quiz-demo-standalone))
- Wordpress ([demo](http://demoquiz-wordpress.mouf-php.com/)) ([code](https://github.com/thecodingmachine/quiz-demo-wordpress))
- Drupal 7 ([demo](http://demoquiz-drupal.mouf-php.com/)) ([code](https://github.com/thecodingmachine/quiz-demo-drupal))
- Joomla ([demo](http://demoquiz-joomla.mouf-php.com/)) ([code](https://github.com/thecodingmachine/quiz-demo-joomla))
- Magento ([demo](http://demoquiz-magento.mouf-php.com/)) ([code](https://github.com/thecodingmachine/quiz-demo-magento))

Installation
------------

- Clone the repository
- Run `composer install`
- Browse to the website root directory and run Wordpress install
- Browse to http://[your-website]/[path-to-wordpress]/vendor/mouf/mouf and run Mouf install process
- Connect to Wordpress administration http://[your-website]/[path-to-wordpress]/wp-admin
- Click the *Plugin* menu, then activate the `WP Router` and the `Moufpress` plugin
- You are done!
- Now, simply browse to: http://[your-website]/[path-to-wordpress]/quiz
