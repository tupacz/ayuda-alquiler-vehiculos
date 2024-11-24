# Guía de Mantenimiento del Sistema de Alquiler de Vehículos

## 1. Introducción

La Guía de Mantenimiento del Sistema de Alquiler de Vehículos está destinada a asegurar la operatividad continua del sistema, proporcionando procedimientos detallados para la conservación, prevención de fallas y restauración del sistema en caso de inconvenientes. Esta guía está orientada a los encargados del mantenimiento de la infraestructura tecnológica y personal técnico que asegura la disponibilidad del sistema.

Se enfoca en las siguientes áreas:

- Mantenimiento preventivo y correctivo del sistema.
- Respaldo y restauración de datos.
- Actualizaciones del sistema.

---

## 2. Mantenimiento Preventivo y Correctivo

### 2.1 Mantenimiento Preventivo

**Tareas Recomendadas**:
- **Actualizaciones**: Mantener el sistema operativo y los drivers actualizados para asegurar la compatibilidad y seguridad.
- **Reinicios Programados**: Programar el reinicio del servidor al menos una vez al mes para liberar recursos y evitar problemas de rendimiento.
- **Pruebas de Rendimiento**: Ejecutar pruebas de rendimiento cada tres meses para detectar posibles problemas y asegurar la eficiencia del sistema.
- **Verificación de Componentes**: Verificar periódicamente los componentes de hardware, como discos y memoria, para evitar fallos inesperados.

### 2.2 Mantenimiento Correctivo

**Descripción**: El mantenimiento correctivo se lleva a cabo cuando se presentan fallas inesperadas en el sistema.

**Pasos Generales para el Mantenimiento Correctivo**:

1. **Identificar la Falla**: Utilizar el **Visor de Eventos de Windows** y el **Monitor de Recursos** para identificar la causa del problema.
2. **Diagnosticar la Causa**: Revisar los registros de eventos para determinar si el problema está relacionado con recursos insuficientes, fallos de hardware, o errores de software.
3. **Aplicar Soluciones**: Dependiendo del diagnóstico, aplicar la solución adecuada, que puede incluir:
   - **Reinicio del servidor**.
   - **Actualización de componentes de software**.
   - **Sustitución de componentes de hardware defectuosos**.
4. **Verificar el Resultado**: Asegurarse de que la solución aplicada haya resuelto el problema y que el sistema esté funcionando correctamente.

---

## 3. Respaldo y Restauración de Datos

### 3.1 Respaldo de la Base de Datos

**Frecuencia**: Los respaldos de la base de datos deben realizarse diariamente, preferentemente en horarios nocturnos para evitar afectar la operatividad del sistema.

**Pasos para realizar un respaldo**:

1. **Acceder al Menú de Administración**: En el menú principal, ir a **Administración** → **Respaldo de Bases**.
2. **Seleccionar Respaldar Base de Datos**: Haz clic en el botón **Respaldar Base de Datos**.
3. **Seleccionar Ubicación del Respaldo**: Se abrirá una ventana para seleccionar la carpeta donde se desea guardar el archivo de respaldo.
4. **Iniciar Respaldo**: Una vez seleccionada la carpeta, el sistema ejecutará el comando SQL para crear el archivo de respaldo.

**Consideraciones Importantes**:
- Los respaldos deben almacenarse en una ubicación segura y también contar con una copia externa (offline o en la nube).

### 3.2 Restauración de la Base de Datos

**Situaciones Comunes para Restaurar un Respaldo**:
- **Falla del Sistema**: Cuando se presenta una falla crítica que afecta la operatividad del sistema.
- **Pérdida de Datos**: Cuando se detecta la pérdida de datos importantes y se necesita restaurar a un estado previo.

**Pasos para restaurar un respaldo**:

1. **Acceder al Menú de Administración**: En el menú principal, ir a **Administración** → **Respaldo de Bases**.
2. **Seleccionar Restaurar Base de Datos**: Haz clic en el botón **Restaurar Base de Datos**.
3. **Seleccionar Archivo de Respaldo**: Se abrirá una ventana para seleccionar el archivo de respaldo que se desea restaurar.
4. **Iniciar Restauración**: Una vez seleccionado el archivo, el sistema ejecutará el comando SQL para restaurar la base de datos utilizando el archivo seleccionado.

**Consideraciones Importantes**:
- Realizar pruebas de restauración periódicas para asegurarse de que los respaldos sean válidos y puedan ser utilizados en caso de emergencia.

---

## 4. Actualizaciones del Sistema

### 4.1 Aplicar Actualizaciones

**Descripción**: Las actualizaciones del sistema son esenciales para mejorar la seguridad, corregir errores y añadir nuevas funcionalidades. Estas deben planificarse de manera que impacten lo menos posible la operatividad del sistema.

**Pasos para aplicar una actualización**:

1. **Descargar Actualización**: Descarga el paquete de actualización desde el sitio seguro del proveedor.
2. **Ejecutar Instalador de Actualización**: Ejecuta el instalador y sigue las instrucciones para aplicar la actualización.
3. **Verificar la Instalación**: Una vez completada la actualización, verifica que todos los componentes del sistema funcionen correctamente.
4. **Documentar los Cambios**: Registra las actualizaciones aplicadas, incluyendo la fecha y la versión, para tener un historial completo.

**Consideraciones**:
- Siempre realizar un respaldo completo de la base de datos antes de aplicar cualquier actualización.

---

## 5. Solución de Problemas Frecuentes

### 5.1 Problemas de Rendimiento

**Causa Común**: Alto uso de recursos, como CPU o memoria, debido a procesos intensivos o falta de mantenimiento preventivo.

**Solución**:
- **Liberar Recursos**: Reiniciar el servidor para liberar recursos.
- **Optimización**: Identificar procesos que consuman más recursos y buscar optimizaciones en el código o configuración.

### 5.2 Problemas de Conectividad

**Causa Común**: Fallos en la comunicación con el servidor SQL Server.

**Solución**:
- **Verificar Conexión**: Comprobar la configuración del **connection string** y asegurarse de que el servidor SQL esté operativo.
- **Reiniciar Servicios**: En caso necesario, reiniciar el servicio de SQL Server.
