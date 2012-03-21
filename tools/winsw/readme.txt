Windows service wrapper - Wrapper для процессов windows (для nginx и php-fpm)
===============================================================================

Позволяет запускать любое приложение Windows как сервис.
Я использую для запуска php-cgi сервера.

Официальный сайт: http://kenai.com/projects/winsw/pages/Home

Download
================
The binaries are available here(http://maven.dyndns.org/2/com/sun/winsw/winsw/) for download.

Usage
================
During your development... 
 Take winsw.exe from the distribution, and rename it to your taste (such as myapp.exe) 
 Write myapp.xml (see Configuration Syntax for more details) 
 Place those two files side by side when you deploy your application, because that's 
 how winsw.exe discovers its configuration. 

 At runtime... 
 To install a service, run myapp.exe install
 To start a service, run myapp.exe start
 To stop a service, run myapp.exe stop
 To restart a service, run myapp.exe restart
 To uninstall a service, run myapp.exe uninstall

 When there's a problem, these commands also report an error message to stderr. On a successful completion, 
these commands do no produce any output and exit with 0. 

In addition, you can also run myapp.exe status to have it print out the current status of the service to stdout. 
Again, any error encountered during the processing would cause output to be reported to stderr. 

All these commands use the same set of exit code to indicate its result.
