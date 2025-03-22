# EXAMEN TEÓRICO

## Unidad I: Fundamentos de la Lógica de Programación

**Nombre del Estudiante:** _Jerónimo Grajales Quintero_______________________________
**Fecha:** 22/03/2025_______________
**Calificación:** _______________

### INSTRUCCIONES

- Tiempo de duración: 1 horas
- Lea cuidadosamente cada pregunta antes de responder
- No se permite el uso de dispositivos electrónicos
- Justifique adecuadamente sus respuestas cuando se indique

---

## PARTE I: CONCEPTOS FUNDAMENTALES (30 puntos)

1. **Defina con precisión el concepto de "lógica de programación" y explique por qué es fundamental para el desarrollo de aplicaciones informáticas.** (6 puntos)
es lo q hace q el algoritmo trabaje adecuadamente y no hallan errores3. **Explique las cuatro principales características que debe tener un algoritmo para ser considerado correcto y eficiente.** (6 puntos)

4. **Describa la diferencia entre abstracción y descomposición como técnicas de la lógica de programación, y proporcione un ejemplo práctico de aplicación de cada una.** (6 puntos)
abstraccion es cuando se abstrae un archivo y descomposicion es cuando se coje el archivo en varias partes

6. **Defina los siguientes conceptos y explique su importancia en la lógica de programación:** (6 puntos)

   a) Variable
significa q un numero(por ejemplo) tiende a ser cambiante, en pocas palabras, q no es fijo
   b) Constante
es algo q se repite hasta q alcanza un punto deseado
   c) Tipo de dato  *(Opcional - **Punto extra**)*

7. **Explique qué es la "jerarquía operacional" y por qué es crucial en el desarrollo de expresiones complejas. Proporcione un ejemplo donde el resultado cambie según la aplicación de la jerarquía.** (6 puntos)



## PARTE II: ANÁLISIS Y APLICACIÓN (40 puntos)

1. **Observe el siguiente pseudocódigo e identifique todos los errores lógicos presentes. Reescriba la solución correcta y explique cada corrección realizada.** (10 puntos)

    ```psc
    ALGORITMO CalcularPromedio
        DEFINIR nota1, nota2, nota3, promedio COMO REAL
        ESCRIBIR "Ingrese las tres notas:"
        LEER nota1, nota2, nota3
        promedio = nota1 + nota2 + nota3
        SI promedio >= 7 ENTONCES
            ESCRIBIR "Aprobado con: ", promedio
        SINO
            SI promedio >= 4 && promedio < 7 ENTONCES
                ESCRIBIR "Recuperación con: ", promedio
            SINO
                ESCRIBIR "Reprobado con: ", promedio
            FINSI
        FINSI
    FINALGORITMO
    ```

2. **Dados los siguientes valores de variables:**
   - `a = 5`
   - `b = 2`
   - `c = 10`

   **Evalúe paso a paso las siguientes expresiones, mostrando los resultados intermedios y explicando la aplicación de la jerarquía operacional en cada caso:** (10 puntos)

   a) `(a * b + c) / (b * b - a)`     (5  *  2   +   10) / (2  *  2  -  5) = 19

   b) `a > b && (c / b) >= a`       5 > 2 && (10 / 2 ) >=5   verdadero 

   c) `!(a = c) || b < (a + c)`   !(5 = 10 ) || 2 < (5 + 10)  

   d) `(a ^ 2 + b ^ 2) > c && !(a = b)`   

3. **Aplique la técnica de descomposición para los siguientes problemas, identificando claramente los subproblemas, las entradas/salidas y las variables necesarias. Proporcione un algoritmo de alto nivel para cada caso (sin necesidad de pseudocódigo detallado):** (10 puntos)

   a) Diseñar un sistema que calcule el total a pagar en una tienda de ropa, considerando el precio base de cada prenda, los impuestos aplicables, y posibles descuentos por temporada o cantidad.
Inicio

a.camisa 20.000
b.pantalon 70.000
c.camibuso 50.000

proceso
cojer los precios a b c y sumarlos tambien calcular un descuento del 20%

a+b+c-20%= 112.000
cancelar el dinero 
final  
dar el precio

finsi
   b) Crear una solución para convertir una cantidad de segundos ingresada por el usuario en su equivalente en horas, minutos y segundos.

5. **Explique la importancia de verificar los datos de entrada en un algoritmo. Proporcione tres ejemplos concretos de técnicas para comprobar que los datos numéricos ingresados por un usuario son válidos para el problema que se intenta resolver.** (10 puntos)

---

## PARTE III: REPRESENTACIÓN DE ALGORITMOS (30 puntos)

1. **Elabore un diagrama de flujo, siguiendo los estándares profesionales vistos en clase, para un algoritmo que determine si un número ingresado por el usuario es par o impar, positivo o negativo.** (10 puntos)

2. **Escriba el pseudocódigo completo utilizando la sintaxis de PSeInt para un algoritmo que calcule el promedio de un conjunto de números ingresados por el usuario, donde primero se solicite la cantidad de números a ingresar.** (10 puntos)

3. **Analice el siguiente algoritmo y describa paso a paso qué operación matemática realiza. Evalúe manualmente el algoritmo con los valores de entrada 24 y 36, mostrando el estado de todas las variables en cada iteración.** (10 puntos)

    ```psc
    ALGORITMO Operacion
        DEFINIR num1, num2, temp COMO ENTERO
        ESCRIBIR "Ingrese dos números enteros positivos:"
        LEER num1, num2
        
        // Aseguramos que num1 sea mayor que num2
        SI num1 < num2 ENTONCES
            temp = num1
            num1 = num2
            num2 = temp
        FINSI
        
        // Proceso principal
        MIENTRAS num2 <> 0 HACER
            temp = num2
            num2 = num1 MOD num2
            num1 = temp
        FINMIENTRAS
        
        ESCRIBIR "El resultado es: ", num1
    FINALGORITMO
    ```

---

## PREGUNTAS DE INTEGRACIÓN PROFESIONAL (bonus - 10 puntos)

1. **En un contexto profesional, un cliente le solicita desarrollar un algoritmo para automatizar ciertos cálculos financieros. El cliente no tiene conocimientos técnicos. Explique detalladamente:**

   a) ¿Qué técnicas de la lógica de programación utilizaría para comprender y modelar este problema?

   b) ¿Cómo documentaría su solución para que sea comprensible tanto para el cliente como para otros programadores?

   c) ¿Qué estrategias implementaría para comprobar que el algoritmo funciona correctamente en todos los casos posibles? (10 puntos)

---

**CRITERIOS DE EVALUACIÓN:**

- Precisión conceptual y uso adecuado de la terminología
- Profundidad y claridad en las explicaciones
- Correcta aplicación de las técnicas de lógica de programación
- Seguimiento de estándares en diagramas y pseudocódigo
- Capacidad de análisis crítico y resolución de problemas
- Aplicación de principios metodológicos en la documentación y comprobación de algoritmos
