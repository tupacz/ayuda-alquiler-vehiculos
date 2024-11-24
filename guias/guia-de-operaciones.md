# Guía de Operación del Sistema de Alquiler de Vehículos

## Índice
1. [Introducción](#1-introducción)
2. [Configuración del Entorno del Sistema](#2-configuración-del-entorno-del-sistema)
   - [Requisitos del Sistema](#21-requisitos-del-sistema)
   - [Instalación del Sistema](#22-instalación-del-sistema)
3. [Manejo de Usuarios y Permisos](#3-manejo-de-usuarios-y-permisos)
   - [Creación de Usuarios](#31-creación-de-usuarios)
   - [Gestión de Permisos](#32-gestión-de-permisos)
4. [Monitoreo y Mantenimiento del Sistema](#4-monitoreo-y-mantenimiento-del-sistema)
   - [Monitoreo del Sistema](#41-monitoreo-del-sistema)
   - [Mantenimiento Preventivo](#42-mantenimiento-preventivo)
5. [Respaldo y Restauración de Datos](#5-respaldo-y-restauración-de-datos)
   - [Respaldo de la Base de Datos](#51-respaldo-de-la-base-de-datos)
   - [Restauración de la Base de Datos](#52-restauración-de-la-base-de-datos)
6. [Actualizaciones del Sistema](#6-actualizaciones-del-sistema)
   - [Aplicar Actualizaciones](#61-aplicar-actualizaciones)
7. [Solución de Problemas Comunes](#7-solución-de-problemas-comunes)
   - [Problemas de Conexión](#71-problemas-de-conexión)
   - [Problemas de Rendimiento](#72-problemas-de-rendimiento)

## 1. Introducción

La Guía de Operación del Sistema de Alquiler de Vehículos está diseñada para proporcionar instrucciones sobre la administración y operación técnica del sistema. A diferencia de la Guía del Usuario, este documento se enfoca en el mantenimiento operativo del sistema, asegurando su disponibilidad y buen funcionamiento, así como la gestión de respaldos y configuraciones.

Esta guía está destinada a administradores del sistema y personal de soporte técnico. Se abordan los siguientes aspectos:

- Configuración del entorno del sistema.
- Manejo de usuarios y permisos.
- Monitoreo y mantenimiento del sistema.
- Respaldo y restauración de datos.

---

## 2. Configuración del Entorno del Sistema

### 2.1 Requisitos del Sistema

**Hardware**:
- Servidor con un procesador de al menos 2.0 GHz, 8 GB de RAM y 100 GB de espacio en disco.

**Software**:
- Sistema Operativo: Windows Server 2016 o superior.
- Base de Datos: SQL Server 2019.
- Framework: .NET Framework 4.8.
- Cliente: Windows 10 o superior para acceso a la interfaz de usuario.

### 2.2 Instalación del Sistema

**Pasos para la Instalación**:

1. **Descargar Instalador**: Accede al instalador del sistema desde el servidor de la empresa o una ubicación segura.
2. **Ejecutar Instalador**: Ejecuta el archivo de instalación y sigue las instrucciones en pantalla.
3. **Configuración Inicial**:
   - Define la ubicación de la base de datos.
   - Configura el **connection string** con los datos del servidor SQL Server.
4. **Verificar Componentes Necesarios**: Asegúrate de que todos los componentes necesarios (frameworks, drivers) estén instalados.

---

## 3. Manejo de Usuarios y Permisos

### 3.1 Creación de Usuarios

**Acceso**: Solo disponible para administradores del sistema.

**Pasos para crear un usuario**:

1. **Acceder a la Gestión de Usuarios**: Ir a **Administración** → **Gestión de Usuarios**.
2. **Completar los Datos del Usuario**: Proporciona el **nombre**, **correo electrónico**, y asigna un **rol** al usuario (e.g., recepcionista, mecánico, inspector).
3. **Asignar Permisos**: Define los permisos específicos según el rol del usuario.
4. **Guardar Usuario**: Haz clic en **Guardar** para completar la creación del usuario.

### 3.2 Gestión de Permisos

Los permisos definen qué acciones puede realizar cada usuario. Los roles predefinidos tienen permisos asociados, pero estos se pueden ajustar manualmente para usuarios específicos.

---

## 4. Monitoreo y Mantenimiento del Sistema

### 4.1 Monitoreo del Sistema

**Herramientas Utilizadas**:
- **Visor de Eventos de Windows**: Para verificar errores y advertencias del sistema.
- **Monitor de Recursos**: Para evaluar el uso de CPU, memoria y disco.

**Métricas Importantes**:
- Uso de CPU y memoria del servidor.
- Espacio en disco disponible para la base de datos.

### 4.2 Mantenimiento Preventivo

**Tareas Recomendadas**:
- **Actualizaciones**: Mantener el sistema operativo y los drivers actualizados.
- **Reinicios Programados**: Reiniciar el servidor mensualmente para liberar recursos.
- **Pruebas de Rendimiento**: Ejecutar pruebas de rendimiento cada tres meses para asegurar la eficiencia del sistema.

---

## 5. Respaldo y Restauración de Datos

### 5.1 Respaldo de la Base de Datos

**Frecuencia**: Los respaldos deben realizarse diariamente, preferentemente en horarios nocturnos para evitar afectar la operatividad.

**Pasos para realizar un respaldo**:

1. **Acceder al Menú de Administración**: En el menú principal, ir a **Administración** → **Respaldo de Bases**.
2. **Seleccionar Respaldar Base de Datos**: Haz clic en el botón **Respaldar Base de Datos**.
3. **Seleccionar Ubicación del Respaldo**: Se abrirá una ventana para seleccionar la carpeta donde se desea guardar el archivo de respaldo.
4. **Iniciar Respaldo**: Una vez seleccionada la carpeta, el sistema ejecutará el comando SQL para crear el archivo de respaldo.

### 5.2 Restauración de la Base de Datos

**Situaciones Comunes**:
- **Falla del Sistema**: Restaurar un respaldo reciente para recuperar la operatividad.
- **Pérdida de Datos**: Restaurar una versión previa para recuperar datos perdidos.

**Pasos para restaurar**:

1. **Acceder al Menú de Administración**: En el menú principal, ir a **Administración** → **Respaldo de Bases**.
2. **Seleccionar Restaurar Base de Datos**: Haz clic en el botón **Restaurar Base de Datos**.
3. **Seleccionar Archivo de Respaldo**: Se abrirá una ventana para seleccionar el archivo de respaldo que se desea restaurar.
4. **Iniciar Restauración**: Una vez seleccionado el archivo, el sistema ejecutará el comando SQL para restaurar la base de datos utilizando el archivo seleccionado.

---

## 6. Actualizaciones del Sistema

### 6.1 Aplicar Actualizaciones

Las actualizaciones del sistema pueden incluir mejoras de seguridad, correcciones de errores o nuevas funcionalidades.

**Pasos para aplicar una actualización**:

1. **Descargar Actualización**: Descarga el paquete de actualización desde el sitio seguro del proveedor.
2. **Ejecutar Instalador de Actualización**: Sigue las instrucciones para aplicar la actualización.
3. **Verificar la Instalación**: Asegúrate de que todos los componentes funcionen correctamente después de la actualización.

---

## 7. Solución de Problemas Comunes

### 7.1 Problemas de Conexión

**Causa Común**: Problemas de conectividad con el servidor de base de datos.

**Solución**:
- Verificar la configuración del **connection string**.
- Asegurarse de que el servidor SQL esté en funcionamiento.

### 7.2 Problemas de Rendimiento

**Causa Común**: Alto uso de recursos del servidor.

**Solución**:
- Reiniciar el servidor para liberar memoria.
- Verificar los procesos que están consumiendo más recursos y optimizar su uso.
