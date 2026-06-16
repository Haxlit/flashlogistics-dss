# Formulario de Refinamiento y Definition of Ready (DoR)

## 📌 Introducción a la Definition of Ready (DoR)

La **Definition of Ready (DoR)** es el estándar de calidad y la directriz técnica que establece el Squad para determinar cuándo una Historia de Usuario (HU) está suficientemente madura, comprendida y preparada para ser integrada y programada dentro de un Sprint. Su propósito fundamental es mitigar el riesgo técnico, previniendo el inicio del desarrollo sobre bases ambiguas, especificaciones incompletas o arquitecturas técnicamente inviables que degraden la velocidad de entrega del equipo (*velocity*) o comprometan la calidad del producto final.

A diferencia de la *Definition of Done (DoD)*, que valida la finalización y el despliegue del incremento, la **DoR actúa como una compuerta de calidad de entrada al Sprint**. Si una Historia de Usuario no satisface la totalidad de los criterios establecidos, el Squad tiene la responsabilidad explícita de mantenerla en refinamiento, rechazando su compromiso en el Sprint Planning hasta que la incertidumbre haya sido resuelta.

---

## 📑 DoR — Definition of Ready (Checklist Completo)

Para que una Historia de Usuario sea considerada oficialmente **LISTA (Ready)** y califique para ingresar al *Sprint Planning*, debe satisfacer obligatoriamente y sin excepciones cada uno de los criterios listados a continuación. El *Scrum Master*, el *Product Owner* y el equipo de desarrollo verifican este checklist de manera estricta durante las sesiones de **Backlog Refinement**.

| Estado | Criterio de Aceptación Técnica | Categoría | Responsable Principal |
| :---: | :--- | :---: | :--- |
| **[ ]** | **Redacción Estándar e Impacto**<br>La historia está estructurada formalmente: `Como [Rol/Actor]`, `quiero [Acción/Funcionalidad]` `para [Valor de Negocio]`. El rol y el valor de negocio están claramente diferenciados y justifican la existencia del desarrollo. | Redacción | Product Owner |
| **[ ]** | **Criterios de Aceptación (CA) Verificables**<br>La historia cuenta con un mínimo de 2 Criterios de Aceptación concretos, medibles y automatizables mediante pruebas. Los CA deben estar redactados estrictamente bajo el formato conductual **Dado / Cuando / Entonces** (*Given / When / Then*). | Funcionalidad | Squad + Product Owner |
| **[ ]** | **Estimación Relativa del Esfuerzo**<br>La historia ha sido estimada en *Story Points* por el equipo técnico completo utilizando la dinámica de *Planning Poker*. La estimación consensuada se encuentra registrada en el campo correspondiente del *Issue* en GitHub Projects. | Estimación | Squad (Dev Team) |
| **[ ]** | **Modelado de Casos de Uso UML**<br>Se dispone de un Diagrama de Casos de Uso UML que define con precisión los actores (primarios y sistemas secundarios) y los casos de uso involucrados, documentando explícitamente las relaciones de inclusión (`<<include>>`) y extensión (`<<extend>>`). | Modelado UML | Arquitecto de Software |
| **[ ]** | **Modelado de Secuencia y Arquitectura**<br>Existe un Diagrama de Secuencia UML que describe el flujo completo de mensajes entre objetos del sistema, respetando el patrón de arquitectura por capas: `Interfaz/Cliente` ➔ `Controlador` ➔ `Servicio` ➔ `Repositorio` ➔ `Base de Datos`. | Modelado UML | Arquitecto de Software |
| **[ ]** | **Modelado y Persistencia de Datos**<br>Las entidades de datos requeridas están mapeadas (tablas, atributos clave, llaves primarias/foráneas y relaciones). Se ha verificado que el esquema actual de la base de datos soporta el desarrollo o que los cambios requeridos no bloquean la iteración. | Datos / BD | DBA / Desarrollador |
| **[ ]** | **Gestión de Excepciones y Robustez (ISO 25010)**<br>Los flujos alternativos, escenarios de error y excepciones críticas han sido identificados, nombrados y documentados formalmente tanto en el Diagrama de Secuencia como en los Criterios de Aceptación. El equipo conoce la resiliencia del sistema. | Robustez | Squad (Dev Team) |
| **[ ]** | **Sustentabilidad y Enfoque Ético (ODS)**<br>Se ha documentado el impacto de la funcionalidad sobre el **ODS 8** (Trabajo Decente y Crecimiento Económico) y/o el **ODS 9** (Industria, Innovación e Infraestructura), incluyendo una justificación técnica concreta de su aporte en el código o proceso. | Ética / ODS | Squad + Product Owner |
| **[ ]** | **Análisis de Dependencias (INVEST)**<br>La historia cumple con el principio de Independencia del framework INVEST. No existen dependencias técnicas bloqueantes con tareas no finalizadas. Cualquier dependencia externa está identificada, mitigada y el orden de implementación acordado. | Independencia | Scrum Master |
| **[ ]** | **Trazabilidad y Gobierno en GitHub Projects**<br>El *Issue* en GitHub está completamente configurado: descripción limpia de la historia, Criterios de Aceptación en formato Markdown, *Story Points* asignados, el Diagrama de Secuencia incrustado (o vinculado como imagen) y la etiqueta (*label*) de la Épica asociada. | Trazabilidad | Squad (Dev Team) |

---
