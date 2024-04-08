# Propuesta TP DSW

## Grupo
### Integrantes
48952- Franco Natalia Belen
49082- Abele Federico
50194 - Zallocco Emilio


### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)
*Nota*: si utiliza un monorepo indicar un solo link con fullstack app.

## Tema
### Descripción
Proponemos elaborar una página para solicitar y reservar turnos médicos en la cual se van a poder registrar todos los doctores que atiendan con sus respectivos horarios de consulta y cargar todos los pacientes para así también registrarlos en el calendario.

### Modelo
![imagen del modelo]()

*Nota*: incluir un link con la imagen de un modelo, puede ser modelo de dominio, diagrama de clases, DER. Si lo prefieren pueden utilizar diagramas con [Mermaid](https://mermaid.js.org) en lugar de imágenes.

## Alcance Funcional 

### Alcance Mínimo

*Nota*: el siguiente es un ejemplo para un grupo de 3 integrantes para un sistema de hotel. El 

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Tipo Paciente<br>2. CRUD Medico<br>3. CRUD Paciente|
|CRUD dependiente|1. CRUD ObraSocial{depende de} CRUD Medico<br>2. CRUD Horarios {depende de} CRUD Medico |
|Listado<br>+<br>detalle| 1. Listado de habitaciones filtrado por tipo de habitación, muestra nro y tipo de habitación => detalle CRUD Habitacion<br> 2. Listado de reservas filtrado por rango de fecha, muestra nro de habitación, fecha inicio y fin estadía, estado y nombre del cliente => detalle muestra datos completos de la reserva y del cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Tipo Paciente<br>2. CRUD tipoConsulta<br>3. CRUD ObraSocial{depende de} CRUD Medico<br>4. CRUD Medico<br>5. CRUD Horarios {depende de} CRUD Medico<br>6. CRUD Turno<br>|
|CUU/Epic|1.Reservar turno para un determinado medico<br>2. Cancelar Turno<br>3. Consultar horario del turno con mail o dni|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|

