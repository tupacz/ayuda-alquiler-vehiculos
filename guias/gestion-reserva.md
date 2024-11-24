## Gestión de Reservas

- [Crear Nueva Reserva](#crear-nueva-reserva)
- [Modificar Reserva](#modificar-reserva)
- [Cancelar Reserva](#cancelar-reserva)
- [Preparar Vehículos para Alquiler](#preparar-vehículos-para-alquiler)

--- 


### Crear Nueva Reserva

**Acceso**: Esta funcionalidad está disponible para los recepcionistas.

**Ubicación en el Menú**:  
- Ir a **Reservas** → **Gestión de Reservas** → **Nueva Reserva**.

**Pasos para crear una reserva**:

1. **Seleccionar Vehículo**:  
   - Selecciona la **Fecha de Retiro** y la **Fecha de Devolución**.
   - Haz clic en **Buscar**. El sistema listará todos los vehículos disponibles para ese rango de fechas.
   - Selecciona un vehículo del listado y haz clic en **Seleccionar**. El precio total se actualizará de acuerdo al vehículo y las fechas elegidas.

   ![Captura de pantalla - Alta de Reserva](/assets/alta-de-reserva.png)

2. **Seleccionar Seguro**:  
   - Selecciona la preferencia del cliente haciendo clic en uno de los **botones de opción (radio button)** disponibles.

3. **Buscar Cliente**:  
   - Haz clic en **Buscar Cliente**. Se abrirá un pop-up con un listado de clientes disponibles.
   - Si el cliente no está en la base de datos, puedes dar de alta al cliente directamente desde este pop-up.

4. **Crear Reserva**:  
   - Una vez seleccionados el vehículo y el cliente, haz clic en **Crear Reserva** para generar la reserva.

**Validaciones Importantes**:
- No podrás hacer clic en **Crear Reserva** si no has seleccionado un vehículo y un cliente.

---

### Modificar Reserva

**Acceso**: Esta funcionalidad está disponible para los recepcionistas.

**Ubicación en el Menú**:  
- Ir a **Reservas** → **Gestión de Reservas** → **Modificar Reserva**.

**Pasos para modificar una reserva**:

1. **Seleccionar Reserva**:  
   - Aparecerá un listado de reservas existentes. Selecciona la reserva que deseas modificar.

2. **Modificar Detalles**:  
   - Puedes modificar detalles como las fechas de retiro y devolución o cambiar el vehículo, siempre y cuando esté disponible.

3. **Guardar Cambios**:  
   - Haz clic en **Guardar Cambios** para confirmar la modificación.

**Validaciones Importantes**:
- Solo se pueden modificar reservas que no hayan comenzado o que no estén en estado de cancelación.

---

### Cancelar Reserva

**Acceso**: Esta funcionalidad está disponible para los supervisores y gerentes de atención al cliente.

**Ubicación en el Menú**:  
- Ir a **Reservas** → **Gestión de Reservas** → **Cancelar Reserva**.

**Pasos para cancelar una reserva**:

1. **Seleccionar Reserva**:  
   - En la pantalla aparecerá un listado de todas las reservas en estado **Pendiente**.
   - Selecciona la reserva que deseas cancelar.

2. **Motivo de Cancelación**:  
   - Escribe el motivo de la cancelación en el campo **Motivo de Cancelación**.

3. **Cancelar Reserva**:  
   - Haz clic en **Cancelar Reserva** para confirmar la cancelación.

**Validaciones Importantes**:
- No podrás cancelar la reserva si no has proporcionado un motivo de cancelación.

---

### Preparar Vehículos para Alquiler

**Acceso**: Esta funcionalidad está disponible para los empleados del taller.

**Ubicación en el Menú**:  
- Ir a **Reservas** → **Gestión de Mantenimiento** → **Vehículos en Reserva**.

**Pasos para preparar un vehículo**:

1. **Seleccionar Vehículo**:  
   - El sistema mostrará un listado con todos los vehículos que están en reserva y necesitan preparación.
   - Selecciona el vehículo que deseas preparar.

2. **Realizar Tareas de Preparación**:  
   - El sistema mostrará una lista de tareas que deben completarse (e.g., limpiar exterior, limpiar interior, inflar ruedas).
   - Marca cada tarea como completada una vez realizada.

3. **Finalizar Preparación**:  
   - Cuando todas las tareas estén marcadas, el botón **Service Realizado** se habilitará. Haz clic para finalizar la preparación y marcar la reserva como **Lista**.

**Validaciones Importantes**:
- No podrás marcar el servicio como realizado hasta que todas las tareas hayan sido completadas.