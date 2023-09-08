# TFG_Altamira

El código pertenece al Trabajo Fin de Grado (TFG) 'Análisis de fluctuaciones térmicas no estacionales en la zona de Cruce en el interior de la cueva de Altamira'

Resumen del trabajo:
Se observaron oscilaciones diarias en la temperatura en la zona del Cruce de la cueva de Altamira. Estas no podías provenir de la condución de calor por la roca, la roca filtra las oscilaciones de alta frecuencia, dejando pasar unicamente la onda anual de temperatura. Se estudió el intercambio de aire convectivo entre el interior y el exterior de la cueva. Para ello se obtuvieron correlaciones lineales entre diferentes variables interiores y exteriores de la cueva, tanto de la zona del Cruce, como de las salas contiguas. Se relacionaron los resultados de estos coeficientes con los desfases entre las oscilaciones diarias de las variables. Se concluyó que hay intercambio de aire convectivo entre el interior y el exterior, pero no hay suficientes datos para determinar la vía preferente de entrada.


Este repositorio contiene 9 archivos Jupyter:
1. Suavizado de datos: Se suavizan los datos de interes de varios archivos excel mediante la media móvil de periodo n=5 y se añaden al excel correspondiente como nuevas columnas en el mismo excel.
2. Gráficas: Se representan las variables de interes para el estudio.
3. Preparar_datos: Contiene funciones necesarias para correr los archivos de correlaciones (los archivos cuyo nombre comienza con CCs).
4. TablaResumenCC: Contiene una función que ordena los coeficientes de correlación de los archivos de correlaciones (los archivos cuyo nombre comienza conCCs) en una tabla.
5. CCsTemperaturasCruceRamalExterior, CCsTemperaturaCruceHallExterior, CCsTemperaturasPolicromosHallCruceExterior, CCsCO2entreSalas, CCsCO2difT: Cada archivo contiene el código necesario para obtener los coeficientes de correlación entre diversos pares de variables, agrupando los datos disponibles por semanas previamente. Desde estos archivos se llama a funciones definidas en 'Preparar_datos.ipynb' y 'TablaResumenCC.ipynb'.
