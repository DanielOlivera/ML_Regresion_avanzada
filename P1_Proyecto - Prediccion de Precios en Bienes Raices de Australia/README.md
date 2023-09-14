# Predicción de Precios de Bienes Raíces en Australia - Regresión Avanzada

## Índice

- [Índice](#índice)
- [Introducción](#introducción)
  - [Métodos Utilizados](#métodos-utilizados)
  - [Tecnologías](#tecnologías)
- [Descarga y Configuración](#descarga-y-configuración)
  - [Requisitos Previos](#requisitos-previos)
  - [Cómo Ejecutar](#cómo-ejecutar)
- [Declaración del Problema](#declaración-del-problema)
  - [Objetivo Comercial](#objetivo-comercial)
  - [Preparación de Datos:](#preparación-de-datos)
  - [Construcción y Evaluación del Modelo](#construcción-y-evaluación-del-modelo)
  - [Conclusiones](#conclusiones)
	- [Regresión Ridge](#regresión-ridge)
	- [Regresión Lasso](#regresión-lasso)
	- [Regresión ElasticNet](#regresión-lasso)
	- [Las Variables Más Significativas Son:](#las-variables-más-significativas-son)

## Introducción

El presente proyecto tiene como objetivo el análisis, limpieza y generación de modelos de regresión para un dataset que contiene datos relacionados a la compra y venta de casas en Australia, con el fin de predecir el precio de venta de las viviendas según sus características.

### Métodos Utilizados
* Entendimiento de los datos
* Eliminación de columnas
* Tratamiento de valores nulos
* Gráficas de barras, diagramas de caja e lineales para la análisis de los datos


### Tecnologías
* Python
* Pandas
* Seaborn
* Matplotlib

## Descarga y Configuración
### Requisitos Previos

Este proyecto necesita que Anaconda esté instalado en la computadora.

Para más detalles sobre la instalación, visite: https://docs.anaconda.com/anaconda/install/index.html

### Cómo Ejecutar

Puede descargar el código fuente clonando este repositorio usando Git:

1. Abra su aplicación Terminal favorita (Unix, Linux o Macos), como Terminal, Comando, Consola, iTerm2, etc.

2. Clone el repositorio

```
git clone <GITHUB_REPO_URL>
```

3. Abra el archivo notebook ** *.ipynb** en Anaconda.

```
jupyter notebook <FILE.ipynb
```


## Declaración del Problema

¿Cómo se puede aplicar técnicas de Machine Learninig para predecir precios de venta de viviendas en Australia según sus características y determinar las variables más relevantes?

### Objetivo Comercial

Encontrar el mejor modelo de regresión entre Lasso, Ridge y ElasticNet, para la predicción de precios de venta de viviendas según determinadas características.

### Preparación de Datos:

1. Limpieza de Datos y Análisis de Datos Faltantes.
2. Análisis y Tratamiento de Valores Atípicos.
3. Derivación de Columnas Categóricas.
4. Análisis Univariable.
5. Análisis Bivariable.
6. Análisis Multivariable.

### Construcción y Evaluación del Modelo

1. División de datos de entrenamiento y prueba.
2. Escalado de Características - StandardScaler.
3. Ingeniería y Selección de Características usando RFE y el Factor de Inflación de Varianza.
4. Preparación del modelo usando OLS & Regresión Lineal.
5. Modelos de Regularización Ridge, Lasso y ElasticNet.
6. Análisis de Residuos.
7. Evaluación y Valoración del Modelo.
8. Predicción.
9. Conclusión y Análisis Final.

### Conclusiones


Score for Ridge regresion: 0.8721780748067949
Score for Lasso regresion: 0.8722363899163617
Score for ElasticNet regresion: 0.8718120987353056

#### Ridge Regression
* **Optimal Lambda Value:** 90.11018251665037
* **R2 Score Train:**  0.8346514492251512
* **R2 Test Score:**  0.8721780748067949
* **RMSE Test:**   27241.12916822731

#### Lasso Regression
* **Optimal Lambda Value:** 1000.0
* **R2 Score Train:**  0.8267222096674578
* **R2 Test Score:**   0.8722363899163617
* **RMSE Test:**   	27234.914465014273

#### ElasticNet Regression
* **Optimal Lambda Value:** 0.10353218432956658
* **R2 Score Train:**  0.8349606293848901
* **R2 Test Score:**   0.8718120987353056
* **RMSE Test:**   	27280.099303630144

#### Las Variables Más Significativas Son:
* ...'Street', 
* ...'LandSlope', 
* ...'OverallQual',
* ...'ExterQual',
* ... 'GarageCars'

