---
title: Instalacion Aranda AVS Gateway
info:
---
🕐 Ultima actualización: MAYO 7  de 2020

-Para empezar a instalar el Aranda AVS Gateway, se debe hacer doble clic en el archivo **avsg_8.1.0**.
Haga clic en **Next**.
-Confirme el inicio de la instalación presionando **Next**.
-El nombre del Sitio donde se instalará el Aranda AVS Gateway está predeterminado, al igual que el del Directorio Virtual del IIS (ArandaGateway). Sin embargo, si desea instalar la aplicación en otro directorio virtual, puede ingresarlo manualmente. Presione**Next**.
-Espere a que los archivos se instalen.
-Cuando el proceso esté terminado, presione </span[Close].
-Al terminar este proceso, se carga una ventana, para la configuración inicial del Aranda AVS Gateway, con el nombre Aranda AVS Gateway Configurator. En esta ventana, se configura la base de datos a utilizar, previamente instalada, y el usuario de correo SMTP a utilizar para notificaciones a los administradores del Gateway.
-Compruebe que la conexión a base de datos es correcta, haciendo clic en  **Test**.
-Si la conexión es correcta, guárdela haciendo clic en **Guardar**.
-Luego de esto, de clic en **Salir** para terminar el proceso.
-Diríjase a Inicio -> Panel de Control -> Herramientas administrativas -> Servicios de Internet Information Server.
-Verifique que se haya creado dentro del Sitio Web Predeterminado del servidor, un directorio virtual con el nombre definido del instalador.
-Haga clic derecho -> Propiedades -> **ASP.NET** sobre cada una de las tres carpetas y verifique   que se haya seleccionado el Framework 2.0. Haga clic en **Aceptar**.
-Si desea que la aplicación Web sea accedida directamente Utilizando las credenciales del usuario autenticado, haga clic derecho -> Propiedades -> [Seguridad de directorios] sobre la carpeta ASM del sitio Web predeterminado en el IIS. Presione **Modificar** y marque la casilla Autenticación de Windows integrada. Haga clic en **Aceptar**.
-Con esto queda instalado el Aranda AVS Gateway como servicio Windows, y un Web Service para la administración de Licenciamiento del Aranda AVS Gateway, el cual es utilizado por el Aranda AVS Web Admin.
Puede probar el correcto funcionamiento del Web Service, ingresando a la URL del sitio en un Navegador **LicensingWebManager**.
Es recomendable dejar el servicio Windows abajo, hasta que se tenga el Aranda AVS Web Admin funcionando, ya que el Aranda AVS Gateway requiere tener conocimiento de donde está corriendo el Administrador.
 

