# ACTIVIDAD 4

## 1. Introducción
### ¿Por qué crees que el pseudocódigo es útil antes de escribir un programa en C?

**R//**  
Yo considero que es importante escribir un pseudocódigo antes del código de programación, ya que esto nos ayuda a organizar todas las ideas y los pasos a seguir de una forma más simple.

## 2. Estructura básica del pseudocódigo
### Toma un pseudocódigo de un ejercicio anterior o escribe tu propio pseudocódigo, similar al mostrado en el ejemplo de arriba.

**R//**  
```
Inicio  
Escribir "Ingrese el primer valor:"  
Leer num1  

Escribir "Ingrese el segundo valor:"  
Leer num2  

resultado = num1 + num2  

Escribir "La suma es: ", resultado  
Fin  
```
## 3. Traduciendo el pseudocódigo a C
### ¿Por qué es importante declarar el tipo de variable (int, float, etc.) antes de usarla en C?

**R//**  
Porque en C, declarar el tipo de variable ayuda a definir cuánto espacio ocupará en memoria y qué tipo de datos almacenará, evitando errores y haciendo el código más eficiente.

## 4. Ejemplos adicionales de pseudocódigo y su traducción
### Escribe tu propio pseudocódigo para calcular el promedio de una lista de calificaciones y tradúcelo a C.

**R//**    

**Pseudocodigo**
```
Inicio  

Escribir "Ingrese la cantidad de calificaciones:"  
Leer n  

suma = 0  

Para i = 1 Hasta n Hacer  
    Escribir "Ingrese la calificación"  
    Leer calificacion  
    suma = suma + calificacion  
FinPara  

promedio = suma / n  

Escribir "El promedio de las calificaciones es:", promedio  

Fin  
```
**Codigo en c**
```
#include <stdio.h>

int main() {
    int n, i;
    float suma = 0, calificacion, promedio;

    printf("Ingrese la cantidad de calificaciones: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++) {
        printf("Ingrese la calificación %d: ", i);
        scanf("%f", &calificacion);
        suma += calificacion;
    }

    promedio = suma / n;
    printf("El promedio de las calificaciones es: %.2f\n", promedio);

    return 0;
}
```
## 5. Buenas prácticas
### ¿Por qué es importante comentar el código, aunque sea breve y conciso?

**R//**   
Esto es importante para tener un buen entendimiento de lo que hace cada parte del código, ya que muchas veces se trabaja con otras personas y esta es una forma de explicar lo que se hizo. Además, muchas personas escriben el código de manera diferente, o simplemente, cuando retomamos el código después de un tiempo, es muy probable que olvidemos lo que hicimos y por qué lo hicimos de esa manera. Estos comentarios nos ayudan a recordarlo y a poder continuar con el código sin dificultades.

## 6. Reto final
### Reto: toma el pseudocódigo de los 5 primeros ejercicios del Reto y realiza la traducción a C:

**R//**  

1. **Se requiere obtener la distancia entre dos puntos en el plano cartesiano,
tal y como se muestra en la figura 1. Realice un diagrama de flujo y pseudocódigo
que representen el algoritmo para obtener la distancia entre
esos puntos.**

**Pseudocodigo**
```
Inicio  
Escribir "Ingrese las coordenadas del primer punto (X1, Y1)"  
Leer X1, Y1    
Escribir "Ingrese las coordenadas del segundo punto (X2, Y2)"  
Leer X2, Y2  
D = SQRT ((X1-X2)*(X1-X2)+(Y1-Y2)*(Y1-Y2))  
Escribir "La distancia entre los dos puntos es: ", D  
Fin  
```
**Codigo en c**
```
#include <stdio.h>  // Librería para entrada y salida de datos
#include <math.h>   // Librería para funciones matemáticas, como sqrt()

int main() {
    float x1, y1, x2, y2, distancia;

    // Pedimos al usuario que ingrese las coordenadas del primer punto
    printf("Ingrese las coordenadas del primer punto (X1, Y1): ");
    scanf("%f %f", &x1, &y1);

    // Pedimos al usuario que ingrese las coordenadas del segundo punto
    printf("Ingrese las coordenadas del segundo punto (X2, Y2): ");
    scanf("%f %f", &x2, &y2);

    // Calculamos la distancia usando la fórmula de distancia entre dos puntos
    distancia = sqrt((x1 - x2) * (x1 - x2) + (y1 - y2) * (y1 - y2));

    // Mostramos el resultado con dos decimales
    printf("La distancia entre los dos puntos es: %.2f\n", distancia);

    return 0; // Fin del programa
}

```

2. **Una modista, para realizar sus prendas de vestir, encarga las telas al extranjero.
Para cada pedido, tiene que proporcionar las medidas de la tela
en pulgadas, pero ella generalmente las tiene en metros. Realice un algoritmo
para ayudar a resolver el problema, determinando cuántas pulgadas
debe pedir con base en los metros que requiere. Represéntelo mediante un
diagrama de flujo y pseudocódigo (1 pulgada = 0.0254 m).**

**Pseudocodigo** 
```
Inicio     
Escribir "ingrese la cantidad de tela en metros"  
Leer metros   
Pulgadas = metros/0.0254  
Escribir "Son", Pulgadas, "pulgadas de tela."  
Fin  
```
**Codigo en c**
```
#include <stdio.h>  // Librería para entrada y salida de datos

int main() {
    float metros, pulgadas;

    // Pedimos al usuario que ingrese la cantidad de tela en metros
    printf("Ingrese la cantidad de tela en metros: ");
    scanf("%f", &metros);

    // Convertimos los metros a pulgadas (1 pulgada = 0.0254 metros)
    pulgadas = metros / 0.0254;

    // Mostramos el resultado con dos decimales
    printf("Son %.2f pulgadas de tela.\n", pulgadas);

    return 0; // Fin del programa
}
```
3. **Se requiere determinar la hipotenusa de un triángulo rectángulo. ¿Cómo sería el diagrama de flujo y el pseudocódigo que representen el algoritmo para obtenerla? 
Recuerde que por Pitágoras se tiene que: $C^2 = A^2 + B^2$.**

**Pseudocodigo** 
```
Inicio  
Escribir "Ingrese la longitud del cateto A:"  
Leer A  
Escribir "Ingrese la longitud del cateto B:"  
Leer B  
C = SQRT((A*A) + (B*B) )  
Escribir "La hipotenusa del triángulo es: ", C  
Fin 
```
**Codigo en c**
```
#include <stdio.h>  // Librería para entrada y salida de datos
#include <math.h>   // Librería para funciones matemáticas, como sqrt()

int main() {
    float A, B, C;

    // Pedimos al usuario que ingrese la longitud del cateto A
    printf("Ingrese la longitud del cateto A: ");
    scanf("%f", &A);

    // Pedimos al usuario que ingrese la longitud del cateto B
    printf("Ingrese la longitud del cateto B: ");
    scanf("%f", &B);

    // Calculamos la hipotenusa usando el teorema de Pitágoras
    C = sqrt((A * A) + (B * B));

    // Mostramos el resultado con dos decimales
    printf("La hipotenusa del triángulo es: %.2f\n", C);

    return 0; // Fin del programa
}

```
4. **Se requiere determinar la edad actual de una persona basándose en su fecha de nacimiento. Además, es necesario establecer si la persona ya ha cumplido años en el año en curso, si aún no lo ha hecho, o si hoy es su cumpleaños, para celebrarlo. La fecha de nacimiento y la fecha actual estarán representadas mediante tres variables: día, mes y año.**
    
    **Pasos a seguir:**
    
    - Diseñe un algoritmo que permita calcular la edad de la persona.
    - Determine si la persona ya celebró su cumpleaños este año o si aún no lo ha hecho.
    - Verifique si la fecha actual corresponde al día de su cumpleaños. De ser así, imprima el mensaje “Feliz Cumpleaños”.
    - Represente la solución utilizando pseudocódigo claro y estructurado.
**Pseudocodigo** 
```
Inicio  
Escribir "Ingrese su fecha de nacimiento (día, mes, año):"  
Leer dia_nacimiento, mes_nacimiento, año_nacimiento  

Escribir "Ingrese la fecha actual (día, mes, año):"  
Leer dia_actual, mes_actual, año_actual  

edad = año_actual - año_nacimiento  

Si (mes_actual > mes_nacimiento) o (mes_actual = mes_nacimiento y dia_actual >= dia_nacimiento) Entonces  
ya_cumplio = Verdadero  
Sino  
ya_cumplio = Falso  
FinSi  

Si no ya_cumplio Entonces  
edad = edad - 1  
FinSi  

Si (dia_actual = dia_nacimiento) y (mes_actual = mes_nacimiento) Entonces  
Escribir "¡Feliz Cumpleaños!"  
FinSi  
Escribir "La edad actual es: ", edad  

Si ya_cumplio Entonces  
Escribir "Ya celebraste tu cumpleaños este año."  
Sino  
Escribir "Aún no has celebrado tu cumpleaños este año."       
FinSi  
Fin
```
**Codigo en c**
```
#include <stdio.h>  // Librería para entrada y salida de datos

int main() {
    int dia_nacimiento, mes_nacimiento, anio_nacimiento;
    int dia_actual, mes_actual, anio_actual;
    int edad;
    int ya_cumplio; // Usaremos 1 para verdadero y 0 para falso

    // Pedimos la fecha de nacimiento al usuario
    printf("Ingrese su fecha de nacimiento (día, mes, año): ");
    scanf("%d %d %d", &dia_nacimiento, &mes_nacimiento, &anio_nacimiento);

    // Pedimos la fecha actual al usuario
    printf("Ingrese la fecha actual (día, mes, año): ");
    scanf("%d %d %d", &dia_actual, &mes_actual, &anio_actual);

    // Calculamos la edad de forma inicial
    edad = anio_actual - anio_nacimiento;

    // Verificamos si ya cumplió años este año
    if (mes_actual > mes_nacimiento || (mes_actual == mes_nacimiento && dia_actual >= dia_nacimiento)) {
        ya_cumplio = 1; // Verdadero
    } else {
        ya_cumplio = 0; // Falso
    }

    // Si aún no ha cumplido años, restamos 1 a la edad
    if (!ya_cumplio) {
        edad = edad - 1;
    }

    // Verificamos si hoy es su cumpleaños
    if (dia_actual == dia_nacimiento && mes_actual == mes_nacimiento) {
        printf("¡Feliz Cumpleaños!\n");
    }

    // Mostramos la edad calculada
    printf("La edad actual es: %d\n", edad);

    // Indicamos si ya celebró su cumpleaños o no
    if (ya_cumplio) {
        printf("Ya celebraste tu cumpleaños este año.\n");
    } else {
        printf("Aún no has celebrado tu cumpleaños este año.\n");
    }

    return 0; // Fin del programa
}

```

5. **Realice un algoritmo que permita determinar el sueldo semanal de un trabajador con base en las horas trabajadas y el pago por hora, considerando que a partir de la hora número 41 y hasta la 45, cada hora se le paga el doble, de la hora 46 a la 50, el triple, y que trabajar
más de 50 horas no está permitido. Represente el algoritmo mediante pseudocódigo.**

**Pseudocodigo** 
```
Inicio  

Escribir "Ingrese el número de horas trabajadas en la semana:"  
Leer horas_trabajadas  

Escribir "Ingrese el pago por hora:"  
Leer pago_hora  

Si horas_trabajadas > 50 Entonces  
Escribir "No es permitido trabajar más de 50 horas."  
Sino  

Si horas_trabajadas <= 40 Entonces  
sueldo = horas_trabajadas * pago_hora  
Sino  

Si horas_trabajadas <= 45 Entonces  
sueldo = (40 * pago_hora) + ((horas_trabajadas - 40) * pago_hora * 2)  
Sino  
sueldo = (40 * pago_hora) + (5 * pago_hora * 2) + ((horas_trabajadas - 45) * pago_hora * 3)  
FinSi  

FinSi  

Escribir "El sueldo semanal es: ", sueldo  

FinSi  

Fin 
```
**Codigo en c**
```
#include <stdio.h>  // Librería para entrada y salida de datos

int main() {
    int horas_trabajadas;
    float pago_hora, sueldo;

    // Pedimos al usuario el número de horas trabajadas en la semana
    printf("Ingrese el número de horas trabajadas en la semana: ");
    scanf("%d", &horas_trabajadas);

    // Pedimos al usuario el pago por hora
    printf("Ingrese el pago por hora: ");
    scanf("%f", &pago_hora);

    // Si trabajó más de 50 horas, no es permitido
    if (horas_trabajadas > 50) {
        printf("No es permitido trabajar más de 50 horas.\n");
    } else {
        // Si trabajó 40 horas o menos, se paga normal
        if (horas_trabajadas <= 40) {
            sueldo = horas_trabajadas * pago_hora;
        }
        // Si trabajó entre 41 y 45 horas, se paga doble las extras
        else if (horas_trabajadas <= 45) {
            sueldo = (40 * pago_hora) + ((horas_trabajadas - 40) * pago_hora * 2);
        }
        // Si trabajó entre 46 y 50 horas, las extras hasta 45 son dobles y las demás triples
        else {
            sueldo = (40 * pago_hora) + (5 * pago_hora * 2) + ((horas_trabajadas - 45) * pago_hora * 3);
        }

        // Mostramos el sueldo calculado
        printf("El sueldo semanal es: %.2f\n", sueldo);
    }

    return 0; // Fin del programa
}

```
### Pregunta final
**Después de este tutorial, ¿qué puntos crees que deberías reforzar para sentirte más seguro al traducir pseudocódigo a C?**

**R//**  
Siento que debo repasar más sobre cómo hacer cada función en el código y en qué momento usar cada una, para no depender tanto de mirar otros ejemplos e interiorizarlo mejor.
