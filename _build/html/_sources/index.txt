.. Tryton Administration Manual documentation master file, created by
   sphinx-quickstart on Fri Oct  7 14:50:28 2011.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to the Tryton Administration Manual!
========================================================

Contents:

.. toctree::
   :maxdepth: 2

Introduction
============
This document describes the way of administration and configuration of the Tryton system. With the help of this manual you create a working application that can support your organisation processes.
This manual is primarily targeted on the Tryton administrator. This manual can also be used to write a Tryton user manual.

Contributors
------------
+----------------+-----------------------------------+
|Name            |Contributions                      |
+================+===================================+
|Anthony Schrijer|* Initial setup of the manual      |
| 		 |* Basic configuration of the system|
|                |* Configuring accounts             |
|                |* Configuring Party management     |
|                |* Creating Products                |
|                |* Writing style conventions        |
|                |* Style sheet                      |
+----------------+-----------------------------------+

Presumptions
============
In this chapter we mention the presumptions that are made before you can do the configuration of the Tryton system.

In this manual most settings are made with a European viewpoint; adapt the settings to your local needs.

* This manual is written for the Tryton server version 2.0 with the corresponding Tryton client (GUI) as the user interface.
* With the Tryton client you must be able to make a connection to a database and you must be able to log in.

Tryton installation specifications
----------------------------------
When Tryton is installed there is initially no database. In this configuration is expected that you have created a database with these settings:

* Tryton Server Password: the password that is used during installation of the Tryton server.
* Tryton database name: databasename
* Tryton administrator name: admin
* Password administrator: password used for the administrator during database installation.
* Standard language: English (choosen in this manual for ease of use and as starting point for translations of this manual).


Basic Configuration
===================
When a new database is created in Tryton and when you log in that database for the first time, you get the screen:
*Welcome to the module configuration wizard!*

Click on the *OK* button if you want to configure modules.

Creating users
--------------
The first configuration step in the wizard is *Add users*.
If you want to create new users click on the *OK* button.

.. figure:: user-screen.png
   :scale: 50 %
   
   The User tab on the Users screen

On the screen Users, go to the User tab:

User Tab
""""""""

    * Name: The real name of the user.
    * Login: The login name of the user.
    * Password: The user login password.
    * Email: The e-mail address of this user.
    * Home action: The initial “home” screen for this user, usually set to “Menu” (see below) - for instance, for a user primarily entering sales, this can be set to Sales or New Sale.
    * Menu action: The menu viewed by the user.


Check the Active box if you want this user to be active. You can block the access of an user by unchecking this box.

Access Permissions Tab
""""""""""""""""""""""

Under Groups click on the *Add* button and select the groups to which the user will belong.
Select existing groups or create a new one.

Under Rules click on the *Add* button to add a rule.
With a rule you can manage in detail what kind of access a user has on the different modules/fields.
Click on the New button and you get the Record rules screen.

    * Model: The model description.
    * Global: Check this box so the rule becomes global and every user must follow this rule.
    * Default: If you check this box the rule will be added to all users by default.
    * Read access: Check this box if you want to give read access to model.
    * Write access: Check this box if you want to give write access to the model.
    * Create access: Check this box if you want to give create access to the model.
    * Delete access: Check this box if you want to give delete access to the model.
    * Name: Name of the rule.

Preferences Tab
"""""""""""""""

    * Language: Select the system language for the user.
    * Timezone: Select the timezone in which the user works.


When you have finished all the tabs for this user then click on the Add button. The user will be added to the system.

A new empty User screen will appear for adding another user. If you do not want to add more users click on the End button.

Installing modules
------------------
After you have added users with the wizard, a list of installable modules appear.

To start a minimal system select first an accounting module by double clicking on the name and then click on the *Mark for Installation* button.

* account_nl # Select the accounting module for your country.

Click on the tab Dependencies.

When you select a module to install, other modules on which it is dependent will be installed too (in this case the module account will be installed too).

When you have selected the module you want to install, click on the button *Perform Pending Installation/Update*. The screen System Upgrade appears with all the modules that will be installed.
Click on the button Start Upgrade.
When the module is installed, the wizard Welcome to the module configuration wizard! appear.
Click on the OK button if you want to configure modules.


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

