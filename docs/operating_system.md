# Plugin Operating System
 
Vesta cuenta con el Plugin Operating System que permite obtener funcionalidades de la configuración del servidor de weblogic.

Cualquier tipo de modificación que sea realizada en los archivos de configuración será interpretada por el plugin y enviará a la aplicación Vesta una notificación indicando que se realizo dicha acción y será implementado.


*Click  Plug-Ins > Install> Operating System*

![](img/weblogic/os/install-os.jpg)


Se procede a la instalación del Plugin Operating System ubicando el archivo requerido:

![](img/weblogic/os/select-plugin-os.jpg)

**Browser** Este botón permite seleccionar el archivo .zip que contiene los binarios de instalación.

Al finalizar el proceso de instalación, la aplicación deberá ser reiniciada.

![](img/weblogic/os/os-instalado.jpg)

## **Configuración de Plug-in “Operating System”**
---

Una vez que el plugin se encuentra instalado en la aplicación, se procede a configurarlo.

*Click  Plug-Ins > Configure*

![4 menú configure](/img/weblogic/os/config-os.jpg)


En la siguiente pantalla se deberá seleccionar la “Aplicación y Ambiente” al cual estará asociado el Plug-in “Operating System”. Es importante conocer que una misma Aplicación” y Ambiente” pueden estar asociados a múltiples plug-ins.


![](/img/weblogic/os/config-ops.jpg)

Una vez que se tiene elegida la aplicación y el ambiente con el plugin OS, se procede a acceder a la ventana de configuración:

![](/img/weblogic/os/ventana-config.jpg)

***Username***: Es el usuario hacia una conexion de un servidor de aplicacion con sftp

***Password*** Corresponde al password del usuario con la conexión al servidor.


***Host***: Corresponde al host del servidor sftp.

***Port***: Puerto correspondiente al servidor sftp.


Una vez que fueron introducidos los datos del servidor, se procede a realizar la conexión con el botón **Connect** para establecer la conexión con el servidor
Con la conexión establecida se procede a seleccionar el archivo

![](/img/weblogic/os/select-file-os.jpg)

***Select Files***. Permite elegir el archivo del servidor.

***Update*** Una vez seleccionado un archivo, permite hacer de archivo.

***View***. Permite visualizar el contenido del archivo seleccionado.

***Delete***. Permite eliminar el archivo seleccionado.

En la sección de *Refresh Interval* se introduce el tiempo en segundos establecido para que cada cierto tiempo se tenga que validar automáticamente el archivo seleccionado.

![](/img/weblogic/os/refresh-os.jpg)

***Import***. Una vez que se tienen establecidos los parámetros se procede a importarlo a la aplicación.

***Cancel***. Permite cancelar la conexión y los cambios realizados.

