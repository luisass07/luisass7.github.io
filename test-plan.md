# Plan de Pruebas – Sprint 0

Este documento define los casos de prueba para las historias de usuario del sistema ERP PolloSoft.

---

# Casos De Prueba – Módulo de Compras

| ID | Caso de prueba | Resultado esperado |
|----|---------------|-------------------|
TC01 | Registrar una orden de compra con proveedor y productos | La orden se guarda correctamente |
TC02 | Registrar compra sin proveedor | El sistema muestra un mensaje de error |
TC03 | Agregar varios productos a la compra | El sistema calcula el total correctamente |
TC04 | Guardar orden de compra | La información queda almacenada |
TC05 | Consultar una orden registrada | La orden aparece en el sistema |

---

# Casos De Prueba – Módulo de Facturación

| ID | Caso de prueba | Resultado esperado |
|----|---------------|-------------------|
TC06 | Crear factura con productos válidos | La factura se genera correctamente |
TC07 | Crear factura sin productos | El sistema muestra error |
TC08 | Calcular total de factura | El sistema calcula subtotal e impuestos |
TC09 | Guardar factura | La factura queda registrada |
TC10 | Consultar factura generada | El sistema muestra la factura |

---

# Casos De Prueba – Módulo Stock / Costos

| ID | Caso de prueba | Resultado esperado |
|----|---------------|-------------------|
TC11 | Consultar inventario | El sistema muestra productos disponibles |
TC12 | Buscar producto por nombre | El sistema muestra el resultado correcto |
TC13 | Ver costo del producto | El sistema muestra el costo |
TC14 | Registrar compra de producto | El stock aumenta |
TC15 | Registrar venta de producto | El stock disminuye |

---

# Casos De Prueba – Módulo Activos Fijos

| ID | Caso de prueba | Resultado esperado |
|----|---------------|-------------------|
TC16 | Registrar activo con datos correctos | El activo queda guardado |
TC17 | Registrar activo sin nombre | El sistema muestra error |
TC18 | Consultar lista de activos | El sistema muestra los activos |
TC19 | Editar información del activo | Los cambios se guardan |
TC20 | Eliminar activo | El activo desaparece del sistema |

---

# Casos De Prueba – Módulo Empleados

| ID | Caso de prueba | Resultado esperado |
|----|---------------|-------------------|
TC21 | Registrar empleado con datos completos | El empleado queda guardado |
TC22 | Registrar empleado sin documento | El sistema muestra error |
TC23 | Consultar lista de empleados | El sistema muestra los empleados |
TC24 | Editar datos del empleado | La información se actualiza |
TC25 | Eliminar empleado | El empleado se elimina del sistema |

---

