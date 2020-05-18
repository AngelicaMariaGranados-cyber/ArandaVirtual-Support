---
title: IntroducciónInstalacion Base de Datos AVS
info:
---
🕐 Ultima actualización: MAYO 7  de 2020

-Para empezar a instalar la base de datos de AVS, se debe hacer doble clic en el archivo **avsdb_8.0.1**.
Haga clic en **Next**.
-Confirme el inicio de la instalación presionando **Next**.
-Espere a que los archivos se instalen.
-Cuando el proceso esté terminado, presione **Close**.
-Diríjase a Inicio -> Programas -> Aranda Software -> Aranda Tools -> Aranda AVS DB Installer.
-A continuación podrá seleccionar el motor de base de datos, SQL Server 2005 (o superior), indicando la información de servidor, usuario y base de datos.
-El proceso se tomará algunos minutos, sujeto a tiempos de respuesta del servidor de base de datos. Se pueden presentar inconvenientes de permisos de usuario y conexión, se recomienda verificar estos datos.
-Posterior a esto, puede verificar la creación de la base de datos, debe tener 22 tablas, 19 procedimientos almacenados.
-Se puede verificar que algunas tablas contienen datos por defecto, a saber:
a. AVS_GATEWAY_BASE: Configuración del servicio de Aranda AVS Gateway, estos datos son administrados por el Aranda AVS Web Admin, contiene datos como:
-Puerto, por defecto está el 443
-Tamaño de los paquetes de listados de información, por defecto 24 usuarios por paquete
-Tiempo de auditoría, por defecto 500 mili segundos.
-Tiempo de espera para conexión de servicio entre clientes, 300000 mili segundos por defecto
-Flag de SSL, por defecto en 1, habilitado
-Asunto del certificado digital a utilizar, en caso de usar un certificado del directorio de la máquina, por defecto: arandasoft.com
-AVS_SERVICE: Definición de los servicios que soporta Aranda AVS Gateway, estos datos no son administrables, esta información es vital para el correcto funcionamiento del Servicio, no se recomienda modificarla.

 -AVS_SW_CLIENT y AVS_SW_VERSION: Definición de los clientes que se pueden comunicar con el Aranda AVS Gateway, como lo son Consolas y Agentes. Desde el Aranda AVS Web Admin se puede actualizar los clientes, cargando un archivo .dat, que debe cumplir con la estructura propia, esto actualiza la versión del cliente que se notifica al momento de reportar autenticación, para que sea actualizado, descargando el instalador en la dirección reportada al cliente.

-AVS_USER y AVS_ROLE: Definición de usuarios y sus respectivos roles en la aplicación. Los roles no son administrables, no es recomendable modificar esta información. Los usuarios son gestionados por el Aranda AVS Web Admin. El nombre de usuario por defecto es “admin” y la contraseña es “123”, es recomendable cambiarla al ingresar al sitio.

-Con estos pasos, está terminado el proceso de instalación de la base de datos de Aranda Virtual Support.


