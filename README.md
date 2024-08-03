Documentación de la Calculadora en Python
Índice
Introducción
Requisitos
Instalación
Desarrollo de la Calculadora
Calculadora Básica
Mejoras Realizadas
Funciones Implementadas
Uso de la Calculadora
Creación de un Ejecutable
Características Futuras
Agradecimientos
Introducción
Esta es una calculadora interactiva desarrollada en Python utilizando la biblioteca Tkinter para la interfaz gráfica. La aplicación se ha ido mejorando progresivamente, comenzando con funciones básicas de cálculo y evolucionando hacia una herramienta más robusta y con funcionalidades avanzadas.

Requisitos
Python 3.8 o superior
Tkinter (incluido por defecto con Python)
PyInstaller (para crear un ejecutable)
Instalación
Instalar Python: Descargue e instale Python si aún no lo ha hecho. Asegúrese de marcar "Add Python to PATH" durante la instalación.

Instalar los requisitos:
Abrir una terminal y ejecutar:

bash

pip install pyinstaller
Desarrollo de la Calculadora
Calculadora Básica
La calculadora comenzó con funciones aritméticas elementales: suma, resta, multiplicación y división. Así se configuró inicialmente:

python

def sumar(x, y):
    return x + y

def restar(x, y):
    return x - y

def multiplicar(x, y):
    return x * y

def dividir(x, y):
    if y != 0:
        return x / y
    else:
        return "Error: División por cero."
Mejoras Realizadas
A medida que se fue desarrollando el proyecto, se implementaron varias mejoras:

Interfaz Gráfica: Se utilizó Tkinter para crear una interfaz gráfica de usuario (GUI) intuitiva y atractiva.

Funciones Avanzadas:

Seno, coseno y tangente.
Raíz cuadrada y factorial.
Funciones de memoria: M+, MR, y MC.
Historial de Operaciones: Se implementó un sistema que permite ver las operaciones anteriores y guardarlas en un archivo.

Funciones Implementadas
Funciones básicas de cálculo: Suma, resta, multiplicación y división.
Funciones avanzadas:
Trigonométricas: seno, coseno, y tangente.
Cálculo de raíz cuadrada y factorial.
Cálculo de porcentaje.
Funciones de memoria:
M+: Sumar el número actual a la memoria.
MR: Recuperar el número de la memoria.
MC: Limpiar la memoria.
Historial de operaciones: Mostrar un historial de las operaciones realizadas.
Uso de la Calculadora
Ejecutar el archivo calculadora_gui.py desde la terminal:

bash

python calculadora_gui.py
Realizar operaciones ingresando números y presionando los botones correspondientes en la interfaz.

Usar los botones de memoria según sea necesario para almacenar o recuperar resultados.

Consultar el historial de operaciones con el botón “Historial” para ver resultados anteriores.

Creación de un Ejecutable
Para empaquetar la calculadora y crear un ejecutable que se pueda distribuir sin necesidad de tener Python instalado:

Navega a la carpeta que contiene el archivo calculadora_gui.py.

Ejecuta el siguiente comando:

bash

pyinstaller --onefile --windowed calculadora_gui.py
Encontrarás el ejecutable en la carpeta dist.

Características Futuras
Estadísticas: Agregar cálculos para media, mediana, y desviación estándar.
Modo científico: Más funciones científicas.
Tema personalizable: Permitir a los usuarios elegir temas de color para la interfaz.
Función de gráficos: Mostrar gráficos básicos para ciertos cálculos.
Agradecimientos
Agradezco a la comunidad de Python y a todos los recursos en línea que facilitaron el aprendizaje y desarrollo de esta calculadora.
