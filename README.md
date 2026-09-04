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
| **Historia de Usuario** | COMO Solicitante QUIERO consultar una tutoria PARA PODER saber la disponibilidad de ellas para solicitar una que me ayude con mis materias academicas.|

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
| **Historia de Usuario** | COMO Usuario QUIERO Recibir Notificaciones PARA PODER asegurarme de que mi tutoria fue asignada a mi correspondiente tutor para tomar la tutoria.|

## Desglose de trabajo: Épicas, Historias de Usuario y Tareas

La implementación de los requerimientos identificados de TutoECI se desglosa de la siguiente manera:

### 1. Épica:

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-5 |
| **Título** | Recomendar Tutor|
| **Descripción** | Permitir a TutoECI que recomiende los mejores tutores para la asignatura que selecciono el solicitante. |
| **Stakeholder** | Solicitantes y Tutores |

### 2. Historias de usuario:

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-6 |
| **Título** | Auntenticacion del solicitante para obtener tutores recomendados |
| **Descripción** | *Como solicitante, quiero obtener recomendaciones de tutores para dar escoger al mejor y disciplinado que pueda ayudarme a entender la materia.* |
| **Criterios de aceptación** | 1. Dado que el solicitante ingresa a TutoECI con sus credenciales, entonces el sistema le concede acceso y lo redirige a solicitar tutoria.<br>2. Dado que el solicitante ingresa credenciales inválidas, cuando envíe el formulario, entonces el sistema muestra un mensaje de error sin conceder acceso.<br>3. Dado que el solicitante deja campos vacíos, cuando intente iniciar sesión, entonces el sistema le indica qué campos son obligatorios. |
| **Prioridad** | *Alta* |
| **Estimación** | *5 puntos de historia* |

### Tareas

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-7 |
| **Título** | CONECTAR BASE DE DATOS AL SOFTWARE |
| **ID de la Historia de Uso asociada** | SCRUM-13 |
| **Descripción** | *Como desarrollador, quiero conectar la base de datos al software , para poder realizar recomendaciones de tutores.*  |
| **Tareas requisito** | *NINGUNA*|

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-8 |
| **Título** | *RECIBIR DATOS*|
| **ID de la Historia de Uso asociada** | SCRUM-13 |
| **Descripción** | *Como desarrollador, quiero poder recibir datos, para poder realizar consultas de tutores disponibles en mi base de datos.*  |
| **Tareas requisito** | *SCRUM-7* |

| Campo | Descripción |
|------|-------------|
| **ID** | SCRUM-9 |
| **Título** | *CONSULTA BASE DE DATOS*|
| **ID de la Historia de Uso asociada** | SCRUM-13 |
| **Descripción** | *Como desarrollador, quiero poder realizar consultas de tutores, para poder realizar validaciones de datos para la recomendacion.*  |
| **Tareas requisito** | *SCRUM-7* |

## Jira

URL de Jira: https://samuelargalle651-178853109245.atlassian.net/jira/software/projects/SCRUM/boards/1/backlog?atlOrigin=eyJpIjoiNWMzNzFkNjM0MjdlNDA2MWFmNTE5NWIyODEyZWY1OWEiLCJwIjoiaiJ9




