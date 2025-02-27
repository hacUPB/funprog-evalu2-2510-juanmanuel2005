# RETOS

1. 
Inicio  
Escribir "Ingrese las coordenadas del primer punto (X1, Y1)"  
Leer X1, Y1    
Escribir "Ingrese las coordenadas del segundo punto (X2, Y2)"  
Leer X2, Y2  
D = SQRT ((X1-X2)*(X1-X2)+(Y1-Y2)*(Y1-Y2))  
Escribir "La distancia entre los dos puntos es: ", D  
Fin  
![Diagrama_de_flujo_1](/IMAGENES/Reto%201.png)  

2.   
Inicio     
Escribir "ingrese la cantidad de tela en metros"  
Leer metros   
Pulgadas = metros/0.0254  
Escribir "Son", Pulgadas, "pulgadas de tela."  
Fin  
![Diagrama_de_flujo_2](/IMAGENES/Reto%202.png)  

3.   
Inicio  
Escribir "Ingrese la longitud del cateto A:"  
Leer A  
Escribir "Ingrese la longitud del cateto B:"  
Leer B  
C = SQRT((A*A) + (B*B) )  
Escribir "La hipotenusa del triángulo es: ", C  
Fin  
![Diagrama_de_flujo_3](/IMAGENES/Reto%203.jpg)  

4. 
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


