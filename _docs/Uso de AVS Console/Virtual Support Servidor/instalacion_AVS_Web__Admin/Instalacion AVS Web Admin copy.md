---
title: Instalacion Aranda AVS Web Admin
info:
---
🕐 Ultima actualización: 7 mayo de 2020

No inicie este procedimiento sin antes haber instalado la Base de Datos de AVS y el Aranda AVS Gateway, ya que el proceso hace referencia a estas instalaciones.

-Para empezar a instalar Aranda AVS Web Admin, se debe hacer doble clic en el archivo **avswa_8.1.0**.
-Haga clic en **Next**.
-Confirme el inicio de la instalación presionando **Next**.
-El nombre del Sitio donde se instalará **_Aranda AVS Web Admin_** está predeterminado, al igual que el del     Directorio Virtual del IIS **_(ArandaGatewayAdmin)_**. Sin embargo, si desea instalar la aplicación en otro directorio virtual, puede ingresarlo manualmente. Presione **Next**.
-Espere a que los archivos se instalen.
-Cuando el proceso esté terminado, presione **Close**.
-Al terminar este proceso, se carga una ventana, para la configuración inicial del **_Aranda AVS Web Admin_**, con el nombre **_Aranda AVS Web Admin_**. En esta ventana, se configura la base de datos a utilizar, previamente instalada, y la URL del Web Service de licenciamiento del Aranda AVS Gateway, previamente instalado.
-Compruebe que la conexión a base de datos es correcta, haciendo clic en  **Test**.
Si la conexión es correcta, guárdela haciendo clic en **Guardar**.
-Luego de esto, de clic en **Salir** para terminar el proceso.
-Diríjase a Inicio -> Panel de Control -> Herramientas administrativas -> Servicios de Internet Information Server.
-Verifique que se haya creado dentro del Sitio Web Predeterminado del servidor, un directorio virtual con el nombre definido del instalador.
-Haga clic derecho -> Propiedades -> **ASP.NET** sobre cada una de las tres carpetas y verifique   que se haya seleccionado el Framework 2.0. Haga clic en **Aceptar**. 
-Si desea que la aplicación Web sea accedida directamente Utilizando las credenciales del usuario autenticado, haga clic derecho -> Propiedades -> [Seguridad de directorios] sobre la carpeta ASM del sitio Web predeterminado en el IIS. Presione **Modificar** y marque la casilla Autenticación de Windows integrada. Haga clic en **Aceptar**. 
-Diríjase a la ruta física en disco, del directorio virtual definido.
-Dele permisos de escritura sobre las carpetas “audit” e “installers” al usuario de IIS asignado, para que el **_Aranda AVS Web Admin_** pueda registrar la información de auditoría, además de generar los instaladores de Agente por Compañía, es necesario que las carpetas “audit” e “installers” de la instalación tenga permisos de escritura.
-Con el **_Aranda AVS Web_ Admin_** instalado, proceda a abrir la aplicación web en un navegador web.
-Si la aplicación web se instaló correctamente, se presentará una página de autenticación, recuerde que el usuario por defecto es “admin” con contraseña “123”, al ingresar tendrá acceso a la administración del sistema.
-Como primer paso diríjase al menú principal (izquierda) a la sección: Licencias -> Instalación Gateway e ingrese el Nombre de la Empresa dueña del Aranda AVS Gateway, por defecto se presenta “Aranda Gateway”, cámbielo si es necesario, guarde los cambios utilizando la opción en la barra de tareas superior.
-Con el nombre de empresa del Aranda AVS Gateway asignado, proceda sobre la misma página a generar un CD Key, con las opciones de la barra de tareas superior.
-Si requiere administrar la configuración de puertos o SSL diríjase a la sección: Configuración -> Gateway y modifique los datos que requiera.
-Con esto ya está completa la instalación del Aranda AVS Web Admin, puede iniciar a crear Proveedores, Empresas y Licencias.
-Al terminar este proceso, ya puede iniciar el Aranda AVS Gateway, diríjase a la consola de servicios del sistema operativo y busque el servicio con nombre: Aranda AVS Gateway, e inícielo.