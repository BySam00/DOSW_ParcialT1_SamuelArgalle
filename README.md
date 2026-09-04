# DOSW_ParcialT1_SamuelArgalle

## Diagrama de Contexto
Construya el diagrama de Contexto

![Diagrama de contexto](../images/context.png)

## Lista general de requerimientos 
El sistema TutoECI tiene los siguientes requerimientos:

### Requerimientos Funcionales
El sistema TutoECI debe tener la capacidad de:

1. Los tutores deben poder crear una tutoria 
2. Los solicitantes deben poder consultar las tutorias 
3. Enviar Notificaciones a los solicitantes

### Requerimientos No Funcionales

1. Debe tener la paleta de colores oficial del programa de Ingenieria de Sistemas
2. Debe tener una tipografia legible 

## Diagramas de Caso de Uso
Requerimiento Funcional 1

| Campo | Descripción |
|------|-------------|
| **ID** | RF-01 |
| **Nombre del requerimiento** | Consultar Tutoria |
| **Descripción** | El sistema debe permitir a los soliciantes consultar las tutorias que estan disponibles acerca de las materias que esta cursando o sobre tutorias acerca del prograna academico que esta cursando. |
| **Precondiciones** | Para que el sistema funcione, antes los tutores tienen que tener sus respectivas tutorias asignadas con horario y materia que esta dispuesto a realizar la tutoria al estudiante. |
| **Actor** | Solicitante |
| **Flujo principal** | 1. El solicitante inicia sesión en el sistema con sus credenciales.<br>2. El solicitante selecciona la opción de consultar tutorias.<br>3. El sistema muestra la opcion de la materia que de la que quiere tener tutoria y el respectivo tutor.<br>4. El solicitante elige la acción deseada.<br>5.El sistema ejecuta la acción y actualiza la actividad creada en el sistema.<br>9. El sistema muestra una confirmación de la operación realizada. |
| **Diagrama de caso de uso** | ![Diagrama de caso de uso - Consultar tutoria](../uml/Caso1.png) |
| **Poscondiciones** | Se espera como resultado que la tutoria haya sido consultada y luego solicitada, reflejando que para los tutores se haya actualizado su cronograma.|

Requerimiento Funcional 2 

| Campo | Descripción |
|------|-------------|
| **ID** | RF-02 |
| **Nombre del requerimiento** | Recibir notificaciones |
| **Descripción** | El sistema debe permitir enviar notificaciones a los solicitantes y a los tutores de que la tutoria ya fue asignada. |
| **Precondiciones** | Para que este sistema funcione debe ya haber sido solicitada la tutoria y estar relacionada con la aplicacion NotifyMe para que pueda hacer el proceso de enviar la notificacion. |
| **Actor** | Usuario |
| **Flujo principal** | 1. El solicitante inicia sesión en el sistema con sus credenciales.<br>2. El solicitante selecciona la opción de solicitar tutoria.<br>3. El sistema verifica que exista una tutoria disponible para la materia que solicita.<br>4. Busca su tutoria de preferencia y la selecciona.<br>5. El sistema muestra una confirmación de la asignacion de la tutoria.|
| **Diagrama de caso de uso** | ![Diagrama de caso de uso - Enviar notificacion](../uml/Caso2.png) |
| **Poscondiciones** | Se espera como resultado que la notificacion llegue al usuario de la confirmacion de su asignacion a una tutoria. |




