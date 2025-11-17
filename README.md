# 📘 Sistema de Pedidos para la Cafetería Universitaria  
### **README.md – Documento Final Integrado (Versión Completa y Actualizada)**

---

## 📝 1. Descripción del Caso

El **Sistema de Pedidos para la Cafetería Universitaria** fue desarrollado para agilizar la toma de pedidos, mejorar la organización interna y optimizar la comunicación entre caja y cocina.  
Permite una gestión eficiente, precisa y estructurada de los pedidos.

El sistema incluye:

- Registro de pedidos con datos del cliente (nombre, mesa o para llevar).  
- Administración del menú: agregar, editar, eliminar y consultar productos.  
- Calcular subtotal, IVA y total automáticamente.  
- Enviar pedidos al módulo de cocina y actualizar estados.  
- Generar comprobantes imprimibles o visibles.  

---

## 🎯 2. Objetivos del Sistema

### **Objetivo General**
Optimizar la gestión de pedidos mediante un sistema digital ágil, eficiente y de fácil uso.

### **Objetivos Específicos**
- Reducir errores en la toma de pedidos.  
- Mejorar la coordinación entre áreas internas.  
- Facilitar actualización del menú y precios.  
- Garantizar una experiencia ágil para el usuario.  
- Generar comprobantes ordenados y claros.  

---

## 🧩 3. Requerimientos del Sistema (Versión Final Integrada)

### 🟦 **Requerimientos Funcionales (Combinados V1 + V2)**

| Nº | Código | Descripción |
|----|--------|-------------|
| 1 | RF1 | El sistema debe permitir al usuario seleccionar productos del menú y registrar un pedido con los datos del cliente. |
| 2 | RF2 | El sistema debe permitir agregar, editar, eliminar y consultar productos	del	menú. |
| 3 | RF3 | El sistema debe calcular de forma automática el valor total del pedido según los productos seleccionados y sus cantidades. |
| 4 | RF4 | El sistema debe permitir cambiar el estado de un pedido. |
| 5 | RF5 | El sistema debe generar un comprobante del pedido con los detalles de los productos, precios y total a pagar. |
| 6 | RF6 | El sistema debe mostrar únicamente los productos disponibles, organizados por categorías para facilitar la selección. |
| 7 | RF7 | El sistema debe permitir registrar un pedido con opciones personalizadas como notas o preferencias especiales del cliente. |
| 8 | RF8 | El sistema debe permitir modificar las cantidades, agregar o eliminar productos del pedido antes de confirmarlo. |
| 9 | RF9 | El sistema debe calcular automáticamente el subtotal, impuesto (IVA) y total final del pedido. |
| 10 | RF10 | El sistema debe enviar los pedidos confirmados al módulo de cocina y permitir actualizar su estado entre las etapas establecidas. |
---

### 🟨 **Requerimientos No Funcionales (Combinados y Ampliados)**

| Nº | Código | Descripción |
|----|--------|-------------|
| 1 | RNF1 | El sistema debe procesar la confirmación de un pedido en un máximo de 1.5 a 2 segundos. |
| 2 | RNF2 | La interfaz debe ser intuitiva, accesible y fácil de usar sin capacitación técnica. |
| 3 | RNF3 | El sistema debe adaptarse correctamente a distintas resoluciones (PC y tablets) y garantizar un 99% de disponibilidad. |
| 4 | RNF4 | Seguridad: El sistema debe implementar autenticación, roles de usuario y proteger datos sensibles. |
| 5 | RNF5 | Registro y auditoría: El sistema debe almacenar logs de operaciones críticas como creación, edición o cancelación de pedidos. |
| 6 | RNF6 | Resiliencia y recuperación: El sistema debe contar con copias de seguridad periódicas y mecanismos de recuperación ante fallos. |

---

## 🧪 4. Tabla de Pruebas (Integrada)

### ✔ **Casos de Prueba Unitarios**

| Caso | Requerimiento | Entrada | Resultado Esperado |
|------|---------------|---------|--------------------|
| PU1 | RF2 | Pedido: Latte + nota “sin azúcar” | El pedido se registra correctamente con la nota. |
| PU2 | RF3 | Cambiar cantidad: Latte x1 → x3 | El subtotal se actualiza correctamente. |
| PU3 | RF4 | Subtotal $7.00 | El sistema calcula IVA y total final correctamente. |
| PU4 | RF5 | Editar precio de un producto | El nuevo precio se actualiza en el menú. |
| PU5 | RF6 | Cambiar estado a "En preparación" | El estado se actualiza en módulo cocina. |

---

### ✔ **Casos de Validación**

| Caso | Requerimiento | Escenario | Resultado Esperado |
|------|---------------|-----------|--------------------|
| PV1 | RF1 | Abrir menú | Se muestran solo productos disponibles. |
| PV2 | RNF1 | Confirmar pedido de 5 artículos | El pedido se confirma en ≤ 1.5 segundos. |
| PV3 | RF7 | Generación de comprobante | Se muestra ticket con totales e IVA. |
| PV4 | RNF2 | Usuario sin experiencia registra un pedido | Lo realiza sin dificultad. |
| PV5 | RNF5 | Verificar logs del sistema | El registro muestra creación, edición y cancelación correctamente. |

---

## 🛠️ 5. Tipo de Mantenimiento Propuesto

### ⭐ **Mantenimiento Perfectivo**
- Integrar un módulo de seguimiento del pedido para el cliente.  
- Incorporar notificaciones PUSH, SMS o dentro del sistema.  
- Mejorar accesibilidad (modo oscuro, escalado de fuentes).  

### 🐞 **Mantenimiento Correctivo**
- Corregir errores encontrados en la cancelación de pedidos.  
- Resolver inconsistencias al actualizar estados del pedido.  

---

## 🔄 6. Reflexión sobre el Control de Versiones

El uso de control de versiones mediante **Git y GitHub** es fundamental porque:

- Mantiene un historial exacto y ordenado.  
- Facilita la colaboración por medio de ramas y revisiones.  
- Permite revertir errores fácilmente.  
- Asegura sincronización entre código, documentación y pruebas.  

**Buenas prácticas:**
- Commits pequeños y descriptivos.  
- Ramas por funcionalidad.  
- Revisiones antes de aplicar cambios.  

---

## 📚 7. Conclusión

La integración de requerimientos, pruebas y mantenimiento asegura que el sistema sea escalable, eficiente y confiable para la cafetería.  
El uso de GitHub fortalece la organización, control y trabajo colaborativo durante el ciclo de vida del software.


---

## 🏁 8. Bibliografía

- Jain, A. (2025). *Requisitos funcionales y no funcionales*. Visure Solutions.  
- Mentores Tech (2025). *Tipos de requerimientos en software*.  

