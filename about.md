# **Conceptos de Vesta**

Esta sección se da una definición sobre cada uno de estos componentes principales para proporcionar un panorama mas fácil de entender sobre lo que son, lo que hacen y cómo funcionan juntos. 

## **Conceptos Básicos**
---
 
- [Vesta](#vesta)
- [Propiedades](#propiedades)
- [Entradas o Entries](#entradas-o-entries)
- [Entradas de configuración](#entradas-de-configuracion)
- [Components](#components)
- [Application](#application)
- [Profile](#profile)
- [Permisions](#permisions)
- [Perfil de Usuario](#perfil-de-usuario)
- [Application Group](#application-group)
- [Environments](#environments)
- [Categories](#categories)
- [Plugin](#plugin)
- [Logs](#log)
 
---

###**Vesta**
Nombre del programa. En el documento se refiera a Vesta como una aplicación. Es un programa que le permite al administrador de sistemas tener el control, la gestión y la configuración de toda la infraestructura y aplicaciones que son utilizadas en la organización.

###**Propiedades**
Se refieren a las características del *componente*, una propiedad es cada campo (*entrada*) o valor que es ingresado al *componente*.  

###**Entradas o Entries**
Se refiere al ingreso de información (configuraciones) al componente, esta información representa la configuración que tiene un equipo de cómputo, un servidor, clúster, sistema o alguna configuración de cierto componente y que este haya tenido mas de una configuración y sea necesario guardar el historial de las misas.

###**Entradas de configuración** 
Se refiere a la información que fue ingresada y se encuentra contenida en los componentes que se ingresaron sobre un ambiente de trabajo.

###**Components** 
Es una plantilla o tabla que contiene las propiedades (características) que utiliza una entrada de configuración para el almacenamiento de valores. 

###**Application**
Una aplicación es un sistema, representa a un conjunto de Componentes (elementos que componen al sistema) donde se almacena la configuración de los recursos informáticos. 

###**Profile**
Un perfil es una agrupación de permisos con funcionalidades específicas dentro de la aplicación y que es asignado a un usuario.

###**Permisions**
Los permisos son una lista de accesos con todas las funcionalidades que tiene la aplicación Vesta, estos permisos son otorgados a los perfiles para que estos sean asignados a los usuarios.

###**Perfil de Usuario**
Es cuando a un usuario le fue asignado un determinado perfil para realizar sus actividades.

###**Applications Groups**
Es el nombre que se le da a un conjunto de aplicaciones que son asignadas a un área en específico de la organización, por ej., la aplicación “PagosApp” y “VentasApp” se asignaría al Grupo “Finanzas”.

###**Environments** 
Los ambientes se refieren a los entornos de trabajo sobre los cuales se trabaja en el proyecto en ese momento.

###**Categories** 
Una categoría es asignada a algunas entradas de configuración con el fin de clasificar su prioridad e identificarlas más rápidamente de las otras de acuerdo con el color que representa.


###**Plugin** 
Es un complemento de software que añade una funcionalidad adicional y específica a un programa que le permitirá un mejor funcionamiento. Los plugins en Vesta son las configuraciones adicionales los cuales permitirán obtener automáticamente funcionalidades especificas.

###**Log**


## **Simbología**
---

Vesta dispone de símbolos, imágenes o iconos los cuales representan cierto elemento o situación en la que se encuentra en la aplicación.

![]() Icono de la aplicación Vesta.

![]() La imagen con el signo **+** en cualquier parte de la aplicación, permite agregar un elemento dependiendo de donde se encuentre ubicado dentro de la aplicación, por ejemplo, si se encuentra en componentes, habilitara la línea para crear un nuevo componente.

![]() Permite eliminar un elemento, dependiendo de donde se encuentre ubicado.

![]() Permite guardar los cambios realizadas en la pantalla que se presenta en ese momento.

![]() Ubicado en el menú Plugins/Install, este icono en color azul significa que aun no se ha instalado el plugin.

![]() Ubicado en el menú Plugins/Install, este icono verde con la palomita indica que ya fue instalado el plugin

![]() Modifica el orden de visualización de la propiedad dentro del componente, desplazando la propiedad seleccionada una posición arriba.

![]() Modifica el orden de visualización de la propiedad dentro del componente, desplazando la propiedad seleccionada una posición abajo.

![]() Permite desplazarse a la edición del componente anterior, previo a la selección de un nuevo componente a través de la opción “Componente”.

![]() Permite desplazarse a la edición del componente original previo a la selección de un nuevo componente mediante la opción Componente

![]()  Representa una aplicación

![]() Representa un grupo de aplicaciones.

![]() Permite actualizar los valores en la ventana de entradas (entries)

![]() Representa un ambiente.

![]()

![]() Representa un componente creado manualmente por el usuario.

![]()

![]() Representa un componente creado mediante un weblogic.


![]() Representa un componente que aún no contiene entradas.

![]() Dependiendo donde se encuentre ubicado: si se encuentra dentro de una plantilla del componente, este representa que fue asociado con otro componente externo, al componente asociado se le llama Children

![]()

![]() Representa las entradas en los componentes de forma visula sin realizar cambios sobre ellas.

![]() Representa las entradas de los componentes, una vez que se ha adquirido el control sobre ellas para realizar algún tipo de configuración.

![]()

![]()

![]()


![]() Este icono indica que el servidor WebLogic requiere reinicio para que el cambio tenga efecto. 

![]() Si el icono se encuentra sobre un ambiente significa que tiene bloqueadas las notificaciones.

![]() Este botón permite asignar el valor default de la propiedad.

![]() Esta opción permite la visualización del archivo log generado durante el proceso de aprovisionamiento de la configuración.

![]() Sincronización 

![]() Este icono representa que un ambiente ha sido bloqueado….

![]() Esta opción cuando está habilitada permite guardar las entradas de configuración como plantilla


![]() Al seleccionar esa opción permite elegir un elemento contenido en la lista.
 
![]()

![]()

![]()

![]()