# 🚀 Guía completa de PSeInt

Este repositorio es una guía detallada sobre cómo usar **PSeInt**, una herramienta para aprender lógica de programación usando pseudocódigo en español.

---

## 📌 ¿Qué es PSeInt?

**PSeInt** significa *Pseudocódigo en Español Interactivo*. Es un programa que ayuda a estudiantes a aprender programación escribiendo instrucciones paso a paso, usando un lenguaje parecido al español.

Es ideal para empezar a entender cómo piensan los programas, sin necesidad de aprender un lenguaje como Java, Python o C desde el principio.

---

## 🧠 ¿Qué es una variable?

Una **variable** es como una cajita que guarda un valor que puedes usar y cambiar más adelante.  
Por ejemplo: si quieres guardar la edad de una persona, necesitas una variable.

### 📌 ¿Cómo se declara una variable en PSeInt?

```pseudocode
Definir edad Como Entero
Definir nombre Como Cadena
Definir promedio Como Real
```
## 🔢 Tipos de datos

| Tipo   | Significado                                |
|--------|---------------------------------------------|
| Entero | Números sin decimales (1, 2, 15...)         |
| Real   | Números con decimales (3.5, 7.2...)         |
| Número | Puede representar tanto Entero como Real    |              
| Cadena | Texto (nombres, frases, etc.)               |
| Lógico | Verdadero o Falso                           |

## ✍️ Entrada y salida de datos
### 🟢 Escribir

Sirve para mostrar mensajes o resultados en pantalla.
```pseudocode
Escribir "Hola mundo"
```
Esto imprime en pantalla: **Hola mundo**

### 🟡 Leer
Sirve para pedirle datos al usuario.
```pseudocode
Escribir "¿Cuál es tu nombre?"
Leer nombre
```
Este código primero muestra el mensaje y luego espera que el usuario escriba algo que se guarda en la variable **nombre.**

## 🔀 Condicionales
### 🧩 ¿Qué es un condicional?
Un condicional permite que el programa tome decisiones.

### 🧍‍♀️ Ejemplo de la vida real:
> **Si llueve**, entonces **llevo paraguas** ☔

### 💻 En programación:
```pseudocodigo
Si clima = "lluvia" Entonces
    Escribir "Llevar paraguas"
FinSi
```

## ✅ Condicional simple
```pseudocodigo
Si edad >= 18 Entonces
  Escribir "Eres mayor de edad"
Fin Si
```
💡 Este bloque solo se ejecuta si la condición se cumple.

## 🔁 Condicional con Sino
```pseudocodigo
Si nota >= 3 Entonces
  Escribir "Aprobaste"
Sino
  Escribir "Reprobaste"
Fin Si
```
💡 Se ejecuta una acción si se cumple la condición, y otra si no se cumple.

## 🔂 Condicionales anidados
```pseudocodigo
Si nota >= 3 Entonces
  Si nota >= 4.5 Entonces
    Escribir "Excelente nota"
  Sino
    Escribir "Pasaste"
  Fin Si
Sino
  Escribir "Reprobaste"
Fin Si
```
💡 Un condicional puede tener otro dentro de sí para tomar decisiones más complejas.

## 🔁 Bucles (Repeticiones)
### 🧩 ¿Qué es un bucle?
Un bucle sirve para repetir un bloque de instrucciones varias veces, sin tener que escribirlo muchas veces.

### 🔁 Mientras (While)
```pseudocodigo
i <- 1
Mientras i <= 5 Hacer
  Escribir i
  i <- i + 1
Fin Mientras
```
🟡 Este bucle se repite mientras se cumpla la condición.

### 🔄 Repetir - Hasta Que
```pseudocodigo
Repetir
  Escribir "Ingresa un número mayor que 0"
  Leer numero
Hasta Que numero > 0
```
🟢 Este bucle siempre se ejecuta al menos una vez y termina cuando la condición se cumple.

### ➰ Para (For)
```pseudocodigo
Para i <- 1 Hasta 5 Hacer
  Escribir i
Fin Para
```
🔵 Este bucle sirve para repetir una cantidad de veces conocida.

## 📦 Arreglos (Arrays)
### 🧩 ¿Qué es un arreglo?
Un arreglo es como una lista de variables del mismo tipo.
### Por ejemplo:
 > una lista de 5 notas, o de 10 nombres.

### 🧾 Declaración
```pseudocodigo
Dimensionar notas[5] 
```
Eso crea 5 espacios: notas[1], notas[2], ..., notas[5]

✍️ Asignar valores
```pseudocodigo
notas[1] <- 3.5
notas[2] <- 4.0
```

### 🔁 Recorrer con un bucle
### recorriendo con para (for)
Para asignar datos a nuestro array:
```pseudocodigo
Para i <- 1 Hasta 5 Hacer
  Escribir "Ingresa la nota ", i
  Leer notas[i]
Fin Para
```
Y luego mostrar:
```pseudocodigo
Para i <- 1 Hasta 5 Hacer
  Escribir "Nota ", i, ": ", notas[i]
Fin Para
```

### recorriendo con el bucle Mientras
```pseudocodigo
i <- 1
Mientras i <= 5 Hacer
  Escribir "Número en posición ", i, ": ", numeros[i]
  i <- i + 1
Fin Mientras
```
### Con el bucle Repetir - Hasta Que
Este bucle siempre se ejecuta al menos una vez.
```pseudocodigo
i <- 1
Repetir
  Escribir "Número en posición ", i, ": ", numeros[i]
  i <- i + 1
Hasta Que i > 5
```

## 🧠 ¿Cuál usar?

| Caso                                           | Bucle recomendado           |
|------------------------------------------------|-----------------------------|
| Sabes cuántos elementos hay                    | `Para`                      |
| Quieres terminar con una condición externa     | `Mientras` o `Repetir`     |
| Siempre quieres ejecutar al menos una vez      | `Repetir - Hasta Que`      |


## Adicional...

## 🧭 Segun (Switch/Case en PSeInt)
### 🧩 ¿Qué es?
Segun es una estructura que permite evaluar una variable o expresión y ejecutar diferentes bloques según su valor. Es más limpio y legible que usar muchos Si...Sino....

### 🔚 Conclusión
Segun es ideal cuando tienes muchas condiciones basadas en el mismo valor.

✅ Estructura:
```pseudocodigo
Segun variable Hacer
  Caso valor1:
    // instrucciones si es valor1
  Caso valor2:
    // instrucciones si es valor2
  De Otro Modo:
    // instrucciones si no coincide ningún caso
Fin Segun

```
### 📌 Ejemplo práctico:
```pseudocodigo
Definir dia Como Entero

Escribir "Ingresa un número del 1 al 7:"
Leer dia

Segun dia Hacer
  Caso 1:
    Escribir "Lunes"
  Caso 2:
    Escribir "Martes"
  Caso 3:
    Escribir "Miércoles"
  Caso 4:
    Escribir "Jueves"
  Caso 5:
    Escribir "Viernes"
  Caso 6:
    Escribir "Sábado"
  Caso 7:
    Escribir "Domingo"
  De Otro Modo:
    Escribir "Día no válido"
Fin Segun

```

### 🔁 También se puede agrupar casos:
```pseudocodigo
Caso 1, 2, 3:
  Escribir "Entre lunes y miércoles"
```

## 🧠 ¿Qué es una función en PSeInt?
Una función es un bloque de código reutilizable que recibe datos de entrada (parámetros), realiza alguna acción y puede devolver un valor.

Sirven para organizar tu código, evitar repetir instrucciones y dividir un problema en partes más pequeñas.

### 🧩 Estructura básica de una función
```pseudocodigo
Funcion NombreFuncion(param1, param2, ...) : TipoDeDato
  // Declarar variables internas
  // Instrucciones
  // Retornar valor (si es necesario)
FinFuncion
```
> El TipoDeDato puede ser: Entero, Real, Caracter, Logico, etc.


### ✅ Ejemplo 1: Función que suma dos números
```pseudocodigo
Funcion Sumar(a, b) : Entero
  Definir resultado Como Entero
  resultado <- a + b
  Retornar resultado
FinFuncion

// Programa principal
Definir x, y, suma Como Entero
Escribir "Ingresa dos números:"
Leer x, y
suma <- Sumar(x, y)
Escribir "La suma es: ", suma
```
### ✅ Ejemplo 2: Función sin retorno (subrutina)
A veces no necesitas que la función devuelva algo, solo que haga algo.
```pseudocodigo
SubProceso Saludar(nombre)
  Escribir "Hola, ", nombre, " ¿cómo estás?"
FinSubProceso

// Programa principal
Definir usuario Como Caracter
Escribir "¿Cuál es tu nombre?"
Leer usuario
Saludar(usuario)
```
### ✍️ Diferencias entre Funcion y SubProceso

| Característica               | Función     | SubProceso  |
|-----------------------------|-------------|-------------|
| Devuelve un valor           | ✅ Sí       | ❌ No       |
| Se puede usar en expresiones| ✅ Sí       | ❌ No       |
| Para mostrar mensajes       | ✅/❌ Opcional | ✅ Recomendado |

### 📚 Ejemplo 3: Función que verifica si un número es par
```pseudocodigo
Funcion EsPar(n) : Logico
  Si n MOD 2 = 0 Entonces
    Retornar Verdadero
  Sino
    Retornar Falso
  FinSi
FinFuncion

// Programa principal
Definir numero Como Entero
Escribir "Ingrese un número:"
Leer numero

Si EsPar(numero) Entonces
  Escribir "Es par"
Sino
  Escribir "Es impar"
FinSi
```

## 🧠 Tips importantes
- 📝 Toda función debe declararse antes del bloque principal.
- 🚫 Si no necesitas retornar nada, usa **SubProceso**.
- 🔁 Puedes reutilizar funciones cuantas veces quieras.











