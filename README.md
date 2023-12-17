# QM2515-Tarea-Nro-6
Programas de la materia de Introducción a la Quimiometría. Tarea Nro. 6
# Programa #1: Código de Análisis de la Cinética de una Reacción Química

## Descripción General

Este código está diseñado para analizar datos de una reacción química y determinar el orden de la reacción, así como calcular la constante de velocidad. Utiliza datos experimentales del cambio en la concentración de un reactivo a lo largo del tiempo y aplica una regresión lineal para hacer estas determinaciones.

## Librerías Utilizadas

- `numpy`: Para el manejo de arrays y operaciones matemáticas.
- `matplotlib.pyplot`: Para crear gráficos y visualizar los datos y resultados.
- `scipy.stats.linregress`: Para realizar la regresión lineal y obtener la ecuación de la línea de mejor ajuste.

## Funcionamiento del Código

- **Ingreso de Datos**: Se introducen los datos experimentales de tiempo y la concentración relativa del reactivo.
- **Cálculo de la Concentración Absoluta**: Se calcula la concentración absoluta del reactivo a partir de la concentración relativa y la concentración inicial.
- **Regresión Lineal**: Se realiza una regresión lineal entre el tiempo y el inverso de la concentración del reactivo.
- **Visualización de Resultados**: Se genera un gráfico para mostrar los datos experimentales y la línea de mejor ajuste, incluyendo la ecuación y el coeficiente de determinación \( R^2 \).

## Instrucciones de Uso

1. Ejecute el script para ver el gráfico generado.
2. El gráfico mostrará los datos experimentales junto con la línea de mejor ajuste.
3. La ecuación de la línea y el valor de \( R^2 \) indicarán la relación entre el tiempo y el inverso de la concentración, lo cual es clave para determinar el orden de la reacción y la constante de velocidad.

## Notas Adicionales

- Este análisis asume que la reacción es de segundo orden, basado en la linealidad entre el tiempo y el inverso de la concentración.
- La pendiente de la línea de ajuste corresponde a la constante de velocidad de la reacción.
  
# Progrma #2: Análisis del Enfriamiento de un Pastel

## Descripción General

Este código modela y analiza el proceso de enfriamiento de un pastel desde su extracción del horno hasta que alcanza la temperatura ambiente. Utiliza la ley de enfriamiento de Newton para calcular la constante de enfriamiento y determinar el tiempo necesario para que el pastel alcance una temperatura específica.

## Librerías Utilizadas

- `numpy`: Para manejo de arrays y cálculos matemáticos.
- `matplotlib.pyplot`: Para visualización de datos y creación de gráficos.
- `math`: Para operaciones matemáticas como el logaritmo.

## Funcionamiento del Código

- **Definición de Temperaturas**: Se establecen las temperaturas iniciales del pastel y del ambiente.
- **Cálculo de la Constante de Enfriamiento**: Se utiliza la ley de enfriamiento de Newton para calcular la constante `k`.
- **Función de Tiempo**: Se define una función para calcular el tiempo necesario hasta alcanzar una temperatura objetivo.
- **Cálculo de Tiempos Específicos**: Se calcula el tiempo aproximado para que el pastel alcance temperaturas cercanas a la del ambiente.
- **Visualización de Resultados**: Se genera una gráfica que muestra la curva de enfriamiento del pastel con respecto al tiempo.

## Instrucciones de Uso

1. Ejecute el script para visualizar la gráfica del proceso de enfriamiento.
2. Observe los puntos de interés marcados en la gráfica, como la temperatura inicial, la temperatura después de 3 minutos, y el tiempo estimado para alcanzar la temperatura ambiente.
3. El resultado impreso proporciona una interpretación del modelo y sus limitaciones.

## Problema Abordado

El código responde a la pregunta: "¿Cuánto tiempo le tomará al pastel enfriarse hasta la temperatura ambiente de 70º F después de ser sacado del horno con una temperatura inicial de 300° F y una temperatura de 200° F tras tres minutos?"

## Notas Adicionales

- Este modelo asume un enfriamiento asintótico hacia la temperatura ambiente.

# Programa #3: Modelo de Competencia entre Poblaciones

## Descripción General

Este código modela la competencia entre dos poblaciones a lo largo del tiempo utilizando un sistema de ecuaciones diferenciales ordinarias (ODEs). Se estudian dos casos con diferentes condiciones iniciales para analizar cómo evolucionan las poblaciones en un periodo de 200 años.

## Librerías Utilizadas

- `scipy.integrate.odeint`: Para resolver el sistema de ODEs.
- `numpy`: Para manejo de arrays y operaciones numéricas.
- `matplotlib.pyplot`: Para visualización y creación de gráficos.

## Funcionamiento del Código

- **Definición del Modelo**: Se establece un sistema de ODEs que describe la interacción entre dos poblaciones.
- **Vector de Tiempo**: Se define un vector de tiempo que abarca 200 años, dividido en 1000 puntos.
- **Condiciones Iniciales**: Se establecen dos conjuntos de condiciones iniciales, uno para cada caso de estudio.
- **Resolución de ODEs**: Se utiliza `odeint` para resolver las ecuaciones con las condiciones iniciales dadas.
- **Visualización de Resultados**: Se generan gráficos para mostrar la evolución de las poblaciones en cada caso.

## Instrucciones de Uso

1. Ejecute el script para observar cómo evolucionan las poblaciones en cada caso.
2. Los gráficos mostrarán la dinámica de las poblaciones x(t) y y(t) a lo largo del tiempo.

## Problema Abordado

El código responde al modelo de competencia definido por las ecuaciones:

- 𝑑𝑥/𝑑𝑡 = 𝑥(1−0.1𝑥−0.05𝑦)
- 𝑑𝑦/𝑑𝑡 = 𝑦(1.7−0.1𝑦−0.15𝑥)

Se analizan dos casos:
a) x(0) = 1.1, y(0) = 1
b) x(0) = 4, y(0) = 10




  
