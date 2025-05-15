# RETO 3 

## Sergio Olivares Martin.

## OBJETIVOS

- A partir del algoritmo de identificación de los divisores plantear la serie de pasos para determinar los números primos hasta un natural n.

- Plantear el algoritmo para obtener los números primos hasta n, usando pseudocódigo y diagramas de flujo.

- Cree un repositorio en github en donde muestre el desarrollo de la actividad y comparta el enlace por el canal de slack reto_3.

## 1. Pasos para determinar los número primos hasta un natural n.

INICIO

Paso 1: Definir n como un número natural y mayor que 2. n>2.

Paso 2: Ingresar el valor de n

Paso 3: Empezar a revisar desde el 2 hasta el número n.

Paso 4: Para cada número revisar cuántos divisores exactos naturales tiene.

Paso 5: Si el número sólo tiene 2 divisores exactos naturales entonces es primo, catalogarlo como "Primo"

Paso 6: Escribir "Los números primos hasta "n" son: "

Paso 7 : Imprimir todos los números catalogados como "Primo"

FIN

## 2.1 Pseudocódigo

INICIO

Escribir "Ingrese un número mayor a 2"
Leer n 

si n < 2 entonces
    
    escribir "Vuelva a ingresar un número mayor a 2"

sino 

Para x desde 2 hasta n hacer

    contador ← 0

    Para j desde 2 hasta x hacer

        Si x mod j = 0 entonces

            contador ← contador + 1

    FinPara

    Si contador = 2 entonces

        Imprimir x es primo

    FinSi

FinPara

FIN

## 2.2 Diagrama de flujo con Mermaid.
```mermaid
flowchart TD
    A[Inicio] --> B[Ingrese un número mayor a 2, n.]
    B -- SI --> C[Para x desde 2 hasta n]
    B -- NO --> T[Ingrese un número mayor a 2.]
    C --> D[Contador_divisores = 0]
    D --> E[Para j desde 1 hasta x]
    E --> F[Si x mod j == 0]
    F --> G[Incrementar contador_divisores]
    G --> H[Fin del bucle j]
    H --> I[¿contador_divisores == 2?]
    I -- Sí --> J[x es primo]
    I -- No --> K[Ignorar]
    J --> L[Fin del bucle i]
    K --> L
    T --> M[Ingrese un número mayor a 2.]
    L --> M[Fin]
   ```
   Fin, muchas gracias.