# Propuesta TP DSW

## Grupo
### Integrantes
* 50672 Martin Pilaszek
* 50336 Lazaro Cerquetti
* 51732 Thiago Pipero
* 48784 Bruno Cussitt

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)
*Nota*: si utiliza un monorepo indicar un solo link con fullstack app.

## Tema
### Descripción
Aplicacion para gestion de reservas en un estacionamiento. Comprende la alta de usuarios, gestion de playas de estacionamientos, reservas, tarifas, clientes y pagos.

### Modelo
![imagen del modelo]()

## Alcance Funcional 

### Alcance Mínimo

|Req|Detalle|
|:-|:-|
| CRUD Simple | 1. CRUD Usuario<br/>2. CRUD Cliente<br/>3. CRUD TipoVehiculo<br/>4. CRUD TipoEstadia<br/>5. CRUD Playa |
| CRUD Dependiente | 1. CRUD Cochera depende de Playa<br/>2. CRUD Pago depende de Reserva<br/>3. CRUD Tarifa depende de TipoVehiculo y TipoEstadia<br/>4. CRUD Reserva depende de Cliente, Cochera, TipoVehiculo y TipoEstadia |
| Listado + detalle | 1. Listado de cochera por playa<br/>2. Listado de reservas<br/>3. Listado de clientes |
| CUU/Epic | 1. Crear una reserva: valida disponibilidad de cochera, calcula precio según tarifa y asocia cliente existente o nuevo<br/>2. Finalizar una reserva: libera cochera y registra el pago<br/>3. Cancelar una reserva |


Adicionales para Aprobación
| Req | Detalle |
|:-|:-|
| Funcionalidad adicional | 1. Registrar pago de una reserva<br>2. Validar solapamiento de reservas por cochera<br>3. Gestión de estado de reserva (pendiente, activa, finalizada, cancelada) |


### Alcance Adicional Voluntario

| Req | Detalle |
|:-|:-|
| Listados | 1. Listado de cocheras disponibles por fecha<br>2. Reporte de ingresos por día<br>3. Filtro de reservas por estado<br>4. Historial de reservas por cliente |
| CUU / Epic | 1. Modificación de una reserva (reprogramación de fechas)<br>2. Reasignación de cochera |
| Otros | 1. Exportación de reportes (CSV o PDF)<br>2. Notificación simple de reservas (opcional) |

