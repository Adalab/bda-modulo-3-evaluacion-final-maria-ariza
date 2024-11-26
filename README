# EVALUACIÓN MODULO 3 - Análisis de Datos de una Aerolínea #

## Descripción del Proyecto ##

Este proyecto tiene como objetivo realizar un análisis detallado de los datos relacionados con el comportamiento de los clientes dentro de un programa de lealtad de una aerolínea. Se trabajará con dos conjuntos de archivos que contienen información sobre la actividad de vuelo de los clientes y su perfil demográfico. Utilizando herramientas de exploración de datos, limpieza, visualización y pruebas estadísticas, se busca obtener insights valiosos sobre cómo los clientes interactúan con el programa y cómo sus características influyen en su comportamiento.

## Requisitos Previos ##

**Archivos de Datos**:
- **Customer Flight Analysis.csv**: Contiene información sobre la actividad de vuelo de los clientes, incluyendo vuelos reservados, distancia volada, puntos acumulados/redimidos y costos asociados.
- **Customer Loyalty History.csv**: Incluye detalles demográficos y de perfil de los clientes, como género, educación, ubicación, tipo de tarjeta de lealtad, y valor que aporta el cliente a la empresa (CLV).

**Herramientas necesarias**:
- Python 3.12
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Sklearn (para imputación de nulos)
- Scipy (para pruebas estadísticas)

## Estructura del Proyecto ##

El proyecto se estructura en varias fases:

### Fase 1: Exploración y Limpieza de Datos
- **Exploración Inicial**: Carga y exploración de los datos para identificar problemas (valores nulos, atípicos, datos faltantes).
- **Limpieza de Datos**: Tratamiento de los valores nulos y corrección de inconsistencias para asegurar que los datos estén listos para el análisis.

### Fase 2: Visualización de Datos
En esta fase, se utilizan herramientas de visualización para responder a diversas preguntas, tales como:
- ¿Cómo se distribuye la cantidad de vuelos reservados por mes durante el año?
- ¿Existe una relación entre la distancia volada y los puntos acumulados por los clientes?
- ¿Cómo se distribuyen los clientes por provincia o estado?
- ¿Cuál es la comparación del salario promedio entre los diferentes niveles educativos?
- ¿Cuál es la proporción de clientes con diferentes tipos de tarjetas de fidelidad?
- ¿Cómo se distribuyen los clientes según su estado civil y género?

### Fase 3 - Evaluación de Diferencias en Reservas de Vuelos por Nivel Educativo
- **Preparación de Datos**: Filtrar el conjunto de datos para trabajar solo con las columnas 'Flights Booked' y 'Education'.
- **Análisis Descriptivo**: Agrupar los datos por nivel educativo y calcular estadísticas descriptivas.
- **Prueba Estadística**: Realizar una prueba de hipótesis para determinar si existen diferencias significativas en el número de vuelos reservados entre los diferentes niveles educativos.

## Ejemplo de Análisis ##

Para ilustrar un análisis básico, se puede analizar la distribución de vuelos reservados por mes en el año. Utilizando la librería `matplotlib`, se puede generar un gráfico de barras que muestre cómo varía la cantidad de vuelos reservados mes a mes.

### Código para Visualización de Distribución de Vuelos por Mes:

```python
import pandas as pd
import matplotlib.pyplot as plt

# Cargar los datos
flight_data = pd.read_csv('Customer Flight Analysis.csv')

# Agrupar los datos por año y mes
monthly_flights = flight_data.groupby(['Year', 'Month'])['Flights Booked'].sum().reset_index()

# Crear el gráfico
plt.figure(figsize=(10, 6))
plt.bar(monthly_flights['Month'], monthly_flights['Flights Booked'], color='skyblue')
plt.xlabel('Mes')
plt.ylabel('Vuelos Reservados')
plt.title('Distribución de Vuelos Reservados por Mes')
plt.xticks(range(1, 13))
plt.show()
```

### Descripción del Análisis

Agrupación de Datos:

- Se agrupan los datos por año y mes para obtener la suma de los vuelos reservados en cada periodo.

Visualización:

- Se utiliza un gráfico de barras para mostrar cómo varía la cantidad de vuelos reservados mes a mes.

Este análisis básico ilustra cómo usar Pandas para agrupar datos y matplotlib para crear una visualización simple y efectiva.

## Instalación y Configuración

1. Clona el repositorio:
```
git clone https://github.com/usuario/proyecto-programa-lealtad-aerolinea.git
cd proyecto-programa-lealtad-aerolinea
```

2. Instala las dependencias necesarias:
```
pip install -r requirements.txt
```
3. Ya puedes ejecutar el análisis y ver las visualizaciones desde el jupyter main.ipynb

