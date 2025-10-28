### actividad1 
**Objeto: Habitación**

**Concepto**

La Habitación es la unidad fundamental de hospedaje que el hotel ofrece a sus huéspedes. Es un espacio físico con un conjunto de comodidades diseñado para la estadía.

**Atributos (Características)**

numeroHabitacion: Identificador único (String o Entero).
tipo: Clasificación (e.g., Sencilla, Doble, Suite).
precioNoche: Tarifa de hospedaje (Decimal).
estado: Situación operativa (e.g., Limpia, Ocupada, En Mantenimiento).
capacidadMax: Límite de personas (Entero).

**Métodos (Comportamientos)**

cambiarEstado(nuevoEstado): Modifica la situación operativa de la habitación.
consultarDisponibilidad(): Revisa si la habitación está lista para ser asignada.
asignarPrecio(nuevoPrecio): Actualiza el costo de la tarifa por noche.
realizarServicioDeLimpieza(): Inicia el proceso de limpieza y actualiza el estado a 'Limpia'.

-----
**Objeto: Huésped**

**Concepto**

La persona que se hospeda en el hotel y hace uso de sus servicios. Es el cliente principal del negocio.

**Atributos (Características)**

identificacion: Identificador único (String).
nombreCompleto: Nombre completo del huésped (String).
telefono: Número de contacto (String).
email: Correo electrónico (String).
historialReservas: Registro de reservas anteriores (Lista).
puntosFidelidad: Puntuación acumulada (Int).

**Métodos (Comportamientos)**

registrarCheckIn(): Proceso de registro de llegada.
realizarCheckOut(): Proceso de registro de salida.
actualizarContacto(nuevoEmail): Modifica la información de contacto.
solicitarServicio(servicio): Petición de un servicio del hotel.
acumularPuntos(monto): Incrementa los puntos de fidelidad según el gasto.

----
**Objeto: Empleado**

**Concepto**

Un miembro del personal del hotel que realiza tareas específicas para garantizar el funcionamiento del servicio (e.g., Recepcionista, Chef, Camarero, Gerente).

**Atributos (Características)**

idEmpleado: Identificador único del empleado (Int).
nombre: Nombre del empleado (String).
cargo: Puesto o rol dentro del hotel (String).
salario: Remuneración mensual (Decimal).
fechaContratacion: Día en que comenzó a trabajar (Date).
departamento: Área de trabajo (String).

**Métodos (Comportamientos)**

marcarEntrada(): Registra el inicio de la jornada laboral.
marcarSalida(): Registra la finalización de la jornada laboral.
asignarTarea(tarea): Se le encomienda una tarea específica.
atenderCliente(huésped): Proporciona asistencia o servicio a un huésped.
solicitarVacaciones(): Proceso para pedir días de descanso.

----

**Objeto: Servicio Extra**

**Concepto**

Cualquier prestación que el hotel ofrece fuera del hospedaje básico, como restaurante, spa o gimnasio, y que puede generar un cargo extra.

**Atributos (Características)**

nombreServicio: Identificación del servicio (String: Spa, Cena, Minibar, SalaConferencia).
costo: Precio del servicio (Decimal).
estaDisponible: Indica si el servicio se puede utilizar actualmente (Boolean).
ubicacion: Lugar físico donde se presta el servicio (String).

**Métodos (Comportamientos)**

añadirACuentaHuesped(huésped, cantidad): Registra el costo del servicio al saldo del huésped.
consultarCosto(): Devuelve el valor actual del servicio.
reservarServicio(hora): Agenda el uso del servicio a una hora específica.
actualizarDisponibilidad(estado): Cambia el estado de estaDisponible.

----

**Objeto 1: Habitación**

**Concepto**

La unidad fundamental de hospedaje que el hotel ofrece a sus huéspedes. Es un espacio físico con un conjunto de comodidades.

**Atributos (Características)**

numeroHabitacion: Identificador único (String/Int).
tipo: Clasificación (String: Sencilla, Doble, Suite).
precioNoche: Tarifa de hospedaje (Decimal).
estado: Situación operativa (String: Limpia, Ocupada, En Mantenimiento).
capacidadMax: Límite de personas (Int).

**Métodos (Comportamientos)**

cambiarEstado(nuevoEstado): Modifica la situación operativa de la habitación.
consultarDisponibilidad(): Revisa si la habitación está lista para ser asignada.
asignarPrecio(nuevoPrecio): Actualiza el costo de la tarifa por noche.
realizarServicioDeLimpieza(): Inicia el proceso de limpieza y actualiza el estado a 'Limpia'.

**Objeto 2: Huésped**

**Concepto**

La persona que se hospeda en el hotel y hace uso de sus servicios. Es el cliente principal del negocio.

**Atributos (Características)**

identificacion: Identificador único (String).
nombreCompleto: Nombre completo del huésped (String).
telefono: Número de contacto (String).
email: Correo electrónico (String).
historialReservas: Registro de reservas anteriores (Lista).
puntosFidelidad: Puntuación acumulada (Int).

**Métodos (Comportamientos)**

registrarCheckIn(): Proceso de registro de llegada.
realizarCheckOut(): Proceso de registro de salida.
actualizarContacto(nuevoEmail): Modifica la información de contacto.
solicitarServicio(servicio): Petición de un servicio del hotel.
acumularPuntos(monto): Incrementa los puntos de fidelidad según el gasto.

**Objeto 3: Empleado**

**Concepto**

Un miembro del personal del hotel que realiza tareas específicas para garantizar el funcionamiento del servicio (e.g., Recepcionista, Chef, Camarero, Gerente).

**Atributos (Características)**

idEmpleado: Identificador único del empleado (Int).
nombre: Nombre del empleado (String).
cargo: Puesto o rol dentro del hotel (String).
salario: Remuneración mensual (Decimal).
fechaContratacion: Día en que comenzó a trabajar (Date).
departamento: Área de trabajo (String).

**Métodos (Comportamientos)**

marcarEntrada(): Registra el inicio de la jornada laboral.
marcarSalida(): Registra la finalización de la jornada laboral.
asignarTarea(tarea): Se le encomienda una tarea específica.
atenderCliente(huésped): Proporciona asistencia o servicio a un huésped.
solicitarVacaciones(): Proceso para pedir días de descanso.

**Objeto 4: Servicio Adicional**

**Concepto**

Cualquier prestación que el hotel ofrece fuera del hospedaje básico, como restaurante, spa o gimnasio, y que puede generar un cargo extra.

**Atributos (Características)**

nombreServicio: Identificación del servicio (String: Spa, Cena, Minibar, SalaConferencia).
costo: Precio del servicio (Decimal).
estaDisponible: Indica si el servicio se puede utilizar actualmente (Boolean).
ubicacion: Lugar físico donde se presta el servicio (String).

**Métodos (Comportamientos)**

añadirACuentaHuesped(huésped, cantidad): Registra el costo del servicio al saldo del huésped.
consultarCosto(): Devuelve el valor actual del servicio.
reservarServicio(hora): Agenda el uso del servicio a una hora específica.
actualizarDisponibilidad(estado): Cambia el estado de estaDisponible.

**Objeto 5: Factura **

**Concepto**

El documento contable que detalla todos los cargos generados por un huésped durante su estancia.

**Atributos (Características)**

numeroFactura: Identificador único (Int).
fechaEmision: Día de la generación (Date).
huéspedAsociado: Objeto Huésped al que se le cobra.
detalleCargos: Listado de items consumidos (Lista).
totalPagar: Suma final de todos los cargos (Decimal).
estadoPago: Situación actual de la factura (String: Pendiente, Pagada).

**Métodos (Comportamientos)**

calcularTotal(): Realiza la suma de todos los detalleCargos.
agregarCargo(servicio, monto): Añade un ítem a la lista de cargos.
procesarPago(metodo): Registra la transacción de pago.
imprimirFactura(): Genera una versión física o digital del documento.


