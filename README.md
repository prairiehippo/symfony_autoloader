symfony_autoloader
==================

A Drupal 7 module to integrate the Symfony classloader for custom modules.

Excited by the thought of using the Symfony classloader in an upcoming Drupal 8 project?  Why not try it out in Drupal 7!

Turns out it's extremely simple to get the magic of the Symfony class loader up and running in a Drupal 6 or 7 system.  While this module is currently for Drupal 7, it's a simple matter of updating the .info file to get the same functionality in Drupal 6.

Installation
============
Download the Symfony Classloader component into your Drupal 7 sites library directory.
Full path to the class loader file should look like this: sites/all/libraries/Symfony/Component/ClassLoader/UniversalClassLoader.php

Enable the symfony_autoloader module.

Done.

Usage
=====
Checkout the included symfony_autoloader_example module for a trival example.

In general, all one needs to do is reference properly namespaced classes using the following pattern:

symfony_autoloader_register_namespace(array('Namespace' => 'dir'));

Note: all paths are based on site root.

License
=======
This code is free to be used by any and all - I do ask if you think of any improvements please submit a pull request so I can add it to my repository.

Thanks!