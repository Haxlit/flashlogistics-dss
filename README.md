# 🚚 FlashLogistics DSS
> **Materia:** Sistemas de Información II — Actividad 2: Formulación del MVP  
> **Unidad:** Elicitación y Formulación de Proyectos de Software

---

## 👥 Equipo (Squad)

| Integrante | 
|---|
| Josue Adhemar Mamani Huanacu | 
| Josue Matias Arroyo Reynoso | 
| Luis Fernando Arias Segovia | 

---

## 🎯 Visión del Producto

> *"Para FlashLogistics, que sufre un 30% de entregas tardías y una sobrecarga operativa crítica,  
> el **DSS FlashLogistics** es un sistema de soporte a la decisión  
> que optimiza rutas, monitorea la flota en tiempo real y automatiza la comunicación con el cliente.  
> A diferencia de las hojas Excel y la pizarra manual actuales,  
> nuestro producto provee inteligencia operativa basada en datos para escalar el negocio."*

---

## 🌳 Análisis Sistémico

### Árbol de Problemas

                ┌─────────────────────────────────────────────────────────┐
                │                  🌿 EFECTOS (Ramas)                     │
                ├───────────────┬──────────────┬────────────┬─────────────┤
                │ Pérdida de    │ Empresa no   │ Fatiga y   │Rentabilidad │
                │ clientes y    │ puede        │ estrés del │comprometida │
                │ contratos     │ escalar      │ personal   │(ODS 8)      │
                └───────┬───────┴──────┬───────┴─────┬──────┴──────┬──────┘
                        │              │             │             │
                ┌───────┴──────────────┴─────────────┴─────────────┴──────┐
                │                  🪵 PROBLEMA CENTRAL (Tronco)            │
                │  FlashLogistics carece de un sistema de gestión que      │
                │  permita planificar rutas eficientemente, monitorear     │
                │  entregas en tiempo real y analizar el desempeño         │
                │  operativo → 30% entregas tardías · +15% combustible     │
                └───────┬──────────────┬─────────────┬─────────────┬──────┘
                        │              │             │             │
                ┌───────┴───┐  ┌───────┴───┐ ┌──────┴─────┐ ┌────┴───────┐
                │  🌱 CR1   │  │  🌱 CR2   │ │  🌱 CR3    │ │  🌱 CR4   │
                │Planifica- │  │ Sin monit.│ │Comunicac.  │ │ Sin datos  │
                │ción manual│  │ en tiempo │ │ineficiente │ │ ni KPIs    │
                │ de rutas  │  │   real    │ │con cliente │ │            │
                └───────────┘  └───────────┘ └────────────┘ └────────────┘

| # | Causa Raíz | Descripción | Sub-causas |
|---|---|---|---|
| CR1 | Planificación manual de rutas | Rutas diseñadas en pizarra y Excel sin optimización → asignaciones subóptimas y combustible desperdiciado | Sin algoritmo de optimización · Dependencia del criterio empírico · Sin variables de tráfico o capacidad |
| CR2 | Ausencia de monitoreo en tiempo real | El gerente no sabe dónde están los camiones → imposible reaccionar ante imprevistos | Sin GPS integrado · Sin alertas de desvíos · Sin mapa operativo centralizado |
| CR3 | Comunicación ineficiente con el cliente | Clientes sin acceso a estado de pedidos → 4 hrs/día de llamadas que sobrecargan al equipo | Sin portal de autoservicio · Sin notificaciones automáticas · Solo canal telefónico |
| CR4 | Inexistencia de datos e indicadores | Sin registro histórico de operaciones → imposible identificar fallas ni mejorar | Sin base de datos histórica · Sin KPIs · Sin herramientas de reportería |

---

### Árbol de Soluciones

                ┌─────────────────────────────────────────────────────────┐
                │                ✅ BENEFICIOS (Ramas+)                    │
                ├───────────────┬──────────────┬────────────┬─────────────┤
                │ Fidelización  │Escalabilidad │ Bienestar  │Rentabilidad │
                │ y crecimiento │ operativa    │ del equipo │ sostenible  │
                │ de cartera    │ real         │ (ODS 8)    │             │
                └───────┬───────┴──────┬───────┴─────┬──────┴──────┬──────┘
                        │              │             │             │
                ┌───────┴──────────────┴─────────────┴─────────────┴──────┐
                │                  🎯 OBJETIVO CENTRAL (Tronco+)           │
                │  FlashLogistics implementa un DSS que optimiza rutas,    │
                │  provee visibilidad en tiempo real, automatiza la        │
                │  comunicación con el cliente y genera inteligencia        │
                │  operativa → -50% entregas tardías · -10% combustible    │
                └───────┬──────────────┬─────────────┬─────────────┬──────┘
                        │              │             │             │
                ┌───────┴───┐  ┌───────┴───┐ ┌──────┴─────┐ ┌────┴───────┐
                │  ⚙️ M1    │  │  ⚙️ M2    │ │  ⚙️ M3     │ │  ⚙️ M4    │
                │Optimizac. │  │ Tracking  │ │  Portal    │ │ Dashboard  │
                │ de Rutas  │  │    GPS    │ │ Pedidos    │ │ Analytics  │
                └───────────┘  └───────────┘ └────────────┘ └────────────┘
                
  | Causa Raíz | Módulo DSS | KPI de Éxito |
|---|---|---|
| CR1: Planificación manual | 🗺️ Módulo 1 – Optimización de Rutas | Reducir entregas tardías del 30% → 15% en 3 meses |
| CR2: Sin monitoreo en tiempo real | 📍 Módulo 2 – Tracking GPS | 100% flota rastreada · Respuesta ante incidencias < 10 min |
| CR3: Comunicación ineficiente | 📲 Módulo 3 – Portal de Pedidos | Reducir llamadas en 80% · Liberar 4 hrs/día del equipo |
| CR4: Sin datos ni KPIs | 📊 Módulo 4 – Dashboard Analytics | 5+ KPIs operativos disponibles para decisiones diarias |

---

## 🗺️ Canvas MVP

| Elemento | Detalle |
|---|---|
| **Propuesta de Valor** | Visibilidad total de la operación logística en tiempo real, con decisiones basadas en datos y clientes informados automáticamente |
| **Usuarios Objetivo** | Gerente de Operaciones · Despachadores · Conductores · Clientes |
| **Funcionalidades Mínimas (MVP)** | Optimización de rutas · Tracking GPS · Portal de seguimiento de pedidos · Dashboard de KPIs |
| **Lo que NO es el MVP** | No es un ERP · No gestiona inventario · No maneja facturación |
| **Métrica clave** | Tasa de entregas a tiempo ≥ 85% al finalizar el Sprint 3 |
| **KPIs del proyecto** | Entregas tardías · Costo combustible/ruta · Llamadas atendidas/día · Tiempo de planificación · Eficiencia por conductor |
| **Cronograma estimado** | Sprint 1 (mes 1): Módulo 1 · Sprint 2 (mes 2): Módulos 2 y 3 · Sprint 3 (mes 3): Módulo 4 |

---

## 🎯 Objetivo SMART

> **Desarrollar un DSS para FlashLogistics que reduzca la tasa de entregas tardías del 30% al 15%, disminuya los costos de combustible en un 10% y libere al equipo de despacho de 4 horas diarias de atención telefónica, mediante la implementación incremental de 4 módulos funcionales en un plazo de 3 meses (3 sprints de 4 semanas cada uno).**

---

## ⚙️ Módulos del Sistema

### 🗺️ Módulo 1 – Optimización de Rutas
- Motor de cálculo automático con criterios de distancia, tiempo, prioridad y capacidad
- Reemplaza la planificación manual en pizarra y Excel
- **Resuelve:** CR1

### 📍 Módulo 2 – Tracking GPS en Tiempo Real
- Mapa digital con ubicación en vivo de cada camión de la flota
- Alertas automáticas ante desvíos o retrasos
- **Resuelve:** CR2

### 📲 Módulo 3 – Portal de Seguimiento de Pedidos
- Interfaz web/app para que el cliente consulte su pedido 24/7
- Notificaciones automáticas por SMS o correo electrónico
- **Resuelve:** CR3

### 📊 Módulo 4 – Dashboard de Analytics e Indicadores
- Panel gerencial con KPIs: eficiencia por conductor, rutas críticas, cumplimiento de entregas
- Historial operativo para mejora continua basada en datos
- **Resuelve:** CR4

---

## 🏁 Cronograma de Sprints

| Sprint | Duración | Módulos | Entregable |
|---|---|---|---|
| Sprint 1 | Semanas 1–4 | Módulo 1 | Motor de optimización de rutas funcional |
| Sprint 2 | Semanas 5–8 | Módulos 2 y 3 | Tracking GPS + Portal de pedidos operativo |
| Sprint 3 | Semanas 9–12 | Módulo 4 | Dashboard de analytics con KPIs en vivo |

---

## 🌱 Impacto en ODS

| ODS | Impacto |
|---|---|
| **ODS 8** – Trabajo decente y crecimiento económico | Reduce la fatiga cognitiva del equipo al eliminar tareas manuales repetitivas y permite el crecimiento sostenible de la empresa |
| **ODS 9** – Industria, innovación e infraestructura | Moderniza la infraestructura logística de FlashLogistics mediante tecnología de optimización e inteligencia operativa basada en datos |
