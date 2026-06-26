1. **Capa de Almacenamiento (SQL Server):** Normalización de las transacciones históricas reales y metas presupuestadas asociadas a las sedes de Lima y Arequipa.
2. **Capa de Abstracción (Vistas SQL):** Desacoplamiento directo de las tablas físicas del motor para garantizar un rendimiento óptimo de refresco y consistencia de los tipos de datos.
3. **Capa Analítica (Power BI / DAX):** Estructuración bajo un diseño de **Modelo en Estrella**, implementando lógica de negocio financiera a través de una tabla dedicada única de medidas (`_Medidas Financieras`).


## El Dashboard Financiero (`Finanzas_Dashboard_P&L_v1.0.pbix`)

El reporte ejecutivo final está diseñado bajo estrictos estándares de UI/UX financieros (Paleta *Emerald Corporate*), estructurado en tres secciones críticas de decisión:

### 1. Cabecera Directiva (KPI Cards)
* **Ingresos Totales:** Monitoreo del volumen bruto de facturación consolidada de la organización ($3.50M).
* **EBITDA Efectivo:** Margen de utilidad operativa neta antes de intereses, impuestos, depreciaciones y amortizaciones ($1.54M), reflejando la salud y productividad del núcleo del negocio.
* **% de Ejecución Presupuestal:** Indicador macro formateado nativamente al **102.31%**, advirtiendo de inmediato una sobreejecución controlada frente a la meta anual planificada.

### 2. Análisis Continuo (Presupuesto vs. Ejecutado)
Un gráfico mixto de líneas y columnas agrupadas con eje de ordenadas secundario para evaluar desviaciones mes a mes:
* **Escenario de Éxito (Abril):** El monto real supera con creces la expectativa, disparando el cumplimiento al **108.53%**.
* **Escenario de Sub-ejecución (Agosto):** Caída por debajo de la meta planificada con un ratio del **91.04%**, aislando desviaciones operativas temporales.

### 3. Matriz Operativa de Auditoría (Drill-Down P&L)
Navegación jerárquica nativa (`Clase --> Categoría --> Subcategoría`) que contrasta en paralelo el Monto Real vs. Presupuesto, computando la **Desviación Presupuestal** real:
* **Principio de Signos Contables Nativos:** Los costos, gastos e inversiones de capital se almacenan y procesan con valores **negativos**. Esto optimiza el motor de cálculo DAX al permitir agregaciones directas mediante sumas matemáticas elementales en lugar de condicionales lógicos pesados, manteniendo la consistencia exacta en subtotales y totales generales.

---

## Tecnologías y Estándares Utilizados

* **Base de Datos:** SQL Server (Modelado Relacional, Vistas de Abstracción, Integridad Referencial).
* **Business Intelligence:** Power BI Desktop, DAX (Data Analysis Expressions) para modelado e inteligencia de tiempo.
* **Diseño Ejecutivo:** Estilo corporativo premium basado en contrastes limpios, alineación contable estricta y formato de datos estandarizado.

---
