# challenge-alura-store-latam
El objetivo de este proyecto es analizar los datos de ventas de las cuatro tiendas del Sr. Juan para identificar cuál de ellas presenta el menor rendimiento y debería ser vendida, liberando capital para reinvertir en las tiendas más rentables.

# AluraStore Latam — Análisis de Tiendas

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-blue)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13-teal)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-F9AB00?logo=googlecolab&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completado-brightgreen)

> **Challenge de Data Science — Alura Latam**  
> Análisis exploratorio de datos de 4 tiendas para ayudar al Sr. Juan a tomar una decisión estratégica de negocio.

---

## Descripción del Proyecto

Este proyecto forma parte del **Challenge #1 de Data Science de Alura Latam**. El objetivo es analizar los datos de ventas de las 4 tiendas del Sr. Juan para identificar cuál de ellas presenta el menor rendimiento y debería ser vendida, liberando capital para reinvertir en las tiendas más rentables.

El análisis fue realizado en **Google Colab** usando Python y las principales librerías de análisis y visualización de datos.

---

## Objetivos del Análisis

| # | Análisis | Descripción |
|---|---|---|
| 1 | **Facturación** | Ingresos totales, número de transacciones y ticket promedio por tienda |
| 2 | **Ventas por Categoría** | Qué categorías de productos generan más ingresos en cada tienda |
| 3 | **Calificación Promedio** | Satisfacción del cliente por tienda (escala 1–5) |
| 4 | **Productos más y menos vendidos** | Top 10 productos con mayor y menor demanda por tienda |
| 5 | **Costo de Envío Promedio** | Análisis del costo logístico por tienda |

---

## Estructura del Proyecto

```
alurastore-latam/
│
├── AluraStoreLatam_Completo.ipynb   # Notebook principal con todo el análisis
└── README.md                        # Este archivo
```

---

## Datos Utilizados

Los datos provienen del repositorio oficial del challenge de Alura Latam:

| Archivo | Descripción |
|---|---|
| `tienda_1.csv` | Datos de ventas — Tienda 1 |
| `tienda_2.csv` | Datos de ventas — Tienda 2 |
| `tienda_3.csv` | Datos de ventas — Tienda 3 |
| `tienda_4.csv` | Datos de ventas — Tienda 4 |

**Columnas disponibles en cada dataset:**

`Producto` · `Categoría del Producto` · `Precio` · `Costo de envío` · `Fecha de Compra` · `Vendedor` · `Lugar de Compra` · `Calificación` · `Método de pago` · `Cantidad de cuotas` · `lat` · `lon`

---

## Tecnologías y Librerías

- **Python 3.10+**
- **Pandas** — manipulación y análisis de datos
- **Matplotlib** — visualización de gráficos
- **Seaborn** — visualización estadística
- **NumPy** — cálculos numéricos y normalización
- **Google Colab** — entorno de ejecución

---

## Cómo ejecutar el proyecto

### Opción 1 — Google Colab (recomendado)

1. Abre [Google Colab](https://colab.research.google.com/)
2. Ve a **Archivo → Subir notebook**
3. Sube el archivo `AluraStoreLatam_Completo.ipynb`
4. Ejecuta todas las celdas con **Runtime → Run all**

> No es necesario instalar ninguna librería adicional. Los datos se cargan directamente desde GitHub.

### Opción 2 — Entorno local

```bash
# Clonar el repositorio
git clone https://github.com/jarangove/challenge-alura-store-latam.git
cd challenge-alura-store-latam

# Instalar dependencias
pip install pandas matplotlib seaborn numpy

# Abrir el notebook
jupyter notebook AluraStoreLatam_Completo.ipynb
```

---

## Resultados y Conclusión

Tras los cinco análisis realizados, los resultados consolidados muestran el siguiente panorama:

| Tienda | Facturación | N° Ventas | Calificación | Costo Envío | Score Global |
|---|---|---|---|---|---|
| Tienda 1 | 🟢 Mayor | 🟢 Mayor | 🟢 Alta | 🟡 Medio | 🟢 **1°** |
| Tienda 2 | 🟢 Alta | 🟢 Alta | 🟢 Alta | 🟡 Medio | 🟢 **2°** |
| Tienda 3 | 🟡 Media | 🟡 Media | 🟡 Media | 🟡 Medio | 🟡 **3°** |
| Tienda 4 | 🔴 Menor | 🔴 Menor | 🔴 Más baja | 🔴 Mayor | 🔴 **4°** |

### Recomendación final

> **La Tienda 4 es la que el Sr. Juan debería vender.**

La Tienda 4 acumula el peor desempeño en todos los indicadores clave: genera los menores ingresos, tiene el menor volumen de transacciones, registra la calificación de clientes más baja y presenta los mayores costos de envío. Esta combinación configura el escenario de menor rentabilidad y mayor riesgo operativo del portafolio.

---

## Autor

Desarrollado como parte del **Challenge de Data Science — Alura Latam**.
