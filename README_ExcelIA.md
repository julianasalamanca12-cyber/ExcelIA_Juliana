# 🥐 Análisis de Rentabilidad de Panadería con Excel e IA

## 📌 Tema y Pregunta Clave

**Tema:** Análisis de rentabilidad de productos en una panadería artesanal

**Pregunta de investigación:**
> ¿Qué producto genera mayor ganancia en una panadería durante los primeros 10 días de marzo 2026?

---

## 📂 Fuente de Datos

- **Origen:** Dataset propio creado manualmente en Microsoft Excel
- **Período:** 1 al 10 de marzo de 2026
- **Tamaño:** 20 registros de ventas
- **Formato:** .xlsx

### Estructura del dataset

| Columna | Variable | Descripción |
|---|---|---|
| A | Fecha | Fecha de venta |
| B | Producto | Nombre del producto |
| C | Cantidad Vendida | Unidades vendidas por día |
| D | Precio Unitario | Precio de venta por unidad ($) |
| E | Ingreso Total | Cantidad × Precio unitario |
| F | Costo Unitario | Costo de producción por unidad ($) |
| G | Costo Total | Cantidad × Costo unitario |
| H | Ganancia | Ingreso Total − Costo Total |
| I | ¿Hay ganancia o pérdida? | Clasificación automática |
| J | Margen de ganancia % | Ganancia / Ingreso Total |

### Proceso de limpieza
- El dataset fue creado directamente en Excel sin valores nulos ni errores.
- Todos los campos numéricos están correctamente tipificados.
- La columna I fue generada con fórmula condicional para clasificar automáticamente ganancia o pérdida.

---

## 🤖 Funciones y Herramientas de IA Usadas

### Funciones de Excel aplicadas

| Función | Uso |
|---|---|
| `PROMEDIO.SI` | Media de ganancia por categoría |
| `DESVEST` | Variabilidad de ganancias |
| `MAX` / `MIN` | Producto más y menos rentable |
| `MIN.SI.CONJUNTO` / `MAX.SI.CONJUNTO` | Extremos filtrados por criterio |
| `INDICE` + `COINCIDIR` | Buscar nombre del producto más rentable |
| `K.ESIMO.MAYOR` | Ranking TOP 3 de ganancias |
| `BUSCARV` | Consulta de datos por producto |

### Herramientas de IA
- **Claude AI (Anthropic):** Generación de fórmulas en Excel, corrección de errores, interpretación de resultados y redacción de insights accionables.
- **Ideas en Excel:** Sugerencias automáticas de gráficos y patrones en los datos.

---

## 📊 Visualizaciones Generadas

1. **Gráfico de barras** — Ganancia por producto (ordenado de mayor a menor)
2. **Gráfico de líneas** — Tendencia de ingresos diarios del 1 al 10 de marzo

---

## ✅ Conclusiones del Análisis

1. **Todos los productos generan ganancia** — el margen promedio es del 50% sobre el ingreso total.
2. **La Torta de vainilla es el producto más rentable** con $56 de ganancia absoluta.
3. Le siguen la **Torta de chocolate** y el **Pay de manzana**, ambos con $45.
4. Las **tortas enteras** dominan en ganancia absoluta por su precio unitario elevado.
5. Los **productos pequeños** (cupcakes, galletas, donas) tienen menor ganancia unitaria pero mayor volumen de ventas, lo que los hace importantes para el flujo de caja diario.
6. Los **días 3 y 7 de marzo** registraron los mayores ingresos, coincidiendo con la venta de tortas completas.

---

## 💡 Insights Accionables

- Priorizar la **venta de tortas enteras los fines de semana** para maximizar la ganancia diaria.
- Crear **combos o promociones** de productos pequeños (ej. 3 cupcakes + café) para aumentar el ticket promedio entre semana.
- Monitorear el **margen % por producto** (columna J) para detectar si algún costo unitario sube y afecta la rentabilidad.
- Considerar aumentar la **cantidad vendida de Pay de limón** (solo 4 unidades) ya que tiene un margen del 50% con precio alto.

---

## ⚠️ Limitaciones y Recomendaciones Futuras

### Limitaciones
- El dataset cubre solo 10 días, lo que no refleja estacionalidad ni tendencias de largo plazo.
- No se consideraron costos fijos (renta, electricidad, mano de obra) — solo costos variables por producto.
- Cada producto aparece una sola vez, por lo que no hay comparación de rendimiento del mismo producto en diferentes días.

### Recomendaciones futuras
- Ampliar el dataset a **al menos 3 meses** para identificar tendencias reales.
- Incorporar **costos fijos** para calcular el punto de equilibrio real del negocio.
- Usar **tablas dinámicas** para analizar ventas por semana, por categoría de producto o por rango de precio.
- Migrar el análisis a **Python (pandas)** o **Power BI** para dashboards más dinámicos y automatizados.

---

*Análisis realizado en Microsoft Excel con apoyo de Claude AI (Anthropic).*
