# 🧾 Informe Técnico — Mantenimiento de Software
## 📌 Sistema de Pedidos – Cafetería Universitaria

---

## 🟦 1. Descripción del Sistema

El **Sistema de Pedidos para Cafetería Universitaria** es una aplicación diseñada para agilizar y optimizar el proceso de compra de alimentos dentro del campus.

Permite a estudiantes, docentes y personal:

- Consultar el menú disponible.
- Realizar pedidos desde dispositivos móviles o terminales.
- Pagar de forma rápida y sencilla.
- Recibir notificaciones del estado del pedido.

El sistema envía pedidos en tiempo real al área de cocina, reduce tiempos de espera y mejora la organización interna.  
También incluye herramientas administrativas para control de inventarios, productos y reportes.

---

## 🟦 2. Análisis del Problema

### 🟥 2.1. Ausencia de Seguimiento del Pedido

No existe un mecanismo para rastrear el estado del pedido.

**🔧 Tipo de mantenimiento:** Perfectivo

**Impacto en estudiantes:**

- Incertidumbre por tiempos de espera.
- Ansiedad por no conocer el estado del pedido.
- Pérdida de tiempo.

**Impacto en el personal:**

- Saturación en el punto de entrega.
- Estrés por presión de clientes.
- Interrupciones constantes por consultas.

**Consecuencias:**

- Ineficiencia en gestión de tiempos de preparación.
- Flujo de trabajo interrumpido.
- Confusiones en la secuencia de pedidos.

---

### 🟥 2.2. Ausencia de Sistema de Notificaciones

No existe un mecanismo automático que informe el estado del pedido.

**🔧 Tipo de mantenimiento:** Perfectivo

**Comunicación ineficiente:**

- El usuario debe estar presente para obtener información.
- No existen alertas automáticas.
- No hay confirmaciones de estado.

**Experiencia del usuario:**

- Frustración.
- Incertidumbre constante.
- Sensación de desorganización.

**Consecuencias:**

- El personal pierde tiempo repitiendo información.
- No existe historial de notificaciones.
- No es posible notificar retrasos o cambios.

---

## 🟦 3. Tipos de Mantenimiento

El mantenimiento permite corregir errores, mejorar rendimiento, adaptarse a cambios y prevenir fallos futuros.  
Representa entre **60% y 80%** del costo total del software.

### 🔧 Tipos principales

| Tipo | Descripción |
|------|-------------|
| 🐞 **Correctivo** | Corrige errores detectados luego del despliegue. |
| 🔄 **Adaptativo** | Ajusta el sistema a cambios del entorno. |
| ⚙️ **Perfectivo** | Mejora funcionalidades o rendimiento. |
| 🛡️ **Preventivo** | Prevé fallos futuros y mejora la estructura interna. |

### 💲 Factores que aumentan el costo

- Código mal estructurado.
- Falta de estándares.
- Requisitos cambiantes.
- Tecnologías obsoletas.

### 💲 Factores que reducen el costo

- Buen diseño desde el inicio.
- Documentación clara.
- Programación modular.
- Uso de control de versiones.

---

## 🟦 3.1. Tipos de Mantenimiento Aplicables

| Tipo | Descripción |
|------|-------------|
| ⚙️ **Perfectivo** | Mejora la funcionalidad, rendimiento y usabilidad. |
| 🐞 **Correctivo** | Corrige errores detectados en producción. |

---

## 🟦 4. Justificación Teórica y Técnica

### 🟩 4.1. Mantenimiento Perfectivo

| Base Teórica | Justificación Técnica |
|--------------|------------------------|
| Mejora de Funcionalidad y Eficiencia | - Integración de nuevos métodos de pago.<br>- Creación de paneles para administrador y cocinero.<br>- Módulo de seguimiento y notificaciones. |
| Mejora de Usabilidad | - Implementación de modo nocturno. |

---

### 🟥 4.2. Mantenimiento Correctivo

| Base Teórica | Justificación Técnica |
|--------------|------------------------|
| Corrección de Errores | - Se corrige el error donde la cancelación de pedidos no se registraba, afectando la integridad de datos. |

---

## 🟦 5. Cambio Funcional Propuesto

### ⭐ 5.1. Sistema Integral de Seguimiento y Notificaciones

El nuevo sistema incluye:

- Seguimiento en tiempo real.
- Notificaciones multicanal.
- Pagos digitales avanzados.
- Sistema de temas visuales.

---

### ⭐ 5.2. Módulo de Seguimiento en Tiempo Real

Incluye:

- Barra de progreso con estados:  
  **Recibido → En preparación → Listo → Entregado**  
- Temporizador inteligente con tiempos estimados.
- Actualizaciones cada 30 segundos mediante WebSockets.

---

### ⭐ 5.3. Notificaciones Multicanal

- Notificaciones PUSH (Firebase).
- SMS como respaldo.
- Notificaciones dentro de la app.
- Tres alertas estratégicas por pedido.

---

### ⭐ 5.4. Métodos de Pago Expandidos

- Tarjetas débito/crédito (PCI DSS).
- Billetera digital universitaria.
- Recargas online.
- Sistema de cashback.

---

### ⭐ 5.5. Sistema de Temas Visuales (Incluye Modo Nocturno)

- Tema claro, oscuro y sepia.
- Accesibilidad AA (contraste 4.5:1).
- Fuentes escalables.
- Iconografía consistente.

---

### ⭐ 5.6. Flujo de Usuario Mejorado

- Flujo optimizado desde compra hasta retiro.
- Arquitectura basada en microservicios.
- APIs RESTful documentadas.
- Código modular y testeable.

---

### ⭐ 5.7. Plan de Implementación

El sistema se implementará en 4 fases alineadas con buenas prácticas de ingeniería de software.

---

## 🟦 6. Reflexión Final

El desarrollo del sistema demuestra cómo la ingeniería de software permite resolver problemas reales mediante automatización y optimización de procesos.  
Este proyecto fortaleció habilidades técnicas, trabajo en equipo y toma de decisiones, mostrando el impacto del software en la mejora institucional y la experiencia del usuario.

---
