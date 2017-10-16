# Eliminación de SAPIs obsoletas y extensiones que no han sido portadas a PHP7
* Fecha: 2015-01-14
* Autor: Anatol Belski, <ab@php.net>
* Estado: Cerrada
* Original: http://wiki.php.net/rfc/removal_of_dead_sapis

## Introducción

Actualmente PHP contiene muchos SAPIs no disponibles o no soportados en servidores desde hace mucho tiempo. Lo mismo puede decirse de varias extensiones que son ha sido declarados como obsoletas hace mucho tiempo o las librerías de las que dependen ya no son compatibles. Aquí hay una lista corta:

## SAPIs eliminadas:
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

## Extensiones with dependencias obsoletas o que ya no son mantenidas por sus desarrolladores
* imap
* mcrypt

## Extensiones no portados ya a PHP7
* interbase
* mssql
* oci8
* pdo_dblib
* pdo_oci
* sybase_ct

## Estensiones deprecadas (obsoletas) manejadas por este otro RFC https://wiki.php.net/rfc/remove_deprecated_functionality_in_php7 (not gestiones en este  RFC)
* mysql
* ereg   

Esto lleva a la situación en la que el repositorio contiene mucho código no mantenido. El código que no se actualiza durante años o que depende de libreías muy pesadas que no actualizan, son candidatas a "deprecarse" en nuevas versiones del lenguaje. Además, el código no hace falta ser mantenido evitando riesgos de seguridad.

## Investigación (justitifación)

### sapi/aolserver
  * Server home: http://sourceforge.net/projects/aolserver/
  * Server last release: 2012
  * Server debian supported: yes
  * SAPI status: 5.4 builds with the latest server API
  
