# PHP RFC: Removal of dead or not yet PHP7 ported SAPIs and extensions
* Version: 2
* Date: 2015-01-14
* Author: Anatol Belski, <ab@php.net>
* Status: Closed
* First Published at: http://wiki.php.net/rfc/removal_of_dead_sapis

## Introduction

Currently PHP contains many SAPIs to the servers either completely unavailable or unsupported for a long time. The same can be said about several extensions which are for long deprecated or their dependency libraries are unsupported. Here's a short list:

## Dead SAPIs:
* aolserver
* apache
* apache_hooks
* caudium
* continuity
* isapi
* milter  
* phttpd
* pi3web
* roxen
* thttpd
* tux
* webjames
* apache2filter - not really dead, but currently broken
* nsapi