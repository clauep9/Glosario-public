# Glosario-public
## Funciones
### 1. **`summary()`**  
   Genera un resumen estadístico:
```
   data <- c(1, 2, 3, 4, 5)
   summary(data)
```
### 2. **`mean()`**
   Calcula la media de un conjunto de números:
  ```
  data <- c(1, 2, 3, 4, 5)
  mean(data)
```
### 3. **`sd()`**  
   Calcula la desviación estándar:
 ```
   data <- c(1, 2, 3, 4, 5)
  sd(data)
 ```
### 4. **`read.csv()`**  
   Lee datos desde un archivo CSV:
 ```
   datos <- read.csv("archivo.csv")
 ```
### 5. **`head()`**  
   Muestra las primeras filas de un objeto:
 ```
   datos <- data.frame(A = 1:100)
  head(datos)
 ```
### 6. **`tail()`**  
   Muestra las últimas filas de un objeto:
 ```
   datos <- data.frame(A = 1:100)
  tail(datos)
 ```
### 7. **`seq()`**  
   Genera secuencias numéricas:
 ```
   numeros <- seq(1, 10, by = 2)
 ```
### 8. **`names()`**  
   Devuelve o establece los nombres de las columnas de un Data Frame:
 ```
   datos <- data.frame(A = 1:3, B = c("X", "Y", "Z"))
   names(datos)
   names(datos) <- c("Columna1", "Columna2")
 ```
### 9. **`rownames()`**  
   Devuelve o establece los nombres de las filas de un Data Frame:
 ```
   datos <- data.frame(A = 1:3, B = c("X", "Y", "Z"))
   rownames(datos) <- c("Fila1", "Fila2", "Fila3")
   rownames(datos)
 ```
 ### 10. **`str()`**  
   Muestra la estructura de un objeto:
 ```
   datos <- data.frame(A = 1:5, B = c("X", "Y", "Z", "W", "V"))
   str(datos)
 ```
 ### 11. **`paste()`**  
   Combina elementos de texto:
 ```
   nombres <- c("Juan", "Ana")
   paste("Hola", nombres)
 ```
### 12. **`as.character()`**  
   Convierte datos a formato de texto:  
```
    numeros <- c(1, 2, 3)
    as.character(numeros)
```
### 13. **`as.numeric()`**  
   Convierte datos a formato numérico:  
```
    texto <- c("1", "2", "3")
    as.numeric(texto)
 ```
### 14. **`substr()`**  
   Extrae una subcadena de un texto:  
   ```
    texto <- "Hola Mundo"
    substr(texto, start = 1, stop = 4)
   ```
### 15. **`tolower()`**  
   Convierte texto a minúsculas:  
   ```
    texto <- "Hola Mundo"
    tolower(texto)
   ```
### 16. **`toupper()`**  
   Convierte texto a mayúsculas:  
   ```
    texto <- "Hola Mundo"
    toupper(texto)
   ```
### 17. **`rownames()`**  
   Asigna nombres a las filas de un Data Frame:  
 ```
    df <- data.frame(Col1 = c(1, 2), Col2 = c("A", "B"))
    rownames(df) <- c("Fila1", "Fila2")
 ```
### 18. **`rowMeans()`**  
   Calcula la media de los valores de cada fila en una matriz o Data Frame:  
   ```
    matriz <- matrix(1:9, nrow = 3)
    rowMeans(matriz)
   ```
## Términos
### 19. **Data Frame**: 
Estructura de datos bidimensional para almacenar datos en forma de tabla.

Creación de un Data Frame
```
datos <- data.frame(
  Nombre = c("Ana", "Luis", "María"),
  Edad = c(23, 30, 27),
  Ciudad = c("San José", "Alajuela", "Cartago")
)
```
Ver el contenido del Data Frame
```
print(datos)
```
### 20. **Vector**: 
Estructura de datos básica en R para almacenar múltiples valores del mismo tipo.
Crear un vector numérico
```
numeros <- c(1, 2, 3, 4, 5)
```
Crear un vector de caracteres
```
nombres <- c("Ana", "Luis", "María")
```
Crear un vector lógico
```
logicos <- c(TRUE, FALSE, TRUE)
```
Imprimir los vectores
```
print(numeros)
print(nombres)
print(logicos)
```
### 21. **Lista**: 
Estructura de datos que puede almacenar diferentes tipos de objetos.
Crear una lista con diferentes tipos de datos
```
mi_lista <- list(
  numeros = c(1, 2, 3, 4),
  texto = "Hola Mundo",
  logicos = c(TRUE, FALSE, TRUE),
  matriz = matrix(1:4, nrow = 2)
)
```
Imprimir la lista completa
```
print(mi_lista)
```
Acceder a un elemento por su nombre
```
mi_lista$numeros  # Devuelve el vector 'numeros'
```
Acceder a un elemento por su posición
```
mi_lista[[2]]  # Devuelve el segundo elemento ('Hola Mundo')
```
Acceder a un subelemento dentro de un elemento
```
mi_lista$matriz[1, 2]  # Devuelve el valor en la primera fila, segunda columna de la matriz
```
Modificar un elemento de la lista
```
mi_lista$texto <- "Nuevo texto"
print(mi_lista$texto)
```
### 22. **Matriz (Matrix)**: 
Estructura bidimensional de datos homogéneos.
Crear un Data Frame
```
datos <- data.frame(
  Nombre = c("Ana", "Luis", "María"),
  Edad = c(23, 30, 27),
  Ciudad = c("San José", "Alajuela", "Cartago")
)
```
Mostrar el Data Frame
```
print(datos)
```
