# 🚚 FlashLogistics DSS
> **Materia:** Sistemas de Información II — Actividad 2: Formulación del MVP  
> **Unidad:** Elicitación y Formulación de Proyectos de Software  
> **Microcompetencia:** Desarrolla sistemas de información de apoyo a la toma de decisiones para facilitar procesos de negocio mediante metodologías y lenguajes de modelado.

---

## 👥 Equipo (Squad)

| Integrante | 
|---|
| [Josue Mamani] | 
| [Josue Arroyo] | 
| [Luis Arias] |

---

## 📋 Proceso de Elicitación

Para abordar el caso de FlashLogistics, el equipo adoptó un proceso de elicitación mixto que combina análisis sistémico con metodologías ágiles:

- **Análisis del caso de negocio** — lectura crítica para identificar actores, datos cuantitativos y puntos ciegos.
- **Tormenta de ideas (Brainstorming)** — identificación y jerarquización de causas por impacto.
- **Árbol de Problemas** — representación visual sistémica de causas raíz y efectos negativos.
- **Árbol de Soluciones** — transformación de cada causa raíz en módulo de software.
- **Taller Lean Inception** — definición de visión, personas, user journey y canvas MVP.

---

## 📊 Diagnóstico Cuantitativo

| Indicador | Valor Actual | Impacto |
|---|---|---|
| Tasa de entregas tardías | **30%** | Pérdida de contratos y reputación |
| Incremento costos de combustible | **+15% (último semestre)** | Erosión de márgenes operativos |
| Tiempo en llamadas de estado | **4 horas/día por despachador** | Fatiga cognitiva y baja productividad |
| Visibilidad de flota en tiempo real | **0% (nula)** | Imposibilidad de reacción ante incidencias |
| Herramientas de análisis de datos | **Ninguna** | Sin base para mejora continua ni escalamiento |

---

## 🌳 Análisis Sistémico

### Árbol de Problemas

```
        ┌──────────────┬──────────────┬──────────────┬──────────────┐
        │ Pérdida de   │ Empresa no   │ Fatiga y     │Rentabilidad  │
        │ clientes y   │ puede        │ estrés del   │comprometida  │
        │ contratos    │ escalar      │ personal     │              │
        └──────┬───────┴──────┬───────┴──────┬───────┴──────┬───────┘
               │              │              │              │
        ┌──────┴──────────────┴──────────────┴──────────────┴───────┐
        │                   PROBLEMA CENTRAL                         │
        │  FlashLogistics carece de un sistema de gestión que        │
        │  permita planificar rutas eficientemente, monitorear        │
        │  entregas en tiempo real y analizar el desempeño            │
        │  operativo → 30% entregas tardías · +15% combustible        │
        └──────┬──────────────┬──────────────┬──────────────┬───────┘
               │              │              │              │
        ┌──────┴───┐  ┌───────┴──┐  ┌────────┴─┐  ┌────────┴──┐
        │  CR1     │  │  CR2     │  │  CR3     │  │  CR4      │
        │Planific. │  │Sin monit.│  │Comunic.  │  │Sin datos  │
        │manual    │  │en tiempo │  │ineficiente│  │ni KPIs    │
        │de rutas  │  │real      │  │con cliente│  │           │
        └──────────┘  └──────────┘  └──────────┘  └───────────┘
```

| # | Causa Raíz | Descripción | Sub-causas |
|---|---|---|---|
| CR1 | Planificación manual de rutas | Rutas diseñadas en pizarra y Excel sin algoritmo de optimización | Sin lógica de optimización · Dependencia del criterio empírico · Sin variables de tráfico o capacidad |
| CR2 | Ausencia de monitoreo en tiempo real | El gerente no sabe dónde están los camiones → imposible reaccionar ante imprevistos | Sin GPS integrado · Sin alertas de desvíos · Sin mapa operativo centralizado |
| CR3 | Comunicación ineficiente con el cliente | Sin acceso al estado del pedido → 4 hrs/día de llamadas que sobrecargan al equipo | Sin portal de autoservicio · Sin notificaciones automáticas · Solo canal telefónico |
| CR4 | Inexistencia de datos e indicadores | Sin registro histórico → imposible identificar fallas ni mejorar | Sin base de datos histórica · Sin KPIs · Sin herramientas de reportería |

---

### Árbol de Soluciones

```
        ┌──────────────┬──────────────┬──────────────┬──────────────┐
        │ Fidelización │Escalabilidad │ Bienestar    │Rentabilidad  │
        │ y crecimiento│ operativa    │ del equipo   │sostenible    │
        │ de cartera   │ real         │ (ODS 8)      │              │
        └──────┬───────┴──────┬───────┴──────┬───────┴──────┬───────┘
               │              │              │              │
        ┌──────┴──────────────┴──────────────┴──────────────┴───────┐
        │                   OBJETIVO CENTRAL                          │
        │  FlashLogistics implementa un DSS que optimiza rutas,       │
        │  provee visibilidad en tiempo real, automatiza la           │
        │  comunicación con el cliente y genera inteligencia           │
        │  operativa → -50% entregas tardías · -10% combustible       │
        └──────┬──────────────┬──────────────┬──────────────┬───────┘
               │              │              │              │
        ┌──────┴───┐  ┌───────┴──┐  ┌────────┴─┐  ┌────────┴──┐
        │  M1      │  │  M2      │  │  M3      │  │  M4       │
        │Optimiz.  │  │Tracking  │  │  Portal  │  │Dashboard  │
        │de Rutas  │  │GPS       │  │Pedidos   │  │Analytics  │
        └──────────┘  └──────────┘  └──────────┘  └───────────┘
```

| Causa Raíz | Módulo DSS | KPI de Éxito |
|---|---|---|
| CR1: Planificación manual | 🗺️ Módulo 1 – Optimización de Rutas | Reducir entregas tardías del 30% al 15% en 3 meses |
| CR2: Sin monitoreo en tiempo real | 📍 Módulo 2 – Tracking GPS | 100% flota rastreada · Respuesta ante incidencias < 10 min |
| CR3: Comunicación ineficiente | 📲 Módulo 3 – Portal de Pedidos | Reducir llamadas en 80% · Liberar 4 hrs/día del equipo |
| CR4: Sin datos ni KPIs | 📊 Módulo 4 – Dashboard Analytics | 5+ KPIs operativos disponibles para decisiones diarias |

---

## 🎯 Objetivo SMART

Desarrollar un Sistema de Soporte a la Decisión (DSS) para FlashLogistics que, en un plazo de 3 meses mediante tres sprints de desarrollo incremental, reduzca la tasa de entregas tardías del 30% al 15%, disminuya los costos de combustible en un 10% y libere al equipo de despacho de las 4 horas diarias actualmente destinadas a la atención de llamadas de estado, a través de la implementación de cuatro módulos funcionales: optimización automática de rutas, monitoreo GPS de la flota en tiempo real, portal de autoservicio para el cliente y un dashboard de indicadores operativos.

---

## 🌀 Taller Lean Inception

### Visión del Producto

| Componente | Descripción |
|---|---|
| **Para (cliente)** | FlashLogistics, empresa distribuidora con crisis operativa: 30% entregas tardías, +15% combustible y pérdida de contratos |
| **Que (necesidad)** | Necesita optimizar rutas, monitorear su flota en tiempo real, informar automáticamente a sus clientes y tomar decisiones basadas en datos |
| **El (producto)** | DSS FlashLogistics — Sistema de Soporte a la Decisión para gestión logística integral |
| **Es un (categoría)** | Sistema web de gestión logística con módulos de optimización de rutas, tracking GPS, portal de pedidos y dashboard de KPIs |
| **Que (beneficio clave)** | Reduce entregas tardías en 50%, disminuye costos de combustible en 10% y libera al equipo de 4 hrs/día de llamadas |
| **A diferencia de (alternativa)** | Las hojas de cálculo Excel manuales, la pizarra de planificación y el canal telefónico como único medio de comunicación |
| **Nuestro producto (diferenciador)** | Integra en una sola plataforma: optimización de rutas, tracking en tiempo real, autoservicio para el cliente e inteligencia analítica gerencial |

---

### Es / No es / Hace / No hace

| ES ✅ | NO ES ❌ |
|---|---|
| Un Sistema de Soporte a la Decisión (DSS) para logística | Un ERP ni sistema de gestión empresarial completo |
| Una herramienta de optimización de rutas de distribución | Un sistema de gestión de inventario o almacenes |
| Un sistema de monitoreo GPS de flota vehicular | Una plataforma de facturación o gestión financiera |
| Un portal de autoservicio para clientes (estado de pedidos) | Un sistema de recursos humanos o nómina |
| Un dashboard gerencial de KPIs operativos en tiempo real | Un software de comercio electrónico o ventas online |
| Una plataforma web accesible desde dispositivos móviles | Un reemplazo del conductor ni del operador logístico |

| HACE ⚙️ | NO HACE 🚫 |
|---|---|
| Calcula y sugiere rutas óptimas de distribución | No gestiona el inventario de productos en bodega |
| Muestra en mapa la ubicación en tiempo real de cada camión | No procesa pagos ni genera facturas |
| Envía notificaciones automáticas al cliente sobre su pedido | No reemplaza la decisión final del operador logístico |
| Permite al cliente consultar el estado de su entrega 24/7 | No controla el mantenimiento mecánico de los vehículos |
| Genera reportes de eficiencia por conductor y por ruta | No administra contratos ni relaciones comerciales |
| Almacena histórico de operaciones para análisis de tendencias | No opera sin conectividad (requiere internet en tiempo real) |
| Alerta al gerente ante desvíos o retrasos en tiempo real | No incluye app móvil nativa en el MVP (versión web responsive) |

---

### Personas (Perfiles de Usuario)

#### 👤 Persona 1 — Carlos Medina · Gerente de Operaciones
> *"Necesito saber dónde está cada camión y cuántas entregas llegaron a tiempo, antes de que el cliente me llame."*

| Campo | Detalle |
|---|---|
| **Objetivo principal** | Tener control total sobre la operación logística: ubicación de flota, KPIs del día y alertas ante problemas en tiempo real |
| **Punto de dolor** | Toma decisiones a ciegas. No tiene visibilidad de la flota ni indicadores. Se entera de los problemas cuando ya es tarde |
| **Comportamiento** | Trabaja desde oficina central. Usa Excel y WhatsApp para coordinar. Recibe llamadas de emergencia de conductores y clientes |
| **Funciones clave** | Dashboard de KPIs, mapa de flota en tiempo real, alertas de retrasos, reporte automático del cierre del día |

#### 👤 Persona 2 — Ana Rojas · Despachadora Senior
> *"Paso las primeras 2 horas del día haciendo rutas en la pizarra y el resto atendiendo llamadas. Necesito herramientas."*

| Campo | Detalle |
|---|---|
| **Objetivo principal** | Planificar rutas rápidamente y que los clientes puedan consultar el estado de su pedido sin llamar al despacho |
| **Punto de dolor** | 2 horas de planificación manual + 40 llamadas diarias de estado de pedidos = jornada agotadora con alto margen de error |
| **Comportamiento** | Muy organizada pero sobrecargada. Conoce las rutas de memoria. Le frustra repetir la misma información todo el día |
| **Funciones clave** | Módulo de optimización de rutas con asignación automática, visualización de rutas asignadas, notificaciones automáticas al cliente |

#### 👤 Persona 3 — Diego Villanueva · Cliente (Gerente de Compras)
> *"Si no sé cuándo llega mi pedido, no puedo planificar mi operación. Ya estoy pensando en cambiar de proveedor."*

| Campo | Detalle |
|---|---|
| **Objetivo principal** | Saber en todo momento el estado de su pedido y recibir entregas en el horario acordado |
| **Punto de dolor** | Sin visibilidad del pedido. Debe llamar a FlashLogistics y esperar. Entregas tardías sin aviso previo lo perjudican internamente |
| **Comportamiento** | Exigente y orientado a la eficiencia. Evalúa continuamente a sus proveedores. Tiene poder de decisión sobre el contrato |
| **Funciones clave** | Portal de seguimiento con estado en tiempo real, notificaciones automáticas de despacho y entrega próxima, historial de entregas |

---

### User Journey — Recorrido del Usuario

| Etapa | Recorrido ACTUAL (Sin DSS) 🔴 | Recorrido IDEAL (Con DSS) 🟢 |
|---|---|---|
| **Planificación de rutas** | El despachador llega temprano, dibuja rutas en la pizarra y las copia a Excel. El proceso toma 2-3 horas y depende del criterio personal. Errores frecuentes por olvidos o duplicación. | El sistema analiza los pedidos del día, aplica un algoritmo de optimización y genera las rutas en menos de 5 minutos. El despachador solo revisa y aprueba con un clic. |
| **Asignación de conductores** | El despachador asigna camiones sin criterio objetivo, sin conocer el historial de eficiencia de cada conductor. Sin registro de quién realizó cada ruta. | El DSS sugiere la asignación según historial de eficiencia, disponibilidad y tipo de ruta. Toda asignación queda registrada automáticamente. |
| **Monitoreo durante la jornada** | El gerente no sabe dónde están los camiones. Si hay un problema, el conductor llama al despacho. La respuesta es lenta y sin información. | El gerente visualiza en mapa en tiempo real la posición de cada camión. Recibe alertas automáticas ante desvíos o retrasos. Puede reasignar pedidos desde el panel. |
| **Atención al cliente** | El cliente llama al teléfono de despacho para preguntar por su pedido. Los despachadores atienden hasta 40 llamadas/día, ocupando 4 horas de su jornada. | El cliente recibe notificación automática cuando su pedido sale a despacho y otra cuando está a 15 minutos de llegar. Consulta el estado en tiempo real desde el portal sin contactar a nadie. |
| **Cierre y análisis del día** | Sin registro formal de lo ocurrido. No se sabe cuántas entregas llegaron a tiempo, cuánto combustible se gastó ni qué conductores fueron más eficientes. | El DSS genera automáticamente un reporte del día: entregas completadas, tardías, consumo de combustible por ruta y KPI de eficiencia por conductor. El gerente lo revisa en 10 minutos. |

---

## 🗺️ Canvas MVP

### Propuesta de Valor
Proveer a FlashLogistics un DSS que otorgue visibilidad total de su operación logística: rutas optimizadas automáticamente, flota monitoreable en tiempo real, clientes informados sin intervención humana y gerencia equipada con KPIs para decidir con datos. Resultado: menos costos, menos errores, más contratos.

### Usuarios Objetivo
| Usuario | Necesidad principal |
|---|---|
| Gerente de Operaciones | Visibilidad y control total de la flota y los KPIs del negocio |
| Despachador | Planificar rutas rápidamente y dejar de atender llamadas de estado |
| Conductor | Recibir su ruta del día de forma clara y reportar incidentes fácilmente |
| Cliente | Saber el estado de su pedido sin tener que llamar a nadie |

### Funcionalidades MVP vs. Fuera del MVP

| MVP ✅ (Mínimo para entregar valor) | Fuera del MVP 🔜 (Versión futura) |
|---|---|
| Optimización automática de rutas (algoritmo base) | Integración con ERP o sistema de inventario |
| Tracking GPS en tiempo real de la flota | App móvil nativa para conductores |
| Portal de seguimiento de pedidos para el cliente | Predicción de demanda con inteligencia artificial |
| Notificaciones automáticas por correo al cliente | Notificaciones por WhatsApp o SMS |
| Dashboard con KPIs: entregas, combustible, conductores | Módulo de mantenimiento de flota |
| Histórico operativo y reportes del día | Multi-empresa o multi-depósito |

### Métricas de Éxito (KPIs)

| KPI | Estado Actual | Meta al Sprint 3 |
|---|---|---|
| Tasa de entregas a tiempo | 70% | ≥ 85% |
| Costo de combustible | Referencia semestral | -10% |
| Llamadas de estado atendidas/día | ~40 llamadas | ≤ 8 llamadas (-80%) |
| Tiempo de planificación de rutas | ~2.5 horas/día | < 15 minutos |

### Cronograma Estimado

| Sprint | Semanas | Módulos | Entregable |
|---|---|---|---|
| **Sprint 1** | 1 – 4 | Módulo 1: Optimización de Rutas | Motor de cálculo de rutas + interfaz de planificación funcional |
| **Sprint 2** | 5 – 8 | Módulo 2: Tracking GPS + Módulo 3: Portal de Pedidos | Mapa de flota en tiempo real + portal de seguimiento con notificaciones |
| **Sprint 3** | 9 – 12 | Módulo 4: Dashboard de Analytics | Panel gerencial con KPIs en vivo + reportes diarios + MVP validado |

---

## ⚙️ Módulos del Sistema

### 🗺️ Módulo 1 – Optimización de Rutas
Motor de cálculo automático de rutas con criterios de distancia, tiempo, prioridad de entrega y capacidad del vehículo. Reemplaza la planificación manual en pizarra y Excel.  
**Resuelve:** CR1 — Planificación manual de rutas

### 📍 Módulo 2 – Tracking GPS en Tiempo Real
Mapa digital con ubicación en vivo de cada camión de la flota. Alertas automáticas ante desvíos o retrasos. Permite al gerente tomar decisiones operativas inmediatas.  
**Resuelve:** CR2 — Ausencia de monitoreo en tiempo real

### 📲 Módulo 3 – Portal de Seguimiento de Pedidos
Interfaz web para que el cliente consulte el estado de su pedido 24/7. Notificaciones automáticas por correo al despachar y al acercarse la entrega.  
**Resuelve:** CR3 — Comunicación ineficiente con el cliente

### 📊 Módulo 4 – Dashboard de Analytics e Indicadores
Panel gerencial con KPIs: eficiencia por conductor, rutas críticas, tasa de cumplimiento de entregas, consumo de combustible por ruta y tendencias históricas.  
**Resuelve:** CR4 — Inexistencia de datos e indicadores

---

## 🌱 Impacto en los ODS

| ODS | Problema actual que afecta al ODS | Cómo el DSS aporta al ODS |
|---|---|---|
| **ODS 8** – Trabajo decente y crecimiento económico | El equipo trabaja bajo presión constante con tareas manuales repetitivas que generan fatiga cognitiva y limitan el crecimiento de la empresa | Al automatizar la planificación y la comunicación con el cliente, el DSS elimina tareas de bajo valor. El equipo se enfoca en trabajo significativo, mejorando condiciones laborales. La empresa puede escalar sin sobrecargar al personal. |
| **ODS 9** – Industria, innovación e infraestructura | FlashLogistics opera con infraestructura tecnológica obsoleta (Excel, pizarra, teléfono), lo que frena la innovación y limita su competitividad | El DSS moderniza la infraestructura logística con tecnología de optimización, tracking en tiempo real y análisis de datos, contribuyendo al desarrollo de una industria logística más eficiente e innovadora. |

---

# Product Backlog — FlashLogistics DSS (Historias de Usuario

### Actividad Práctica 3: Product Backlog Building (PBB) · Sistemas de Información II · UPDS



---


| ID | Épica Relacionada | Historia de Usuario (Rol + Acción + Valor) | Criterios de Aceptación (Mínimo 2) | Prioridad |
| :---: | :--- | :--- | :--- | :---: |
| **HU01** | 🟦 `Epic: Data` | Como **despachadora**, quiero importar pedidos diarios vía archivo CSV, para evitar la carga manual en Excel y reducir errores de digitación. | <ul><li>[ ] El sistema valida el formato CSV y rechaza archivos con columnas incorrectas mostrando el error específico.</li><li>[ ] Se muestra un log con el total de registros importados, exitosos y fallidos.</li></ul> | 🔴 **Alta** |
| **HU02** | 🟦 `Epic: Data` | Como **despachadora**, quiero registrar manualmente un nuevo pedido con datos de cliente, dirección y producto, para cubrir pedidos de última hora no incluidos en el CSV. | <ul><li>[ ] El formulario valida campos obligatorios (cliente, dirección, producto, cantidad) y no permite guardar si están vacíos.</li><li>[ ] El pedido registrado aparece inmediatamente en la lista de pendientes del día.</li></ul> | 🔴 **Alta** |
| **HU03** | 🟦 `Epic: Data` | Como **gerente de operaciones**, quiero consultar el historial de pedidos por fecha y estado (entregado/fallido/pendiente), para tener trazabilidad de las operaciones pasadas. | <ul><li>[ ] El sistema permite filtrar por rango de fechas y por estado de entrega.</li><li>[ ] Los resultados se paginan en grupos de 20 registros y muestran el total encontrado.</li></ul> | 🟡 **Media** |
| **HU04** | 🟪 `Epic: Routing` | Como **gerente de operaciones**, quiero que el sistema calcule automáticamente la ruta óptima para cada camión al inicio del día, para eliminar la planificación manual en pizarra y reducir las entregas tardías. | <ul><li>[ ] El algoritmo considera capacidad del camión, zona geográfica y prioridad de pedido para asignar rutas.</li><li>[ ] El resultado se presenta en un mapa digital con la secuencia de paradas antes de las 7:15 am.</li></ul> | 🔴 **Alta** |
| **HU05** | 🟪 `Epic: Routing` | Como **gerente de operaciones**, quiero ver el costo estimado de combustible por ruta antes de aprobarla, para decidir si el despacho es rentable. | <ul><li>[ ] El cálculo de costo se muestra automáticamente en el dashboard de rutas antes de la aprobación.</li><li>[ ] El sistema genera una alerta visual si el costo estimado supera el presupuesto diario configurado.</li></ul> | 🔴 **Alta** |
| **HU06** | 🟪 `Epic: Routing` | Como **despachadora**, quiero reconfigurar la ruta de un camión ante la cancelación de un pedido, para no enviar al conductor a una dirección innecesaria. | <ul><li>[ ] Al cancelar un pedido, el sistema recalcula la ruta del camión afectado y actualiza la secuencia de paradas.</li><li>[ ] El conductor recibe la ruta actualizada en su app en menos de 2 minutos tras la cancelación.</li></ul> | 🟡 **Media** |
| **HU07** | 🔷 `Epic: GPS` | Como **gerente de operaciones**, quiero ver en un mapa en tiempo real la ubicación de cada camión de la flota, para tomar decisiones operativas inmediatas ante cualquier incidencia. | <ul><li>[ ] El mapa se actualiza con la posición de cada camión cada 30 segundos sin necesidad de recargar la página.</li><li>[ ] Cada camión se muestra con su código e ícono de estado (en ruta, detenido, con retraso).</li></ul> | 🔴 **Alta** |
| **HU08** | 🔷 `Epic: GPS` | Como **gerente de operaciones**, quiero recibir alertas automáticas cuando un camión lleva más de 15 minutos de retraso sobre el ETA estimado, para tomar acciones correctivas antes de que el cliente se comunique. | <ul><li>[ ] La alerta se muestra en el dashboard y envía notificación push al gerente cuando el retraso supera los 15 minutos.</li><li>[ ] La alerta incluye nombre del conductor, pedido afectado y nueva hora estimada de llegada calculada por el sistema.</li></ul> | 🔴 **Alta** |
| **HU09** | 🟩 `Epic: Portal` | Como **cliente minorista**, quiero consultar el estado de mi pedido en tiempo real desde un portal web sin necesidad de llamar al despachador, para planificar mi jornada con certeza. | <ul><li>[ ] El portal permite buscar un pedido por número de pedido o RUC del cliente sin necesidad de crear una cuenta.</li><li>[ ] Se muestra el estado actual (despachado / en ruta / entregado) y la hora estimada de llegada actualizada.</li></ul> | 🔴 **Alta** |
| **HU10** | 🟩 `Epic: Portal` | Como **cliente minorista**, quiero recibir una notificación automática por SMS o email cuando mi pedido salga del almacén y cuando esté a 30 minutos de llegar, para no tener que consultar el portal manualmente. | <ul><li>[ ] El sistema envía un SMS/email al salir el camión con el número de pedido y rango horario estimado de entrega.</li><li>[ ] Se envía una segunda notificación cuando el camión está a 30 minutos o menos de la dirección de entrega.</li></ul> | 🔴 **Alta** |
| **HU11** | 🟧 `Epic: Analytics` | Como **gerente de operaciones**, quiero ver un dashboard con los KPIs principales del día (% entregas a tiempo, consumo de combustible, eficiencia por conductor), para tomar decisiones basadas en datos sin construir reportes en Excel. | <ul><li>[ ] El dashboard muestra mínimo 5 KPIs en tiempo real: % entregas a tiempo, combustible consumido, pedidos entregados/fallidos, tiempo promedio por ruta y ranking de conductores.</li><li>[ ] Los gráficos se actualizan automáticamente al cierre de cada entrega sin necesidad de recargar la página.</li></ul> | 🔴 **Alta** |
| **HU12** | 🟧 `Epic: Analytics` | Como **gerente de operaciones**, quiero exportar el reporte de desempeño semanal en formato PDF o Excel, para compartirlo con la dirección de la empresa en reuniones de gestión. | <ul><li>[ ] El reporte exportado incluye los mismos KPIs del dashboard para el rango de fechas seleccionado.</li><li>[ ] El archivo se genera y descarga en menos de 10 segundos para rangos de hasta 30 días de datos.</li></ul> | 🟡 **Media** |

---

## 🏷️ Guía de Configuración de Labels (Etiquetas) en GitHub

Para mapear correctamente el Backlog con los tableros de GitHub, se recomienda configurar las siguientes etiquetas en la sección **Issues ➔ Labels ➔ New Label**:

| Nombre de Etiqueta | Color Hexadecimal | Módulo / Épica |
| :--- | :---: | :--- |
| `Epic: Data` | `#2E75B6` | Gestión de Datos |
| `Epic: Routing` | `#7030A0` | Motor de Cálculo |
| `Epic: GPS` | `#0070C0` | Tracking GPS |
| `Epic: Portal` | `#00B050` | Portal Cliente |
| `Epic: Analytics` | `#C55A11` | Dashboard Analytics |

---
