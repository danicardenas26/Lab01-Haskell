# Laboratorio 1 - Introduccion Haskell

## 📌 Descripción  
Este laboratorio tiene como objetivo que los estudiantes fortalezcan sus conocimientos relacionados con **Haskell** y la programación funcional.

---

## 🛠️ Instrucciones Generales  

1. **Fork del repositorio**  
   - Realice un **fork** de este repositorio en su cuenta personal de GitHub.  
   - No realice cambios directamente sobre el repositorio original.  

2. **Estructura de carpetas**  
   - Dentro de su fork, cree una carpeta llamada **`lab01/`**.  
   - Cada ejercicio debe resolverse en un archivo **independiente** con el siguiente formato:  
     ```
     lab01/ejercicio01.ipynb
     lab01/ejercicio02.ipynb
     ...
     ```  

3. **Resolución de ejercicios**  
   - Desarrolle los programas en el entorno de programacion indicado en clase.  
   - Una vez finalizados, cargue el código de los archivos `.ipynb` correspondientes en su repositorio.  
   - Cada archivo debe contener:
     - La implementación de su solución.  

4. **Buenas prácticas**  
   - Use **nombres de predicados claros y significativos**.
---

## 🚀 Entrega  

- **Plazo**: La entrega debe realizarse a mas tardar el proximo lunes, se habilitara una tarea en Moodle para adjuntar el link del repositorio.

---

## ✅ Criterios de Evaluación  

1. **Correctitud de las soluciones** (funcionalidad de los predicados).  
2. **Cumplimiento de la estructura solicitada** (archivos independientes en `lab01/`).  
3. **Claridad en la codificación** (nombres, comentarios y legibilidad).  
4. **Uso adecuado de variables** (incluyendo variables anónimas donde corresponda).  

---

## 💡 Recomendaciones  

- Revise la documentación oficial de Haskell: [Haskell Documentation](https://www.haskell.org/documentation/).  
- Antes de subir sus archivos, **ejecute y verifique** cada consulta en el compilador en linea.  
- Mantenga su repositorio organizado y actualizado.

---

## Ejercicio 1 - Fundamentos básicos y tipos

1. Escribe el codigo correspondiente para concatenar dos listas: [1,2,3] y [4,5]
2. Revisa el tipo de una expresión usando :t, por ejemplo

     ```  
      :t True
      :t "Hola mundo"
      :t [1,2,3]
     ```

   **Pregunta teórica:**
      ¿Qué significa que Haskell sea un lenguaje fuertemente tipado y evaluado perezosamente?

3. Define las siguientes funciones

   a. ``doble :: Int -> Int``. Devuelve el doble de un número.
   
   b. ``esMayorEdad :: Int -> Bool``. Devuelve True si la edad ingresada es mayor o igual a 18.
   
   c. ``areaCirculo :: Float -> Float``. Calcula el área de un círculo dado su radio.
      
      Pista: Usa pi que ya está definido en Haskell.

   **Pregunta de reflexión:**
      ¿Qué diferencias encuentras entre los tipos Int y Float?}

---


## Ejercicio 2 - Listas y operaciones básicas

1. Ejecuta y analiza el resultado de las siguientes funciones sobre listas

   ```
   head [10,20,30,40]
   tail [10,20,30,40]
   take 3 [1..10]
   drop 4 [1..10]
   length [1,2,3,4,5]
   ```
   
**Pregunta:**
¿Qué hace la expresión [1..10] y cómo se relaciona con la evaluación perezosa?

2. Define las siguientes funciones

   a. ``primerElemento :: [a] -> a``. Devuelve el primer elemento de la lista usando patrones.
   
   b. ``productoLista :: [Int] -> Int``. Calcula el producto de todos los elementos de la lista de forma recursiva.
   
   c. ``eliminarNegativos :: [Int] -> [Int]``. Devuelve una lista que contiene solo los números mayores o iguales a 0.

   d. Reto: Implementa ``invertir :: [a] -> [a]``. Para invertir una lista sin usar la función reverse.


---

## Ejercicio 3 - Definición de funciones: composición y casos

1. Define las siguientes funciones:

   a. ``sumaCuadrados :: Int -> Int -> Int``. Que calcule la suma de los cuadrados de dos número, define suma y cuadrado.

   b. ``dobleLista :: [Int] -> [Int]``. Multiplica por 2 cada elemento de una lista usando map y una funcion "duplicar".

      * Averigua cual es la forma mas simple de implementar esto

2. Define las siguientes funciones:

   a. ``clasificarNota :: Int -> String``. Que retorne:

         Menor a 3 → "Reprobado"
         
         Entre 3 y 4 → "En recuperación"
         
         Mayor o igual a 4 → "Aprobado"
         
   b. ``fibonacci :: Int -> Int``


---

## Ejercicio 4 - Evaluación funcional

1. Predice la evaluación paso a paso

   Dada la expresión:

   ``take 5 (map (*2) [1..])``

   a. Predice el resultado sin ejecutarlo.

   b. Luego, ejecútalo y compara tu predicción.

   **Pregunta de análisis:**
   ¿Por qué [1..] no causa un ciclo infinito?


2. Considera la siguiente función: ``misterio x y = if x > 10 then y * 2 else x + y``

   a. Evalua paso a paso ``misterio (5+7) (4*3)``

---

## Ejercicio 5 - Expresiones Lambda

1. Reescribe estas funciones usando lambda:

   a. ``incrementarLista xs = map suma xs``
   
   b. ``filtrarPares xs = filter even xs``

   c. ``sumarTuplas xs = ...``

---


## Retrospectiva
1. ¿Cuál fue el tiempo total invertido en el laboratorio por cada uno de ustedes? (Horas/Hombre)
2. ¿Cuál es el estado actual del laboratorio? ¿Por qué?
3. ¿Cuál consideran fue el mayor logro? ¿Por qué?
4. ¿Cuál consideran que fue el mayor problema técnico? ¿Qué hicieron para resolverlo?
5. ¿Qué hicieron bien como equipo? ¿Qué se comprometen a hacer para mejorar los resultados?
6. ¿Qué referencias usaron? ¿Cuál fue la más útil? Incluyan citas con estándares adecuados.

