# **Plug-Ins**
---

Los plugins son componentes adicionales de Vesta que le permiten acceder a un aplicativo y descubrir u obtener automáticamente sus configuraciones.

**VESTA** cuenta con una serie de Plug-ins Oracle WebLogic 11g, y WebLogic 12c que permiten la generación automatizada de componentes, estos “Plug-ins” a su vez están encargados de recuperar las configuraciones de los servidores y almacenarlos en la aplicación en modo de “Entradas”, mismas que son asociadas a una aplicación y a un ambiente en particular.

Ademas se dispone de los Plug-ins Oracle SOA Suite 11g y 12g que permiten la administración de configuraciones de componentes principales.

También cuenta con el Plugin Operating System el cual permite obtener funcionalidades de la configuración del servidor de weblogic.


Es importante mencionar que se debe instalar el plugin de acuerdo con la versión de la base de datos que se tenga instalado, por ejemplo, si se cuenta con Oracle DataBase 11g se debe de instalar el plugin de WebLogic 11g. 

!!! Nota
    Es importante remarcar que se debe tener instalado en el equipo de computo el plugin correspondiente para poder instalarlo en la aplicación. Para esto se debe descargar de la pagina oficial de Oracle.

En esta sección se abordarán los plugins correspondientes a "Weblogic y SOA". Cabe mencionar que la instalación es de forma similar para ambos, solo cambian los nombres de los plugins con sus respectivas nomenclaturas, el procedimientos y los pasos son prácticamente los mismos. Se describirá de manera general haciendo referencia solo mencionando el plugin sin la versión, que correspondería a: Weblogic 11g o Weblogic 12c y SOA 11g o SOA 12c


## **Install WebLogic**
---

Se procede a la instalación del Plugin de WebLogic 

*Click  Plug-Ins > Install> WebLogic > General.*

![1 menú plugin](/img/weblogic/plugins.jpg)

!!! Nota
    El release del Plugin de WebLogic 11g corresponden a las versiones 10.3.x.
    
    El release del Plugin de WebLogic 12c corresponde a las versiones de 12.1 , 12.2.x


En la siguiente pantalla se deberá seleccionar el plug-in a instalar, se solicitará una serie de archivos y directorios requeridos. Para el caso de los plug-ins de WebLogic 11g y WebLogic 12c, los siguientes datos son solicitados:

![2 ventana install weblogic](/img/weblogic/instalar-pluginweb.jpg)

**Browser** Este botón permite seleccionar el archivo .zip que contiene los binarios de instalación.

**Browser** Este botón permite seleccionar el directorio ORACLE_HOME de una instalación local de WebLogic 11g o WebLogic 12c respectivamente.

Al finalizar el proceso de instalación, la aplicación deberá ser reiniciada.

![3 confirmacion para reiniciar](/img/weblogic/3confirmacionreiniciar.jpg)

### **Configuración de Plug-in “WebLogic”**
---

Una vez que el plugin se encuentra instalado en la aplicación, se procede a configurarlo.

*Click  Plug-Ins > Configure*

![4 menú configure](/img/weblogic/plug-conf.jpg)

!!! Nota
    En necesario revisar si el usuario tiene los permisos para configurar el plugin, de lo contrario solo se mostrará la ventana vacia. 

En la siguiente pantalla se deberá seleccionar la “Aplicación y Ambiente” al cual estará asociado el Plug-in “WebLogic 11g”. Es importante conocer que una misma Aplicación” y Ambiente” pueden estar asociados a múltiples plug-ins.

![5 ventana de configuración](/img/weblogic/5ventanaconf.jpg)

En la siguiente pantalla se deberán ingresar los datos de conexión al servidor de dominio “WebLogic 11g”.

![6 datos configuración](/img/weblogic/6datosconf.jpg)

***Servidor:*** IP en donde recibe peticiones el servidor de dominio WebLogic.

***Puerto:*** Puerto en donde recibe peticiones el servidor de dominio WebLogic (Admin Server).

***Usuario:*** Usuario de conexión, este usuario deberá pertenecer al grupo de dominio WebLogic “Administrators”. 

***Password:*** Contraseña del usuario de conexión.

El proceso de conexión al servidor es iniciado, en ese momento las diferentes entradas de configuración en el servidor de dominio “WebLogic” serán descubiertas.

![7 configuracion en proceso](/img/weblogic/7confenproceso.jpg)

#### **Recuperación de la configuración “WebLogic”**
---

En la siguiente pantalla se deberá seleccionar las entradas de configuración a descargar desde el servidor de dominio “WebLogic 11g”.

![8 Config weblogic](/img/weblogic/8Configweblogic.jpg)

***Select All*** Este botón selecciona todas las propiedades del componente de configuración seleccionado.

***Select Suggested*** Este botón selecciona las propiedades del componente de configuración sugeridas por el sistema.

!!! Nota
    Las propiedades sugeridas por el sistema indican los campos necesarios para el proceso de aprovisionamiento de la configuración en el servidor de dominio “WebLogic”.


***Unselect All*** Este botón deselecciona todas las propiedades del componente de configuración seleccionado.

***Set as layout*** Esta opción cuando está habilitada permite guardar las entradas de configuración como plantilla, de manera que para próximas importaciones de otros ambientes se pre-seleccionen las entradas de configuraciones definidas en la plantilla.

***Import*** Este botón realiza la importación de las configuraciones seleccionadas desde WebLogic hacia Vesta.


Una vez seleccionadas las entradas de configuración el proceso de descarga de la configuración es iniciado.

![9 Descarga configuración](/img/weblogic/9Descargaconfiguracion.jpg)

#### **Listar entradas “WebLogic 11g”**

En la siguiente pantalla se muestran las entradas de configuración provenientes de un plug-in, estas entradas son identificadas mediante iconos de color “morado”.

*Click  File > Entries*

![10 ventana entries](/img/weblogic/listas-entries-plugins.jpg)

#### **Opciones sobre entradas en plugins**

Una vez que han sido definidas las entradas de plugins, se cuenta con una serie de opciones a realizar sobre ellas, estas opciones se encuentran en el menú emergente sobre la entrada seleccionada. 


#### **Opciones sobre entradas**
---

Opciones generales

Las siguientes opciones se encuentran descritas en la sección Configuración inicial > [Opciones sobre entradas](/opciones.md)> 

- Acquiere control
- Release control
- View entry
- Duplicate entry
- Promote entry
- Delete entry
- View children
- View History
- Tree History
- Copy Selection
- Copy property
- Compare

##### **Migrate to**

Esta opción permite migrar una configuración de 11g a una configuración de 12c.

*Right click  entry > Migrate to > Version to migrate*

![19 version to migrate](/img/weblogic/19versiontomigrate.jpg)


##### **Push to Server (Individual)**

Esta opción permite enviar la entrada de configuración seleccionada hacia el servidor de dominio “WebLogic” destino. 
Nota: Esta opción solo está disponible para “entradas de configuración” asociadas a plug-ins.

*Right Click  > Push to Server*

![20 menu push to server](/img/weblogic/20menupushtosever.jpg)

!!! Nota
    Confirmación es requerida

![21 ventana push to server](/img/weblogic/21ventanapush.jpg)


**Start** Al presionar este botón el proceso de aprovisionamiento de la configuración es iniciado.

**Close** Este botón es habilitado una vez finaliza el proceso de aprovisionamiento de la configuración.

![22 sincronizacion completa](/img/weblogic/22sincronizacioncompleta.jpg)

Cuando una configuración no pudo ser aprovisionada en el servidor de dominio “WebLogic” manda la siguiente pantalla indicando el inconveniente:

![23 push to server](/img/weblogic/23pushtoserver.jpg)

**RollBack** Este botón es habilitado cuando una configuración no pudo ser aprovisionada en el servidor de dominio “WebLogic” permitiendo así deshacer los cambios en conflicto.


##### **Resolver conflictos**

Esta opción permite resolver conflictos de sincronización entre la configuración almacenada en Vesta y la configuración en el servidor “WebLogic”. Esta opción es útil cuando el envío de la configuración realizada hacia el servidor de dominio “WebLogic” no pudo comprobarse de manera automática por el sistema. Garantizando que la configuración almacenada en Vesta y la configuración del servidor de dominio “WebLogic” es concisa.


!!! Notas 
    Validación manual por parte del usuario dentro del servidor de dominio “WebLogic” es necesaria.
    Esta opción solo está disponible para “entradas de configuración” asociadas a plug-ins.


*Right Click > Resolve Conflicts*

![24 menu resolve conflicts](/img/weblogic/24menuresolveconflicts.jpg)


Al ingresar a “Resolver Conflicts”, muestra en pantalla un mensaje preguntando si está seguro de realizar dicha acción.

![25 confirmar resolver](/img/weblogic/25confirmarresolver.jpg)

**Si** Al presionar este botón el proceso de resolución de la configuración es iniciado.
 

**No** Al presionar este botón el proceso de resolución de la configuración es cancelado.

Resultados: Cuando un conflicto es resuelto, el icono asociado a la entrada de configuración es cambiado de dirección.

![26 resolviendo conflictos](/img/weblogic/26resolviendoconflictos.jpg)

Al termino, muestra el mensaje de que se resolvió el conflicto.

![27 conflicto resuelto](/img/weblogic/27conflictoresuelto.jpg)

##### **Down from Server**

Esta opción permite descargar los cambios de configuración desde el servidor de dominio “WebLogic” hacia la entrada de configuración seleccionada dentro de la aplicación. 

> Nota: Esta opción solo está disponible para “entradas de configuración” asociadas a plug-ins.


*Right Click  > Down from Server*

![28 menu down server](/img/weblogic/28menudownserver.jpg)

Al seleccionar esta opción empieza cargar, una vez terminado, muestra la ventana

![29 ventana down server](/img/weblogic/29ventanadownserver.jpg)

![30 punto](/img/weblogic/30punto.jpg) Esta opción permite aceptar el cambio pendiente desde el servidor de dominio “WebLogic”.

![31 sel categoria](/img/weblogic/31selcategoria.jpg) Esta opción permite la selección de categoría. Es útil cuando se desea identificar un cambio de alta prioridad de manera visual.


!!! Nota
    El historial de cambios sobre las entradas de configuración descargadas será actualizado de manera automática.

La siguiente pantalla muestra el resumen de cambios descargados desde el servidor de dominio “WebLogic” hacia VESTA. Los enlaces situados en la parte superior del cambio permiten la navegación a la entrada de configuración modificada.

![32 resumen de cambios](/img/weblogic/32resumencambios.jpg)

Al presionar los enlaces situados en la parte superior de la entrada de configuración se mostrará la pantalla “visualización de entradas”.

La siguiente pantalla permite visualizar las entradas de configuración descargadas desde el servidor de dominio “WebLogic”.

![33 entries de config descargadas](/img/weblogic/33entriesconfigcargadas.jpg)

##### **Restore default values**

Esta opción establece los valores por default de toda la entrada de configuración, los valores por default son los establecidos por el fabricante del application server.

*Right click entry > Restore default values*

![34 menu restore](/img/weblogic/34restore.jpg)


### Sincronización de Plug-in “WebLogic”
---

El proceso de sincronización es el método mediante el cual las diferentes entradas de configuración almacenadas en VESTA y las configuraciones en el servidor de dominio “WebLogic” son sincronizadas.

!!! Nota
    Esta opción es útil cuando se desea sincronizar más de una entrada de configuración entre el servidor de dominio “WebLogic” y Vesta.

*Click Plug-Ins > Synchronize*

![35 menu syncrinize](/img/weblogic/plug-sincro.jpg)

Al ingresar a la opción de sincronización, muestra la siguiente ventana:

![36 ventana sincro](/img/weblogic/36ventanasincro.jpg)

![37 btn paloma](/img/weblogic/37btnpaloma.jpg) Esta opción selecciona la aplicación y ambiente a sincronizar.

**Push to Server** Al presionar este botón las entradas de configuración almacenados en Vesta son enviadas hacia el servidor de dominio “WebLogic”.

**Down from Server** Al presionar este botón las entradas de configuración almacenados en el servidor de dominio “WebLogic” son descargados hacia Vesta.

### **Push to server**

Esta opción permite enviar de manera selectiva un conjunto de configuraciones almacenadas en Vesta hacia el servidor de dominio “WebLogic”.

![38 pantalla push to server](/img/weblogic/38pantallapushtoserver.jpg)

!!! Nota
    Esta opción es útil cuando se desea enviar un conjunto de configuraciones de manera global.

**Start** Al presionar este botón el proceso de aprovisionamiento de la configuración es iniciado.

**Close** Este botón es habilitado una vez finaliza el proceso de aprovisionamiento de la configuración.

![39 btn cmd](/img/weblogic/39btncmd.jpg)Esta opción permite la visualización del archivo log generado durante el proceso de aprovisionamiento de la configuración.

![40 ventana cmd](/img/weblogic/40ventanacmd.jpg)

#### **Down from server**

Esta opción permite descargar de manera selectiva un conjunto de configuraciones desde el servidor de dominio “WebLogic” hacia Vesta.

![41 down from server](/img/weblogic/41downfromserver.jpg)

!!! Nota
    Esta opción es útil cuando se desea descargar un conjunto de configuraciones de manera global. 

![37 btn paloma](/img/weblogic/37btnpaloma.jpg) Esta opción permite aceptar el cambio pendiente desde el servidor de dominio “WebLogic”.

![31 sel categoria](/img/weblogic/31selcategoria.jpg) Esta opción permite la selección de categoría. Esta opción es útil cuando se desea identificar un cambio de alta prioridad de manera visual.

La siguiente pantalla muestra el resumen de cambios descargados desde el servidor de dominio “WebLogic” hacia Vesta. Los enlaces situados en la parte superior del cambio permiten la navegación a la entrada de configuración modificado.

![42 result sincronización](/img/weblogic/42resultsincronizacion.jpg)

Al presionar los enlaces situados en la parte superior de la entrada de configuración se mostrará la pantalla “visualización de entradas”.

La siguiente pantalla permite visualizar las entradas de configuración descargados desde el servidor de dominio “WebLogic”.

![43 view children](/img/weblogic/43viewchildren.jpg)

## **Auditor**
---


El auditor es la funcionalidad complementaria de los plug-ins de WebLogic 11g y 12c. Dicha funcionalidad es para detectar modificaciones en los ambientes administrados por Vesta , de manera que cuando haya una modificación en alguna configuración de WebLogic ésta sea detectada por Vesta e informe al usuario de dicha actividad en los ambientes.

### **Instalación**
---

Para la instalación se requiere:

- El jar de instalación llamado CustomAuditor.jar proporcionado por Vesta
- Acceso a la consola de WebLogic 
- Acceso al sistema operativo donde está instalado WebLogic
 


### **Auditoria de cambios**
---

 Para instalar el auditor, tienes que iniciar sesión en la consola de WebLogic donde será instalado.
En esta pantalla se deberá seleccionar mediante la opción “Configuration Audit Mode” el modo de auditoria “Audit Changes” 

*Click domain name > Configuration > General > Advance*

![consola](/img/auditor/1consola.jpg)


!! Nota
    El servidor de dominio “Admin Server” será apagado y encendido según se indique en este documento.

La opción “Change Audit” deberá ser seleccionada.

Posteriormente se selecciona la opción “Save” y de ser necesario “Activate changes”

![2 config auditor](/img/auditor/2configauditor.jpg)


!!! Nota
    Para modificar el valor es necesario obtener el lock de la consola en la opción “Lock & Edit” ubicada en la parte superior izquierda en la sección Change Center, solo aplica a dominios instalados en modo Production.

**Apagar AdminServer**

Luego de establecer el valor se procede a apagar el AdminServer

Una vez apagado el Admin Server el archivo “CustomAuditor.jar” deberá ser copiado a la ubicación de domino “MBeans” ubicado en la siguiente ruta:
<WL_HOME>\server\lib\mbeantypes

!!! Nota
    Durante el proceso de copiado de “Custom Auditor” el servidor de dominio “Admin Server” deberá estar apagado 


Por ejemplo:
**D:\Middleware_SOA\Oracle_Home\wlserver\server\lib\mbeantypes**

![3 ruta](/img/auditor/3ruta.jpg)

Se procede a levantar el servidor Admin Server

!!! Nota
    Una vez finalizado el proceso de copiado de “Custom Auditor” el servidor de domino “Admin Server” deberá ser encendido 
  
 
### **Publicación**
---

En la siguiente pantalla se deberá crear un nuevo proveedor de auditoria previendo la siguiente información 
 
!!! Nota
    Si durante el proceso de publicación un mensaje de “validación de esquemas” es mostrado los servidores de dominio “Admin Server y Managed Servers” deberán ser reiniciados 

*Domain name > click Security Realms > Click myrealm*

![4 myrealm](/img/auditor/4myrealm.jpg)

*Providers  > Auditing > Click New*

!!! Nota
    Para modificar el valor es necesario obtener el lock de la consola en la opción “Lock & Edit” ubicada en la parte superior izquierda en la sección Change Center, solo aplica a dominios instalados en modo Production.

![5 new auditor](/img/auditor/5new-auditor.jpg)

- Name : Nombre del Proveedor de Auditoria , por ej.: CustomAuditor

- Type : Tipo de Auditor de cambios , ej. CustomAuditor

- Click  OK

![6 creara nuevo](/img/auditor/6creara-nuevo.jpg)

*Click Auditor name*

![7 clic name](/img/auditor/7clic-name.jpg)

*Configuration > Click Provider Specific*

![8 provide specif](/img/auditor/8provide-specif.jpg)

Enabled : true 

Active Context Handler Entries : ALL 

![9 enable](/img/auditor/9enable.jpg)

Posteriormente se selecciona la opción “Save” y de ser necesario “Activate changes” 
 
!!! Nota
    Una vez finalizado el proceso de publicación el servidor de dominio “Admin Server” y los servidores de dominio “Managed Servers” deberán ser apagados 

### **Configuración Admin Server**

Para que WebLogic informe a Vesta los cambios que ocurren en el ambiente es necesario modificar los parámetros de inicio del servidor de dominio “Admin Server” esto es editando el script “startWebLogic.sh” o “startWebLogic.cmd” ya sea Linux o Windows el sistema operativo donde corre WebLogic.

-Dvesta.server= IP de servidor de dominio principal en VESTA 

-Dvesta.port= Puerto de servidor de dominio principal en VESTA default (7890) 

-Dvesta.id= Identificador de configuración dentro de VESTA 
 
> Nota: El identificador de configuración usado en -Dvesta.id se obtiene en Vesta cuando se elige la opción “Plug-ins > Configure” , una vez configurado un WebLogic con una aplicación y ambiente y se guarda, entonces se genera un Id de configuración mostrado en un popup si la configuración fue exitosa, ese id es el que se asigna en este parámetro. 

D:\Middleware_SOA\Oracle_Home\user_projects\domains\base_domain\startWebLogic.cmd

![10 set path](/img/auditor/10set-path.jpg)

> Nota: Una vez finalizado el proceso de configuración el servidor de dominio “Admin Server” deberá ser reiniciado para que los cambios al script hagan efecto. 

#### **Configuracion managed server**
 
En este paso los parámetros de inicio de los servidores de dominio “Managed Servers” deberán ser modificados 
 
*Click domain name > Servers > Server name > Configuration> Server start > Arguments*

![11 argumentos](/img/auditor/11argumentos.jpg)

!!! Nota
    Una vez finalizado el proceso de configuración los servidores de dominio “Managed Servers” deberán ser reiniciados. 