# 2627-PR-U1-ssiegon731-ActividadesRepaso
### 1. Informe de una frase

Desarrolla un programa que lea una frase y muestre una versión normalizada junto con algunos datos sobre ella.

Funciones que debes implementar:

- **`preparar_texto(frase)`**: elimina los espacios de los extremos y convierte el texto a minúsculas. Devuelve el texto preparado.

- **`analizar_texto(frase)`**: recibe el texto preparado y devuelve una tupla con tres datos: número de caracteres —incluidos los espacios interiores—, número de palabras y si contiene la palabra completa `"python"`. Para obtener las palabras, utiliza `split()`.

La función **`main()`** debe leer la frase, llamar a `preparar_texto()` y comprobar si el resultado está vacío. Si está vacío, mostrará un mensaje de error. En caso contrario, llamará a `analizar_texto()`, desempaquetará la tupla y mostrará el informe.

Ejemplo:

```text
Entrada:
  Aprender PYTHON es divertido  

Salida:
Texto: aprender python es divertido
Caracteres: 28
Palabras: 4
Contiene la palabra python: sí
```

Puedes suponer que las palabras están separadas por espacios y que la frase no contiene signos de puntuación.

**Requisitos**

- Añade anotaciones de tipo a los parámetros, retornos y variables principales.
- Documenta las funciones auxiliares mediante docstrings con `:param` y `:return`.
- Gestiona la entrada y la salida en `main()`; las funciones auxiliares devuelven sus resultados con `return`.
- Incluye la guarda de ejecución.
- Entrega un repositorio PÚBLICO con el nombre `2627-PR-U1-usarioPasen-informe_frase` y tu solución.

### 2. Ficha de un rectángulo**

Desarrolla un programa que lea la base y la altura de un rectángulo, expresadas en centímetros, y muestre sus medidas y orientación.

Funciones que debes implementar:

- **`calcular_medidas(base, altura)`**: devuelve una tupla con el área y el perímetro, en ese orden. El área es el producto de la base por la altura; el perímetro es el doble de la suma de ambas.
- **`determinar_forma(base, altura)`**: devuelve `"cuadrado"` si ambas medidas son iguales, `"horizontal"` si la base es mayor que la altura y `"vertical"` en el caso restante.

La función **`main()`** debe leer y convertir las dos medidas. Si alguna es menor o igual que cero, mostrará un mensaje de error. En caso contrario, llamará a las dos funciones, desempaquetará las medidas y mostrará los resultados con dos decimales.

Ejemplo:

```text
Entrada:
8
3

Salida:
Forma: horizontal
Área: 24.00 cm²
Perímetro: 22.00 cm
```

Puedes suponer que las entradas tienen un formato numérico válido.

**Requisitos**

- Añade anotaciones de tipo a los parámetros, retornos y variables principales.
- Documenta las funciones auxiliares mediante docstrings con `:param` y `:return`.
- Gestiona la entrada y la salida en `main()`; las funciones auxiliares devuelven sus resultados con `return`.
- Incluye la guarda de ejecución.
- Entrega un repositorio PÚBLICO con el nombre `2627-PR-U1-usarioPasen-rectangulo` y tu solución.

  ### 3. Puntuación de una partida

Desarrolla un programa que lea el número de aciertos y de errores obtenidos en un juego de preguntas. Cada acierto suma **3 puntos** y cada error resta **1 punto**.

**Constantes**

Declara a nivel de módulo las constantes correspondientes a los puntos por acierto y la penalización por error.

Crea también la constante **`VALORACION_PARTIDA`**, una tupla de tres posiciones con estos textos, en este orden:

```python
("Sigue practicando", "Buen resultado", "Excelente")
```

**Funciones que debes implementar**

- **`calcular_resultados(aciertos, errores)`**: devuelve una tupla con el número total de preguntas respondidas y la puntuación obtenida, en ese orden.
- **`valorar_partida(puntuacion)`**: devuelve un número entero que indica la posición del mensaje que se debe mostrar de `VALORACION_PARTIDA`:
  - **`0`** si la puntuación es inferior a 10.
  - **`1`** si está entre 10 y 19, ambos incluidos.
  - **`2`** si es de 20 o más.

La función **`main()`** debe leer y convertir los dos datos a enteros.

Si los aciertos o los errores son negativos, el programa debe mostrar **únicamente** este mensaje y finalizar, sin llamar a las funciones auxiliares:

```text
ERROR - valores incorrectos
```

Si ambos valores son válidos, `main()` llamará a las dos funciones, desempaquetará la tupla de resultados y utilizará el índice devuelto por `valorar_partida()` para acceder al mensaje correspondiente de `VALORACION_PARTIDA`.

Una partida con cero preguntas respondidas es válida. La puntuación final puede ser negativa.

**Entrada y salida**

Lee primero los aciertos y después los errores, en líneas separadas y **sin imprimir mensajes para solicitar los datos**. Puedes suponer que ambas entradas tienen un formato de número entero válido.

Con esta entrada:

```text
6
2
```

La salida debe ser:

```text
Preguntas respondidas: 8
Puntuación: 16
Valoración: Buen resultado
```

**Requisitos**

- Define exactamente dos funciones además de `main()`.
- Utiliza las constantes declaradas en el programa.
- Añade anotaciones de tipo a los parámetros, retornos y variables principales.
- Documenta las funciones auxiliares mediante docstrings con `:param` y `:return`.
- Gestiona la entrada y la salida en `main()`; las funciones auxiliares devuelven sus resultados con `return`.
- Incluye la guarda de ejecución.
- Entrega un repositorio PÚBLICO con el nombre `2627-PR-U1-usarioPasen-partida` y tu solución.
