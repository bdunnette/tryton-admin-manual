Introduction
============
This document describes the way of administration and configuration of the Tryton system. With the help of this manual you create a working application that can support your organisation processes.
This manual is primarily targeted on the Tryton administrator. This manual can also be used to write a Tryton user manual.

Contributors
------------
+----------------+------------------------------------+
|Name            |Contributions                       |
+================+====================================+
|Anthony Schrijer|* Initial setup of the manual       |
| 		 |* Basic configuration of the system |
|                |* Configuring accounts              |
|                |* Configuring Party management      |
|                |* Creating Products                 |
|                |* Writing style conventions         |
|                |* Style sheet                       |
+----------------+------------------------------------+

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
