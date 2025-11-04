# 🛍️ Alura Store – Análisis de Ventas

Este proyecto forma parte del **Challenge de Data Science de Alura Latam**.  
El objetivo es realizar un **análisis exploratorio y comparativo de las ventas de diferentes tiendas**, identificando patrones, productos más vendidos y posibles oportunidades de mejora.

---

## 🎯 Propósito del análisis

El propósito principal de este análisis fue **comprender el desempeño comercial de la cadena de tiendas Alura Store**, a través de la limpieza, consolidación y exploración de los datos disponibles.

Se buscó responder preguntas como:
- ¿Qué tienda tuvo el mejor rendimiento en ventas?
- ¿Cuáles fueron los productos más y menos vendidos?
- ¿Existen patrones de consumo entre las distintas tiendas?

Para ello, se desarrolló un proceso automatizado de análisis y visualización de los datos.

---

## 🧱 Estructura del proyecto

El repositorio está organizado de la siguiente manera:

alura-store-desafio-analisis/
│
├── notebooks/
│ └── analisis_tienda_alura.ipynb # Notebook principal con el análisis completo
│
├── data/ # (Opcional) Carpeta para almacenar datasets locales
│
├── images/ # (Opcional) Gráficos exportados del análisis
│
└── README.md # Documentación general del proyecto



### Descripción del notebook principal

El archivo `analisis_tienda_alura.ipynb` contiene:
- **Importación de datos** desde varias tiendas.  
- **Limpieza y unificación** de la información.  
- **Creación de la función `obtener_resumen_tienda()`**, que resume automáticamente los productos más y menos vendidos.  
- **Visualizaciones** para comparar resultados entre tiendas.

---

## 📊 Ejemplos de gráficos e insights

Durante el análisis se generaron distintos gráficos y conclusiones, entre ellos:

### Ejemplo 1: Ingresos Totales por Tienda

```python
ingresos = [ingreso_tienda_1, ingreso_tienda_2, ingreso_tienda_3, ingreso_tienda_4]
tiendas = ['Tienda 1', 'Tienda 2', 'Tienda 3', 'Tienda 4']

plt.figure(figsize=(8, 5))
plt.bar(tiendas, ingresos, color=['#5DADE2','#58D68D','#F5B041','#AF7AC5'])
plt.title('Ingresos Totales por Tienda')
plt.ylabel('Ingresos')
plt.grid(axis='y', linestyle='--', alpha=0.7)
plt.show()

📈 Descripción:
Un gráfico de barras que muestra las ventas totales por tienda, facilitando la comparación del rendimiento general.

Principales insights

Algunas tiendas presentan una mayor diversidad de productos vendidos, lo que sugiere mejor rotación de inventario.

La tienda con mayores ventas supera significativamente el promedio de las demás.

Los productos con menores ventas podrían estar asociados a categorías poco demandadas o estrategias de marketing menos efectivas.

⚙️ Instrucciones para ejecutar el notebook
🔹 Opción 1: En Google Colab

Haz clic aquí para abrir el notebook directamente:
https://colab.research.google.com/drive/github.com/picolacastillo/alura-store-desafio-analisis/blob/main/notebooks/analisis_tienda_alura.ipynb
