#La librería NumPy se usa para realizar cálculos matemáticos y científicos en Python. Es una herramienta clave para la programación científica, la ingeniería, las matemáticas y la ciencia de datos.   
#¿Qué hace NumPy? 
#1. Permite crear y manipular matrices y vectores multidimensionales
#2. Ofrece funciones matemáticas de alto nivel
#3. Es ideal para procesar grandes volúmenes de datos
#4. Permite realizar operaciones aritméticas con arreglos
#5. Es muy útil para multiplicar matrices o cuadros multidimensionales
#¿Cómo funciona NumPy? 
#1. Incorpora una nueva clase de objetos llamados arrays
#2. Permite invocar métodos de forma vectorizada
#3. Permite trabajar con una variedad de tipos POD (Plain Old Data)
#4. Se integra con C/C++ y Fortran
#¿Qué funciones tiene NumPy? 
#1. array(), zeros(), ones(), full(), arange(), numpy.mean().
#NumPy es una biblioteca de código abierto. Su nombre es la abreviatura de Numerical Python. 
#Importamos la librería Numpy con la siguiente línea de código:

import numpy as np

#Creamos una variable llamada MatrizA que almacenará los coeficientes del sistema lineal con datos reales y las variables nf y nc con datos de tipo entero

MatrizA=float()
nf=int()
nc=int()

#Cargamos los valores de la matriz de coeficientes A, desde el archivo de texto llamado coeficientes.txt, con las siguiente línea de código:

MatrizA=np.loadtxt("coeficientes.txt", dtype='int')

#Imprimimos la matriz A para verificar que fue almacenada con la siguiente línea de código

print(MatrizA)

#Desde el archivo de texto llamado orden.txt traemos el número de filas y columnas de la matriz A con las siguientes líneas de código:

nf=np.loadtxt("orden.txt", dtype='int')
nc=np.loadtxt("orden.txt", dtype='int')

#Imprimimos el orden la matriz (fila,columna), con las siguientes líneas de código:
print(nf)
print(nc)

#Cargamos lo valores de los términos independientes, con la siguiente línea de código:
Vectorb=np.loadtxt("independientes.txt", dtype='int')

#Imprimimos todo el vector de terminos independientes, con la siguiente línea de código:
print(Vectorb)

#Imprimimos un solo dato del vector de términos independientes, el que est{a ubicado en la posición 2, con la siguiente línea de código:
print(Vectorb[2])
