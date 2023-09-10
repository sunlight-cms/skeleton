SunLight CMS skeleton
#####################

This is a SunLight CMS template project.

.. contents::


Creating a new project
**********************

You can create a new project using the Composer's `create-project <https://getcomposer.org/doc/03-cli.md#create-project>`_ command:

.. code:: bash

   composer create-project sunlight-cms/skeleton my-website

This will create a "my-website" directory with all of the required files inside.


SunLight console
****************

This project contains preconfigured `sunlight-cms/console <console_>`_
which is used to maintain the CMS files.

- CMS files are downloaded automatically after you run ``composer install`` or ``composer update``
- the console reads configuration from your project's *composer.json*
- see `sunlight-cms/console documentation <https://github.com/sunlight-cms/console#configuration>`_
  for a list of all available commands and options


Default .gitignore
******************

There is a default *.gitignore* file that ignores most of the CMS files.

The idea is to commit only your templates and/or plugins and rely
on the `console`_ to maintain the CMS files.


Updating SunLight CMS
*********************

When a new project is created, the latest 8.x version of SunLight CMS is downloaded.
That version is then set into cms.version_.


Applying patches
================

If you wish to upgrade to a newer version, you can apply `patches <https://sunlight-cms.cz/resource/8.x/update>`_
using the ``bin/console cms.patch`` command. This will also update cms.version_ in *composer.json*.


Redownloading CMS files
=======================

If you just want to overwrite the CMS files with a different version, you can edit cms.version_
manually and then run ``bin/console cms.download --overwrite``. Note that doing this will not
patch your database or perform any other updates.


.. _console: https://github.com/sunlight-cms/console
.. _cms.version: https://github.com/sunlight-cms/console#version
