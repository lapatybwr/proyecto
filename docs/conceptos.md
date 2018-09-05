# **Menú File** 
---

Dentro de la aplicación se encuentra la sección del menú File donde se tienen las funciones más importantes del sistema: 

[1. Entries](entries.md)

[2. Applications](#applications)

[3. Application Groups](#application-groups)

[4. Components](#components)

[5. Environments](#environments)

[6. Categories](#categories)

[7. Snapshots](#snapshots)

[8. Disconnect](#disconnect)

[9. Exit ](#exit)


## **Application Groups**
---
Como seguimiento se inicia con crear el ó los grupos de aplicaciones que se usaran en la aplicación.
Un grupo de aplicaciones se usa para asignar aplicaciones a un área de la organización, por ej., la aplicación “PagosApp” y “VentasApp” se asignaría al Grupo “Finanzas”.

El grupo permitirá asociar a un conjunto de aplicaciones en un subgrupo superior permitiendo mantener una estructura organizacional definida.

*Click  File > Application Groups*

![Aplication Group](/img/profundizando/file-application-groups.jpg)


En la siguiente pantalla se podrán crear o eliminar grupos de aplicaciones, en la ventana también se visualizan todos los grupos que han sido creados.

![](/img/profundizando/aplication-group.jpg)

![](/img/profundizando/6-1btn+.jpg) Este botón habilita un nuevo registro en modo edición; permitiendo la captura de un nuevo grupo de aplicaciones.

![](/img/profundizando/6-2btn-.jpg) Este botón elimina el grupo de aplicaciones seleccionado. Confirmación por parte del usuario será solicitada.

!!! Nota
    Una vez creada un grupo de aplicación, se puede relacionar con otro grupo si esto fuera necesario en la columna Parent.


## **Applications**
---

Una aplicación es un conjunto de Componentes que se encuentran dentro de un grupo de aplicación. La aplicación es donde se almacenará la configuración.

*Click  File > Applications*

![imagen aplic](/img/profundizando/file-applications.jpg)

La siguiente pantalla muestra las acciones que se podrán realizar sobre una aplicación.

![acciones aplic](/img/profundizando/crear-applications.jpg)

![btn mas](/img/profundizando/6-1btn+.jpg) Este botón habilita un nuevo registro en modo edición, permitiendo la captura de una nueva aplicación.

![btn menos](/img/profundizando/6-2btn-.jpg) Este botón elimina la aplicación seleccionada. Confirmación por parte del usuario será solicitada

!!! Nota
    Una aplicación puede ser agrupada de manera lógica a través de un “Grupo de Aplicaciones”.


## **Components**
---

Un componente representa una plantilla basada en propiedades que utilizan una entrada de datos de configuración para el almacenamiento de valores. 

*Click  File > Components*

![](/img/profundizando/file-components.jpg)

!!! Nota
    Un componente puede ser generado de manera manual, o provenir de un plug-in.

La siguiente ventana muestra las acciones que se podrán realizar sobre un componente.

![](/img/profundizando/6compon.jpg)


![](/img/profundizando/6-1btn+.jpg) Este botón habilita un registro en modo edición, permitiendo la captura de un nuevo componente.

![](/img/profundizando/6-2btn-.jpg) Este botón elimina el componente seleccionado. Confirmación por parte del usuario será solicitada.

!!! Nota
    Cuando un componente es eliminado, todas las entradas de configuración basados en el componente son eliminadas de manera automática.


Una vez creado el componente se acceder a él  para agregarle sus propiedades. La siguiente pantalla muestra cómo acceder y modificar las propiedades de un componente.

*Right Click  > View Properties*

![](/img/profundizando/7view-proper.jpg)


La siguiente pantalla muestran las propiedades del componente y permite agregar, modificar o eliminar de maneara manual las diferentes propiedades que conforman un componente.

![](/img/profundizando/8tabla.jpg)

![](/img/profundizando/6-1btn+.jpg) Este botón habilita un registro en modo edición, permitiendo la captura de una nueva propiedad.

Una vez que ha sido habilitado un registro se deben considerar los siguientes campos a capturar de las propiedades del componente:

- **Type** (Tipo de dato): Define el tipo de dato a almacenar, se tienen seis tipos de datos, String, Integer, Boolean, DataTime, File y Bean (permite hacer referencia a otro componente)

- **Name**: Es el nombre que representa el campo
Protected: Define si el tipo de dato debe ser enmascarado (Password).

- **Protected**: Al activar esta opción, los datos ingresados se visualizan con asteriscos, suele utilizarse para escribir las contraseñas.

- **Key**: Define si la propiedad será marcada como la llave primaria dentro del componente (Propiedad utilizada por el método de comparación).

!!! Nota
    Para guardar la propiedad editada será necesario presionar la tecla [Enter].


La ventana propiedades del componente contiene funciones que se describen a continuación:

![](/img/profundizando/6-2btn-.jpg) Elimina la propiedad seleccionada. Confirmación por parte del usuario será solicitada

!!! Nota
    Cuando una propiedad es eliminada todas las entradas de configuración del componente son modificadas, eliminando de manera automática los valores asociados a estas propiedades dentro de la entrada de configuración.


![arriba](/img/profundizando/6-2btn-.jpg) Permite modificar el orden de visualización de la propiedad dentro del componente, desplazando la propiedad seleccionada una posición arriba.

![abajo](/img/profundizando/8-2btn-abajo.jpg) Permite modificar el orden de visualización de la propiedad dentro del componente, desplazando la propiedad seleccionada una posición abajo.

![](/img/profundizando/8-3btn-aunlado.jpg) Permite desplazarse a la edición del componente anterior, previo a la selección de un nuevo componente a través de la opción “Componente”.

![home](/img/profundizando/8-4btb-home.jpg) Permite desplazarse a la edición del componente original previo a la selección de un nuevo componente mediante la opción “Componente”.


La siguiente pantalla, la opción enmarcada permite elegir un nuevo componente a editar.  No precisamente lleva el nombre que se muestra, ya que el nombre es de acuerdo con el componente que se tenga en su momento.

![](/img/profundizando/prop-comp.jpg)

***Agregar un “file” como propiedad en un componente***

Esta opción permite asignar el tipo “File” para una propiedad en un componente. Este tipo permite guardar archivos y obtenerlos cada vez que se requiera. Por ejemplo, si quieres guardar un reporte de Excel tendrás que elegir el “type” como “File”. De manera que cuando creas una entrada de configuración puedas guardar un documento XLS en esa propiedad.

![agregar file](/img/profundizando/10agregar-file.jpg)

!!! Nota
    El documento se genera cuando es agrega una entrada al componente.


## **Environments**

---

Un ambiente representa un entorno de trabajo de una “Aplicación”. Toda la entrada de información que sea introducida deberá ser ingresada bajo un ambiente de trabajo para diferenciar la etapa de desarrollo que se lleva a cabo.

*Click  File > Environments*

![Menú Environments](/img/profundizando/file-environments.jpg)

La siguiente ventana muestra los ambientes que se encuentran definidos dentro de la aplicación. Se pueden crear los ambientes que se consideren necesarios.

![](/img/profundizando/12ambientes.jpg)

![](/img/profundizando/6-1btn+.jpg) Este botón habilita un nuevo registro en modo edición, permitiendo la captura de un nuevo ambiente.

![](/img/profundizando/6-2btn-.jpg) Este botón elimina el ambiente seleccionado. Confirmación por parte del usuario será solicitada.

!!! Nota
    Cuando un ambiente es eliminado, todas las entradas de configuración asociados al ambiente son eliminados de manera automática.


## **Categories**
---

Una categoría tiene la función de clasificar entradas de configuración de acuerdo con la prioridad de la configuración. Agrupar varias entradas en una misma categoría facilita la búsqueda y la edición de múltiples entradas de configuración por vez.  También sirve para visualizar las propiedades con códigos de colores de manera que facilite la localización de estas.

!!! Nota
    Definir múltiples categorías es útil para clasificar los cambios. Un cambio de mayor importancia es identificado de manera visual a través de un color distintivo.


*Click  File > Categories*

![Menú categories](/img/profundizando/file-categories.jpg)

La siguiente pantalla muestra las diferentes categorías, donde se pueden agregar, eliminar o modificar las categorías

![](/img/profundizando/14cat.jpg)


Entre las características a destacar se encuentra el color de letra que puede ser asignado a cada una de las categorías.

![](/img/profundizando/6-1btn+.jpg) Este botón habilita un registro en modo edición que permite la captura de una nueva categoría

![](/img/profundizando/6-2btn-.jpg) Este botón elimina la categoría seleccionada. Confirmación por parte del usuario será solicitada.

!!! Nota
    Para guardar la categoría editada será necesario presionar la tecla [Enter]


## **Snapshots**
---


*Click  File > Snapshots*

![Ventana snapshots](/img/profundizando/file-snapshots.jpg)


## **Disconnect**
---

Esta opción permite “cerrar sesión” del usuario actual y se puede volver a ingresar con otro usuario sin necesidad de cerrar la aplicación.

*Click  File > Disconnect*

![menú disconnect](/img/profundizando/file-disconnect.jpg)

## **Exit**
---

Esta opción permite detener y salir completamente de la aplicación.

*Click  File > Exit*

![menpu exit](/img/profundizando/file-exit.jpg)

!!! Nota
    Al cerrar la aplicación desde el icono de “cerrar” la aplicación seguirá abierta en segundo plano.






# **Conceptos de Vesta**

Vesta dispone de terminología y
en esta sección se proporciona una definición sobre cada uno de los componentes principales de la aplicación para brindar un panorama fácil de entender a que se refieren. 

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



