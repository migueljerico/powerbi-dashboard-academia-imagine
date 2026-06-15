# ☕ Dashboard Ejecutivo Power BI — Academia Imagine

![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Estado](https://img.shields.io/badge/Estado-Completado-4CAF50?style=for-the-badge)
![Tipo](https://img.shields.io/badge/Práctica-Visualización%20de%20Datos-FF6B6B?style=for-the-badge)

> **Ejercicio Práctico — Análisis de Datos con Excel: Power Query, Power Pivot y Power BI.**  
> Caso de negocio: cadena de cafeterías ficticia **Academia Imagine**

---

## 📥 Descarga

[![Descargar .pbix](https://img.shields.io/badge/⬇️%20Descargar%20Dashboard-Power%20BI%20(.pbix)-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://github.com/migueljerico/powerbi-dashboard-urban-coffee/raw/main/Ejercicio_Practico_Visualizacion_Power_BI_Miguel_Jerico.pbix)

[![Ver Release v1.0](https://img.shields.io/badge/📦%20Release-v1.0-0078D4?style=for-the-badge&logo=github&logoColor=white)](https://github.com/migueljerico/powerbi-dashboard-urban-coffee/releases/tag/v1.0)

> Requiere **Microsoft Power BI Desktop** (descarga gratuita en [powerbi.microsoft.com](https://powerbi.microsoft.com/es-es/desktop/))

---

## 📋 Descripción del Proyecto

Dashboard ejecutivo desarrollado en **Microsoft Power BI Desktop** bajo un escenario ficticio como responsable de datos en una academia de formación. La secretaría nos ha entregado tres tablas en un mismo libro de Excel (Caso_Academia_Query_PowerBI.xlsx), y nos avisan de que dos de ellas vienen “sucias”: tienen errores de tecleo, formatos mezclados y alguna fila repetida, por lo que el encargo tiene dos fases:
Fase 1 (Power Query): importar las tres tablas, limpiarlas y dejarlas bien tipadas.
Fase 2 (Power BI): relacionar las tablas y construir varios gráficos para analizar las matrículas.

El objetivo principal es facilitar la **toma de decisiones estratégicas** mediante KPIs visuales e interactivos.
---

## 📁 Estructura del Repositorio

```
powerbi-dashboard-academia-imagine/
│
├── 📊 Caso_Academia_Query_PowerBI_Miguel_Jericó.pbix
│       └── Archivo Power BI Desktop con el dashboard completo
│
├── 📁 docs/
│       └── 📄 Caso_Caso_Academia_Query_PowerBI_Miguel_Jericó.pdf
│               └── Documentación técnica detallada paso a paso
│
└── 📖 README.md
```

---

## 🗂️ Modelo de Datos

El modelo estrella contiene **3 tablas relacionadas** con relaciones Muchos a Uno (*:1):

| Tabla | 
|-------|
| **Matrículas** | 
| **Cursos** | 
| **Alumnos** | 

**Relaciones:**
Matriculas es la tabla de HECHOS (en el centro); Cursos y Alumnos son DIMENSIONES. 
Dos relaciones de tipo “Uno a varios” (1 → *): el “1” en la dimensión (Alumnos, Cursos) y el “*” en Matriculas. La flecha de filtro va de la dimensión hacia Matriculas.

Alumnos → Matriculas
Alumnos[ID_Alumno] sobre Matriculas[ID_Alumno].
Cursos → Matriculas
Cursos[ID_Curso] sobre Matriculas[ID_Curso].

---

## 📊 Visualizaciones del Dashboard

| Visual | Tipo | Objetivo |
|--------|------|----------|
| 3 Tarjetas KPI | Tarjeta | Importe Total · Nº de Matrículas · Nº de Alumnos |
| Importe por categoría | Barras horizontales | Ver la categoría con mayor importe de matrícula |
| Reparto por ciudad | Gráfico de anillas | Ver la ciudad con mayor % de alumnos  |
| Importe por sexo | Gráfico de columnas agrupadas| Ver distribución de importe de matrículas según sexo  |
| Matrículas por mes | Gráfico de líneas  | Ver la evolución mensual de las matrículas |
| Matrículas por curso | Gráfico de columnas agrupadas  | Ver las matrículas por curso |


---

## 🔍 Interactividad

- **1 segmentadores** por Categoría
- Todos los gráficos se interconectan al seleccionar cualquier filtro

-  **1 marcador** implementado mediante botón de revertir
- Para eliminar los filtros aplicados.
---


## 📈 Resultados del Dashboard

| KPI | Valor |
|-----|-------|
| Importe Total | **5.867 €** |
| Número de Matrículas | **13** |
| Número de alumnos | **8** |
| Categoría líder | **Programación (1.920 €)** |
| Ciudad líder | **Valencia (22,16%)** |
| Sexo líder | **Mujer (3.256 €)** |
| Curso líder | **Excel Avanzado (4 matrículas)** |
| Período de datos | **Ene 2025 – Mar 2025** |

---

## 🧰 Tecnologías utilizadas

| Herramienta | Uso |
|---|---|
| **Microsoft Power BI Desktop** | Creación del dashboard ejecutivo |
| **Power Query** | Transformación y limpieza de datos |
| **Excel** | Fuente de datos (Caso_Academia_Query_PowerBI.xlsx) |

---

## 📚 Contexto formativo

Este ejercicio forma parte del programa de formación en **Análisis de Datos**, dentro del módulo **Análisis de Datos con Excel: Power Query, Power Pivot y Power BI**. El objetivo es desarrollar competencias en modelado de datos (modelo estrella) y diseño de dashboards ejecutivos interactivos.

**Ejercicio relacionado:** [Dashboard Ejecutivo Power BI — Urban Coffee](https://github.com/migueljerico/powerbi-dashboard-urban-coffee) — misma herramienta, otro caso de negocio.
---

<p align="center">
  <sub>Desarrollado por <a href="https://github.com/migueljerico">@migueljerico</a> · 2026</sub>
</p>
