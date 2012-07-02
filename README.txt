// $Id: README.txt,v 1.00 2011/02/08 17:04:38 md-2 Exp $

CONTENTS OF THIS FILE
---------------------

 * Introduction
 * Installation
 * Usage


INTRODUCTION
------------

Current Maintainer: Mark Davies <mark@618designs.co.uk>

Uber_Invoice is a simple helper module that allows users to override the 
default Ubercart invoice templates by enabling the module and editing the 
templates contained within this module.

This helps you have invoice templates per site, if running a multi site 
install.

The module contains the following files which should not be edited.
-uc_order.tpl.php
-uc_order-admin.tpl.php
-uc_order-customer.tpl.php

These are ubercart core invoice templates and are required in the module 
folder to allow the override to work.


INSTALLATION
------------

1. Drop the module into sites/all/modules/ or if your running multisite, drop the module into
	 sites/<yoursite.com>/modules/.

2. Enable the module


USAGE
------------

1. The module comes with two predefined invoice templates that can be edited.
		-uc_order-ubercustomer.tpl.php
		-uc_order-uberadmin.tpl.php
		
		Edit these invoices as you wish and save.
		
		Additional templates can be created by editing uber_invoice_uc_invoice_templates()
		function in the uber_invoice.module file (See comments).
		
2.  After you made your changes you need to select the template in the Ubercart configuration
		and also modify the conditional actions to use your new template.