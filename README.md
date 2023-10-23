# Calculadora Clase

# Documentación de la Calculadora Simple

Esta documentación proporciona información sobre cómo instalar y utilizar la aplicación de calculadora simple desde la terminal de línea de comandos.

## Instalación

La calculadora simple no requiere una instalación especial. Solo necesitas asegurarte de tener Python instalado en tu sistema. 
Asegurate de tener instalado el sistema de contenedores docker y la herramienta de visualización de código VisualStudio

[Ir a la sección **Código**](#código)

Puedes verificar si tienes Python instalado ejecutando el siguiente comando en tu terminal:
## python --version
Si Python no está instalado, puedes descargarlo desde el sitio oficial de Python: Descargar Python.
```bash
Requisitos Mínimos
Los requisitos mínimos para ejecutar la calculadora simple son:

Python 3.x
Terminal de línea de comandos
Iniciar la Calculadora
Para iniciar la calculadora, sigue estos pasos:

Abre una terminal de línea de comandos en tu sistema.
Navega al directorio donde se encuentra el archivo de la calculadora.
Ejecuta el archivo Python con el siguiente comando:

python calculadora.py

Uso de la Calculadora
Una vez que hayas iniciado la calculadora, podrás realizar operaciones matemáticas básicas. Sigue las instrucciones en la terminal para ingresar los números y seleccionar la operación deseada. Puedes realizar sumas, restas, multiplicaciones y divisiones.

La aplicación maneja casos de error, como la división por cero, y te proporcionará el resultado de la operación en la terminal.
```
## Ejecutar la calculadora:
Para ejecutar la calculadora abre el archivo llamado Calculadora.py y ejecuta el código en el boton de ejecutar.


```
Ejemplo
A continuación, se muestra un ejemplo de cómo se vería la ejecución de la calculadora:

Calculadora Simple
Ingrese el primer número: 10
Ingrese el segundo número: 5
Operaciones disponibles:
1. Suma
2. Resta
3. Multiplicación
4. División
Seleccione la operación (1/2/3/4): 1
Resultado: 15.0
Contenedor (Opcional)
No es necesario utilizar un contenedor para ejecutar esta aplicación, ya que Python es un lenguaje de programación ampliamente utilizado y no requiere entornos de ejecución especiales.

Contribuciones
Si deseas contribuir o mejorar la calculadora simple, puedes clonar el repositorio en GitHub: Repositorio de la Calculadora Simple y enviar solicitudes de extracción.

¡Disfruta utilizando la calculadora simple!


Reemplaza `calculadora.py` con el nombre de tu archivo si es diferente. Además, asegúrate de proporcionar el enlace a una imagen de la calculadora si deseas agregar una imagen a la documentación.
```
## Código
```
# Función para realizar la suma de dos números
def suma(num1, num2):
    return num1 + num2
```

```
# Función para realizar la resta de dos números
def resta(num1, num2):
    return num1 - num2
```

```
# Función para realizar la multiplicación de dos números
def multiplicacion(num1, num2):
    return num1 * num2
```

```
# Función para realizar la división de dos números
def division(num1, num2):
    if num2 == 0:
        return "Error: No se puede dividir por cero"
    return num1 / num2
```

```
# Función principal de la calculadora
def calculadora():
    print("Calculadora Simple")
    try:
        num1 = float(input("Ingrese el primer número: "))
        num2 = float(input("Ingrese el segundo número: "))
        print("Operaciones disponibles:")
        print("1. Suma")
        print("2. Resta")
        print("3. Multiplicación")
        print("4. División")
        operacion = input("Seleccione la operación (1/2/3/4): ")
        
        if operacion not in ["1", "2", "3", "4"]:
            print("Opción no válida")
        else:
            if operacion == "1":
                resultado = suma(num1, num2)
            elif operacion == "2":
                resultado = resta(num1, num2)
            elif operacion == "3":
                resultado = multiplicacion(num1, num2)
            else:
                resultado = division(num1, num2)
            
            print("Resultado: ", resultado)
    except ValueError:
        print("Error: Ingrese números válidos")

    if __name__ == "__main__":
    calculadora()
```
