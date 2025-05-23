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
### 23. **Variable**: 
Valor o conjunto de valores que se almacenan en memoria para ser utilizados en cálculos o análisis.

Asignar un valor a una variable
```
x <- 5  # 'x' contiene el valor numérico 5
```
Asignar un vector a una variable
```
mi_vector <- c(1, 2, 3, 4, 5)
```
Asignar texto a una variable
```
saludo <- "Hola Mundo"
```
Mostrar las variables
```
print(x)
print(mi_vector)
print(saludo)
```
### 24. **Package**: 
Conjunto de funciones, datos y documentación adicional.

Instalar y luego llamar un paquete 
```
install.packages("ggplot2")
library(ggplot2)
```
### 25. **Environment**: 
Espacio de trabajo donde se almacenan los objetos creados (como variables, funciones, etc.).

Crear un nuevo environment
```
mi_entorno <- new.env()
```
Asignar un objeto al nuevo environment
```
assign("x", 42, envir = mi_entorno)
```
Acceder al objeto dentro del nuevo environment
```
mi_entorno$x
```
## Funciones comunes en GGPLOT
### 26. **library()**
Activa el paquete ggplot2.
```
library(ggplot2)
```
### 27. **ggplot()**
Crea la estructura base del gráfico.
```
ggplot(data = dataframe, aes(x = gene, y = expression)) + geom_point()
```
### 28. **aes()**
Define el mapeo estético entre variables.
```
aes(x = gene_length, y = mutation_rate, color = tissue_type)
```
### 29. **geom_point()**
Crea un gráfico de dispersión.
```
ggplot(dataframe, aes(x = age, y = gene_expression)) + geom_point()
```
### 30. **geom_bar()**
Genera un gráfico de barras.
```
ggplot(dataframe, aes(x = cancer_type)) + geom_bar()
```

### 31. **geom_line()**
Dibuja líneas para datos continuos.
```
ggplot(dataframe, aes(x = time, y = cell_count, color = treatment)) + geom_line()
```
### 32. **geom_boxplot()**
Crea un diagrama de caja para comparar grupos.
```
ggplot(dataframe, aes(x = group, y = gene_expression)) + geom_boxplot()
```
### 33. **geom_histogram()**
Construye un histograma.
```
ggplot(dataframe, aes(x = gene_length)) + geom_histogram(bins = 30)
```
### 34. **geom_smooth()**
Añade líneas de ajuste, como regresiones.
```
ggplot(dataframe, aes(x = age, y = gene_expression)) + geom_smooth(method = "lm")
```
### 35. **labs()**
Agrega títulos y etiquetas.
```
labs(title = "Expresión génica por edad", x = "Edad", y = "Expresión")
```
### 36. **theme_minimal()**
Aplica un tema minimalista, es decir, elimina elementos visuales innecesarios para destacar los datos relevantes.
```
ggplot(dataframe, aes(x = var1, y = var2)) + geom_point() + theme_minimal()
```
### 37. **scale_color_manual()**
Define colores personalizados.
```
scale_color_manual(values = c("red", "blue"))
```
### 38. **facet_wrap()**
Divide gráficos según una variable categórica.
```
facet_wrap(~ tissue_type)
```
### 39. **facet_grid()**
Organiza gráficos en una cuadrícula basada en dos variables.
```
facet_grid(rows = vars(treatment), cols = vars(cancer_stage))
```
### 40. **coord_flip()**
Invierte los ejes para gráficos horizontales.
```
ggplot(dataframe, aes(x = cancer_type, y = sample_count)) + geom_bar(stat = "identity") + coord_flip()
```
### 41. **geom_density()**
Visualiza la densidad de datos.
```
ggplot(dataframe, aes(x = gene_length)) + geom_density()
```
### 42. **scale_x_log10()**
Aplica una escala logarítmica al eje x.
```
ggplot(dataframe, aes(x = gene_length, y = mutation_rate)) + geom_point() + scale_x_log10()
```
### 43. **scale_y_continuous()**
Ajusta el rango del eje y.
```
scale_y_continuous(limits = c(0, 100))
```
### 44. **geom_violin()**
Crea diagramas de violín.
```
ggplot(dataframe, aes(x = group, y = expression)) + geom_violin()
```
### 45. **theme()**
Personaliza elementos gráficos.
```
theme(axis.text.x = element_text(angle = 45, hjust = 1))
```
### 46. **ggsave()**
Guarda el gráfico en un archivo.
```
ggsave("grafico.pdf", width = 10, height = 8)
```
### 47. **geom_tile()**
Crea mapas de calor.
```
ggplot(dataframe, aes(x = gene, y = sample, fill = expression)) + geom_tile()
```
### 48. **stat_summary()**
Resume y visualiza estadísticas.
```
ggplot(dataframe, aes(x = treatment, y = expression)) + stat_summary(fun = mean, geom = "bar")
```
### 49. **element_blank()**
Oculta elementos del gráfico.
```
theme(axis.title.y = element_blank())
```
### 50. **annotate()**
Añade anotaciones al gráfico.
```
annotate("text", x = 10, y = 20, label = "Nota importante", color = "red")
```
