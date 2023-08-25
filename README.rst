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

By default it is configured to automatically download or update CMS files
after you run ``composer install`` or ``composer update``.


Default .gitignore
******************

There is a default *.gitignore* file that ignores most of the CMS files.

The idea is to commit only your templates and/or plugins and rely
on the `console`_ to maintain the CMS files.


Configuration
*************

By default, the latest 8.x version of SunLight CMS will be downloaded.

See `sunlight-cms/console documentation <https://github.com/sunlight-cms/console#configuration>`_
for more information about configuration.


.. _console: https://github.com/sunlight-cms/console
