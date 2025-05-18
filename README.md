# RETO 4
Buen día, adjunto se encuentra el archivo del reto cuatro donde se realiza la siguiente actividad:

---

### 1. Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.

```
num = int(input("Ingrese un número entero: "))
if chr(num) in ['a', 'e', 'i', 'o', 'u']:
    print(f"{num} corresponde a la vocal minúscula '{chr(num)}'")
else:
    print(f"{num} no corresponde a una vocal minúscula")
```

### 2. Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.

```
char = input("Ingrese una cadena de longitud 1: ")
if len(char) == 1:
    codigo = ord(char[0])
    if codigo % 2 == 0:
        print(f"El código ASCII de '{char}' es {codigo} y es par.")
    else:
        print(f"El código ASCII de '{char}' es {codigo} y es impar.")
else:
    print("La cadena no es de longitud 1.")
```

### 3. Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.

```
caracter = input("Ingrese un carácter: ")
if caracter.isdigit():
    print(f"'{caracter}' es un dígito.")
else:
    print(f"'{caracter}' no es un dígito.")
```

### 4. Realice un programa que lea dos números reales y determine si el primero es múltiplo del segundo.

```
a = float(input("Ingrese el primer número real: "))
b = float(input("Ingrese el segundo número real: "))
if b != 0 and a % b == 0:
    print(f"{a} es múltiplo de {b}")
else:
    print(f"{a} no es múltiplo de {b}")
```

### 5. Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:

  - Positivo: "El número x es positivo"
  - Negativo: "El número x es negativo"
  - Cero (0): "El número x es el neutro para la suma"

```
x = float(input("Ingrese un número real: "))
if x > 0:
    print(f"El número {x} es positivo")
elif x < 0:
    print(f"El número {x} es negativo")
else:
    print(f"El número {x} es el neutro para la suma")
```
  
### 6. Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.

```
cx = float(input("Ingrese la coordenada x del centro del círculo: "))
cy = float(input("Ingrese la coordenada y del centro del círculo: "))
r = float(input("Ingrese el radio del círculo: "))
px = float(input("Ingrese la coordenada x del punto: "))
py = float(input("Ingrese la coordenada y del punto: "))

distancia = ((px - cx)**2 + (py - cy)**2)**0.5
if distancia < r:
    print("El punto está dentro del círculo.")
elif distancia == r:
    print("El punto está sobre el borde del círculo.")
else:
    print("El punto está fuera del círculo.")
```

### 7. Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.

```
l1 = float(input("Ingrese la longitud 1: "))
l2 = float(input("Ingrese la longitud 2: "))
l3 = float(input("Ingrese la longitud 3: "))
if l1 + l2 > l3 and l1 + l3 > l2 and l2 + l3 > l1:
    print("Se puede construir un triángulo con esas longitudes.")
else:
    print("No se puede construir un triángulo con esas longitudes.")
```

### 8. Escriba un programa que reciba el nombre en minúsculas de un país de America y retorne la ciudad capital, si el país no pertenece al continente debe arrojar país no identificado (Utilice match-case).

```
pais = input("Ingrese el nombre del país en minúsculas: ").lower()

match pais:
    case "argentina":
        print("Buenos Aires")
    case "bolivia":
        print("Sucre")
    case "brasil":
        print("Brasilia")
    case "chile":
        print("Santiago")
    case "colombia":
        print("Bogotá")
    case "costa rica":
        print("San José")
    case "cuba":
        print("La Habana")
    case "ecuador":
        print("Quito")
    case "el salvador":
        print("San Salvador")
    case "guatemala":
        print("Ciudad de Guatemala")
    case "haití":
        print("Puerto Príncipe")
    case "honduras":
        print("Tegucigalpa")
    case "méxico" | "mexico":
        print("Ciudad de México")
    case "nicaragua":
        print("Managua")
    case "panamá":
        print("Ciudad de Panamá")
    case "paraguay":
        print("Asunción")
    case "perú" | "peru":
        print("Lima")
    case "república dominicana":
        print("Santo Domingo")
    case "uruguay":
        print("Montevideo")
    case "venezuela":
        print("Caracas")
    case _:
        print("País no identificado")

```

El reto se desarrolló en Google Colab.
#### Eso es todo, gracias.
