# EXAMEN AZZ - LVV 2025  
**Somos + Podemos +**  

A continuación se presenta una evaluación compuesta por tres preguntas. No es necesario desarrollar todas las preguntas, pero es importante tener en cuenta que cada una tiene un peso asignado.  

### Importancia de las preguntas:
- **Pregunta N° 03** (Pregunta de mayor importancia)  
- **Pregunta N° 01**  
- **Pregunta N° 02**  

---

## Pregunta N° 01  

Crear un dataframe (`df`) con tres variables:  
- **Producto** (`str`)  
- **Ventas** (`float`)  
- **Categoría** (`category`)  

Debe contener **1000 observaciones** con las siguientes características:

| Index | Producto | Ventas | Categoría |
|-------|---------|--------|-----------|
| 0     | P0001   | 1500   | GIMPAR    |
| 1     | P0002   | 3000   | GPAR      |
| 2     | P0003   | 1900   | GIMPAR    |
| ...   | ...     | ...    | ...       |
| 999   | P1000   | 6252   | GPAR      |

**Condiciones**:
- `Index` es el índice generado por `pandas` u otra biblioteca de manejo de datos.
- `Producto` debe estar ordenado del 1 al 1000, con formato de cuatro dígitos (`P0001`, `P0002`, ...).
- `Ventas` debe ser un número aleatorio entre **1000 y 10000**.
- `Categoría`:  
  - Si el número del producto es **impar**, será `"GIMPAR"`.  
  - Si es **par**, será `"GPAR"`.  

### Creación de la variable "Venta Neta"  
Se debe generar una nueva variable **"Venta Neta"**, calculada de la siguiente manera:  

$\text{Venta Neta} = \text{Ventas} - \text{(Impuesto IGV 18\%)} - \text{(Descuento variable)}$


**Tabla de descuentos**:

| Rango de Ventas | Descuento |
|-----------------|-----------|
| 1000 - 1500    | 1%        |
| 1500 - 3000    | 2%        |
| 3000 - 7000    | 3%        |
| 7000 - 9000    | 4%        |
| 10000 >        | 5%        |

**Se valorará el uso de funciones.**

---

## Pregunta N° 02  

- Exportar el **dataframe inicial** en formato **Parquet** con compresión **Snappy**.  
- Importarlo a **Power BI** y realizar lo siguiente:  
  1. Crear la columna **"Venta Neta"** utilizando **DAX**.  
  2. Crear **gráficos y visualizaciones** a partir de los datos generados.  

---

## Pregunta N° 03 (Pregunta de mayor importancia)  

Usando el **Libro de Excel** titulado **BASES_MODELO**, realizar las siguientes tareas en **Python**:  

1. **Unir datos**:
   - Unir la hoja **BASE_VARIABLES** con la hoja **BASE_ESTIMADOS** agregando la columna **CANTIDADES ESTIMADAS** correspondiente a cada producto.  
   - Agregar la hoja **BASE_ASESORAS**, incluyendo el número de asesoras por campaña y zona.  

2. **Modelado Predictivo**:  
   - Construir un modelo donde la **variable respuesta** sea **VENTA** (total de ventas realizadas).  
   - Considerar como **variables explicativas** los datos de ventas por zonas.  
   - Dividir los datos en **entrenamiento** y **validación**, probando el modelo con campañas no incluidas en el entrenamiento.  

3. **Evaluación y Comparación**:
   - Comparar el **poder predictivo** del modelo construido con las **CANTIDADES ESTIMADAS** de mercadeo.  
   - Concluir cuál es mejor:  
     - **El modelo realizado** o  
     - **Las estimaciones de mercadeo**.  

### Criterios de Evaluación:
1. **Poder predictivo del algoritmo**.  
2. **Creación de variables a partir de los grupos**.  
3. **Presentación del análisis y resultados**.  
4. **Interpretación y metodología utilizada en cada paso del proceso**.  
