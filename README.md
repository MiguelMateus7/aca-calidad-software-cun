# ACA FINAL: DISEÑO Y ELABORACIÓN DE DOS PRUEBAS DE SOFTWARE Y TRES MÉTRICAS DE CALIDAD

**Asignatura:** Calidad del Software  
**Ficha:** 54461 - Segundo Bloque  
**Docente / Tutor:** Alexander Calderón Martínez  
**Institución:** Corporación Unificada Nacional de Educación Superior (CUN)  
**Año:** 2026  

---

## 👥 Integrantes
* **Miguel Ángel Pérez Mateus**
* **Gabriel Geovanny Vargas Molina**

---

## 🖥️ Sistema Evaluado
* **Nombre del Software:** Swag Labs Inventory System (SauceDemo App)
* **URL del Entorno Web:** [https://www.saucedemo.com/](https://www.saucedemo.com/)
* **Descripción:** Plataforma web transaccional para la gestión e inspección de catálogo de productos e inventarios.

---

## 🧪 Resumen de Pruebas de Software

### 1. Prueba Funcional (Caja Negra) - CP-01
* **Módulo:** Inicio de sesión y control de acceso.
* **Datos de Entrada:** `Username: standard_user` | `Password: secret_sauce`
* **Resultado Esperado:** Redirección exitosa a `/inventory.html` y renderizado correcto de la parrilla de productos.
* **Estado:** **PASSED (Exitoso)**

### 2. Prueba de Rendimiento / Red - CP-02
* **Módulo:** Inspección de respuesta HTTP y latencia de carga mediante DevTools (F12).
* **Parámetros Medidos:** Código de estado `200 OK`, peso de transferencia y tiempo de finalización.
* **Resultado Obtenido:** 6 solicitudes HTTP exitosas, 581.07 kB transferidos y **1.07 segundos** de tiempo total de carga.
* **Estado:** **PASSED (Exitoso)**

---

## 📊 Métricas de Calidad (Norma ISO/IEC 25010)

1. **Densidad de Defectos (DD):**
   $$\text{DD} = \frac{2 \text{ defectos}}{1.2 \text{ KLOC}} = 1.67 \text{ defectos/KLOC}$$
   *(Valor óptimo de mantenibilidad y bajo índice de fallas).*

2. **Cobertura de Pruebas Funcionales (CP):**
   $$\text{CP} = \left(\frac{2 \text{ casos aprobados}}{2 \text{ casos diseñados}}\right) \times 100 = 100\%$$
   *(Cumplimiento total del alcance planificado).*

3. **Tiempo Medio de Respuesta (TMR):**
   $$\text{TMR} = 1.07 \text{ segundos}$$
   *(Satisface el requerimiento no funcional de responder en menos de 2.0 segundos).*

---

## ⚠️ Análisis Crítico y Riesgos
* **Riesgos de Seguridad:** Falta de bloqueo de intentos fallidos (Rate Limiting) en la vista de acceso.
* **Optimización:** El script principal (`index-DnLqFCJl.js`) pesa 550 kB, por lo que se recomienda aplicar minificación y división de código (*Code Splitting*).

---

## 🎥 Entregable Multimedia
* **Video Pitch en YouTube:** [Ver Explicación del Proyecto](https://www.youtube.com/watch?v=ACA_FINAL_CALIDAD_CUN_2026)
