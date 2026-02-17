---
fecha: Febrero 2026
title: Plantilla ![arc42](./images/arc42-logo.png)
---

# 1. Introducción y Metas

## Propósito del Sistema

El propósito de este proyecto es diseñar un sistema ERP (Enterprise Resource Planning) orientado a asaderos de pollo, que permita gestionar de forma integrada y eficiente los procesos principales del negocio.

El sistema permitirá administrar los módulos de:

- Compras
- Facturación Electrónica
- Stock y Costos
- Activos Fijos
- Empleados
- EIS (Executive Information System)

Este sistema permitirá mejorar el control, la organización y la toma de decisiones dentro del negocio.

---

## Objetivos del Sistema

Diseñar un sistema ERP funcional, integrable y comercializable, capaz de gestionar la operación completa de un asadero de pollo, incluyendo compras, inventario, facturación, activos, empleados y reportes ejecutivos.

---

## Stakeholders

| Stakeholder | Descripción | Necesidad |
|------------|-------------|-----------|
| Administrador | Administra el sistema | Control total del sistema |
| Gestor de Inventario | Controla el inventario | Registrar y consultar stock |
| Responsable de Compras | Gestiona compras | Crear y consultar órdenes |
| Responsable de Facturación | Maneja facturas | Generar facturas |
| Gerencia | Toma decisiones | Consultar reportes |

---

# 2. Restricciones de Arquitectura

## Restricciones Tecnológicas

El sistema ERP será desarrollado utilizando las siguientes tecnologías:

- Lenguaje de programación: C#
- Framework: .NET
- Base de datos: SQL Server
- Entorno de desarrollo: Visual Studio Community
- Control de versiones: GitHub
- Documentación: arc42
- Diagramación: PlantUML (PlantText)

---

## Restricciones Organizacionales

- El sistema será desarrollado como proyecto académico.
- El sistema debe cubrir los módulos definidos en el documento de la guía.

---

## Restricciones Técnicas

- El sistema debe ser modular.
- Debe permitir integración entre módulos.
- Debe permitir almacenamiento en base de datos.

---

# 3. Alcance y Contexto del Sistema

## Descripción General

El sistema ERP permitirá a los asaderos de pollo gestionar sus procesos principales en una sola plataforma.

Los usuarios interactúan con el sistema para realizar operaciones como:

- Registrar compras
- Generar facturas
- Controlar inventario
- Gestionar empleados
- Consultar reportes

---

## Diagrama de Contexto

![Diagrama de Contexto](./images/Diagrama%20de%20Contexto.png)

---

## Sistemas Externos

- Sistema Contable
- Sistema Bancario

---

## Usuarios

- Administrador
- Responsable de Compras
- Responsable de Facturación
- Gestor de Inventario
- Gerencia

---

# 5. Vista de Bloques de Construcción

## Descripción

El sistema ERP está compuesto por los siguientes contenedores:

---

## Aplicación Web

Responsable de:

- Mostrar la interfaz al usuario
- Permitir interacción con el sistema

---

## API Backend

Responsable de:

- Implementar la lógica de negocio
- Procesar las solicitudes

Incluye los módulos:

- Compras
- Facturación
- Stock y Costos
- Activos Fijos
- Empleados
- EIS

---

## Base de Datos

Responsable de:

- Almacenar toda la información del sistema

---

## Diagrama de Contenedores

![Diagrama de Contenedores](./images/Diagrama%20de%20Contenedores.png)

---

# 6. Vista de Ejecución

## Escenario: Registrar Entrada de Inventario

Este escenario describe el proceso cuando el usuario registra una entrada de inventario.

---

## Flujo

1. El usuario ingresa la información del producto
2. La aplicación web envía la información al API
3. El API valida los datos
4. El API guarda la información en la base de datos
5. El sistema confirma el registro

---

## Diagrama de Secuencia

![Diagrama de Secuencia](./images/Diagrama%20de%20Secuencia.png)

---

# 7. Vista de Despliegue

## 7.1 Descripción General

El sistema ERP será desplegado utilizando una arquitectura cliente-servidor.

El sistema estará compuesto por:

- Cliente Web
- Servidor de Aplicación ERP
- Servidor de Base de Datos

Esta arquitectura permite separar la interfaz de usuario, la lógica de negocio y el almacenamiento de datos.

---

## 7.2 Nodos de Despliegue

### Cliente

Dispositivo del usuario que accede al sistema.

Puede ser:

- Computador
- Laptop

Software utilizado:

- Navegador Web (Chrome, Edge, etc)

Responsabilidad:

- Mostrar la interfaz gráfica
- Enviar solicitudes al servidor

---

### Servidor de Aplicación

Equipo donde se ejecuta el sistema ERP desarrollado en C# .NET.

Responsabilidades:

- Procesar solicitudes de los usuarios
- Ejecutar la lógica de negocio
- Gestionar los módulos:

  - Compras
  - Facturación Electrónica
  - Stock y Costos
  - Activos Fijos
  - Empleados
  - EIS

- Comunicarse con la base de datos

---

### Servidor de Base de Datos

Servidor que ejecuta SQL Server.

Responsabilidades:

- Almacenar los datos del sistema
- Guardar información de:

  - Productos
  - Proveedores
  - Facturas
  - Inventario
  - Empleados
  - Activos
  - Reportes

---

## 7.3 Comunicación entre los Componentes

El flujo de comunicación es el siguiente:

1. El usuario accede al sistema mediante el navegador web

2. El navegador envía una solicitud al servidor ERP mediante protocolo HTTP o HTTPS

3. El servidor ERP procesa la solicitud utilizando la lógica de negocio

4. El servidor ERP consulta o guarda información en la base de datos SQL Server

5. La base de datos devuelve la respuesta al servidor ERP

6. El servidor ERP envía la respuesta al cliente

7. El cliente muestra el resultado al usuario

---

## 7.4 Beneficios de esta Arquitectura

Esta arquitectura permite:

- Separación de responsabilidades
- Mayor seguridad
- Mejor organización del sistema
- Facilidad de mantenimiento
- Escalabilidad futura

---

## Diagrama de Despliegue

![Diagrama de Despliegue](./images/Diagrama%20de%20Despliegue.png)

---

# 10. Glosario

## ERP

Sistema de planificación de recursos empresariales.

---

## Producto

Elemento que el negocio compra o vende.

---

## Proveedor

Empresa que suministra productos.

---

## Inventario

Cantidad de productos disponibles.

---

## Factura

Documento que registra una venta.

---

## Activo Fijo

Bien propiedad de la empresa.

---

## Empleado

Persona que trabaja en la empresa.

---

## EIS

Sistema de información ejecutiva para toma de decisiones.
