# 📊 Challenge1 Data Science Latam

Este proyecto corresponde al Challenge 1 del programa Data Science Latam, donde se realiza un análisis exploratorio completo de datos de ventas de diferentes tiendas. El objetivo es comprender patrones de compra, métricas clave, desempeño relativo entre tiendas y aspectos geográficos asociados a las compras.

## 📝 Descripción General

El proyecto trabaja datos de 4 tiendas independientes y permite analizar:
- Ingresos totales por tienda
- Calificación promedio
- Costo de envío promedio
- Distribución geográfica (latitud y longitud)
- Mapas de calor y dispersión
- Comparación del rendimiento entre tiendas

## 📂 Estructura del Proyecto

.
├── data/
│   ├── tienda1.csv
│   ├── tienda2.csv
│   ├── tienda3.csv
│   └── tienda4.csv
├── src/
│   ├── analisis_ventas.py
│   ├── graficos.py
│   └── utils.py
├── notebooks/
│   └── challenge1_exploracion.ipynb
├── images/
│   ├── grafico_ingresos.png
│   ├── grafico_calificaciones.png
│   ├── grafico_costos_envio.png
│   ├── grafico_geodispersión.png
│   └── heatmap_ventas.png
├── README.md
└── requirements.txt

## 🛠️ Tecnologías Utilizadas

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Folium
- Jupyter Notebook

## 📦 Instalación

1. Clona el repositorio:  
git clone https://github.com/jgmartinezfernandez/Desafio_Trello_Tiendas

2. Entra al proyecto:  
cd challenge1-ds-latam

3. Instala dependencias:  
pip install -r requirements.txt

## 📚 Dependencias

Archivo requirements.txt recomendado:

pandas  
numpy  
matplotlib  
seaborn  
folium  
jupyter  

## ▶️ Ejecución del proyecto

Opción 1 — Script Python:  
python src/analisis_ventas.py

Opción 2 — Jupyter Notebook:  
jupyter notebook notebooks/challenge1_exploracion.ipynb

## 📊 Visualizaciones Disponibles

En la carpeta images/ se incluyen:

- grafico_ingresos.png — Ingreso total por tienda
- grafico_calificaciones.png — Calificación promedio
- grafico_costos_envio.png — Costo de envío promedio
- grafico_geodispersión.png — Distribución geográfica de ventas
- heatmap_ventas.png — Mapa de calor de densidad

## 🧠 Ejemplos del Análisis

Ingreso total:
ingreso_total = tienda['Precio'].sum()
print(f"Ingreso total: ${ingreso_total:,.0f}")

Calificación promedio:
calificacion_prom = tienda['Calificación'].mean()
print(f"Calificación promedio: {calificacion_prom:.2f}")

Mapa de dispersión:
plt.scatter(tienda['lon'], tienda['lat'], c=tienda['Precio'], cmap='viridis')

## 📈 Preguntas Analíticas Respondidas

- ¿Qué tienda obtiene mayores ingresos?
- ¿Cómo varían las calificaciones entre tiendas?
- ¿Existen zonas geográficas de alta concentración?
- ¿Cómo influye la ubicación en el costo de envío?
- ¿Se detectan patrones geoespaciales en las ventas?

## ⚠️ Problemas Comunes

Error: ModuleNotFoundError: pandas  
Solución:  
pip install pandas

Folium no muestra el mapa  
- Ajustar zoom inicial  
- Re-ejecutar la celda  

## 👤 Autor

Julio Martínez Fernández  
Challenge 1 – Data Science Latam.

## 📄 Licencia

Este proyecto se distribuye bajo la licencia MIT.

