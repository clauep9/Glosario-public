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
    ```R
    texto <- "Hola Mundo"
    toupper(texto)
    ```
