Para deployar el CAS:
===

* La carpeta cas, deberá ser deployada en webapps de tomcat.  
* La carpeta etc/cas, deberá ser copiada en la misma ubicación con permisos para el usuario tomcat.  
* La carpeta opt, contiene el keystore a ser utilizado con el tomcat para funcionar sobre SSL.  
* La carpeta lib, contiene las librerias que se necesitan agregar al tomcat para funcionar correctamente.  
* La carpeta conf, tiene los archivos de configuración del tomcat con los parametros necesarios para utilizar el cas (SSL con el keystore).  


**Se asumen las siguientes condiciones**:  

* Los hosts spr.stp.gov.py y login.stp.gov.py, apuntan a localhost (127.0.0.1).  
* La base de datos spr, se encuentra en localhost y la constraseña del usuario postgres es stp123.  
* Memcached se encuentra instalado en el equipo local.  
 
** Si desea ajustar las credenciales de base de datos favor editar el archivo**:  
 
* cas/WEB-INF/deployerConfigContext.xml a partir de la linea 52.  