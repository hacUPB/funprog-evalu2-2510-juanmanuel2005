# ACTIVIDAD 2

## EJERCICIO 1

### 1. Representación de datos en una computadora
Las computadoras almacenan y procesan datos en formato binario, es decir, usando solo los números 0 y 1. Esto se debe a que los circuitos electrónicos funcionan con dos estados: encendido (1) y apagado (0). Los números se representan con combinaciones de estos bits, mientras que las letras se codifican con sistemas como ASCII o Unicode. Las imágenes y otros archivos multimedia también se convierten en datos binarios, organizados en píxeles o señales digitales.

### 2. Conclusiones sobre el ejercicio 1
Después de hacer el ejercicio, me di cuenta de que la cantidad de estados que se pueden representar con \( N \) bits sigue una fórmula sencilla: \( 2^N \). Es decir, si tenemos 1 bit, hay 2 combinaciones posibles; con 2 bits, hay 4; con 3 bits, hay 8, y así sucesivamente. Esto muestra cómo la cantidad de combinaciones crece exponencialmente al agregar más bits.

### 3. Unidades de almacenamiento en computación

| Unidad     | Abreviatura | Equivalencia  |
|------------|------------|--------------|
| Byte       | B          | 8 bits       |
| Kilobyte   | KB         | 1024 bytes   |
| Megabyte   | MB         | 1024 KB      |
| Gigabyte   | GB         | 1024 MB      |
| Terabyte   | TB         | 1024 GB      |
| Petabyte   | PB         | 1024 TB      |

### 4. Importancia del trabajo de George Boole
El matemático George Boole creó el Álgebra de Boole, que es la base del funcionamiento de los circuitos lógicos en las computadoras. Gracias a su trabajo, hoy en día podemos realizar operaciones con bits, lo que permite que la tecnología digital funcione de manera eficiente. Sin su aporte, los sistemas computacionales no existirían tal como los conocemos.

## EJERCICIO 2

Ahora es tu turno de intentar usar el método. Te voy a proponer varios números binarios y tú vas a convertirlos a decimales utilizando la tabla 3. Recuerda que el subíndice 2 significa que el número es binario (base 2).

- `1010101010₂`
- `11111₂`
- `10000000₂`
- `100100100₂`

### Conversión de binario a decimal

- `1010101010₂` = **682₁₀**
- `11111₂` = **31₁₀**
- `10000000₂` = **128₁₀**
- `100100100₂` = **292₁₀**

### EJERCICIO 2  
Ahora es tu turno. Vas a convertir los siguientes números decimales a binarios. Recuerda que el subíndice 10 significa que el número es decimal (`base 10`).

- `127₁₀`
- `246₁₀`
- `1025₁₀`
- `354₁₀`

### Conversión de decimal a binario

- `127₁₀` = **1111111₂**
- `246₁₀` = **11110110₂**
- `1025₁₀` = **10000000001₂**
- `354₁₀` = **101100010₂**



## EJERCICIO 3 y 4

### 1.C
|Tipo C      | Tamaño de datos de 32 bits | Tamaño de datos de 64 bits  |
|------------|----------------------------|-----------------------------|
| char       | 08 bits                    | 08 bits                     |
| short      | 16 bits                    | 16 bits                     |
| int        | 32 bits                    | 32 bits                     |
| long       | 32 bits                    | 64 bits                     |
| long long  | 64 bits                    | 64 bits                     |
| puntero    | 32 bits                    | 64 bits                     |

[Tipos de datos de c y su tamaño](IMAGENES_AC2/C.png)

### 2.Python
|Tipo Python  | Tamaño de datos de 32 bits             | Tamaño de datos de 64 bits             |
|-------------|----------------------------------------|----------------------------------------|
| int         | Variable (minimo 32 bits)              | Variable (minimo 32 bits)              |
| float       | 64 bits (usa double de c)              | 64 bits (usa double de c)              |
| bool        | 8 bits (internamente un int)           | 8 bits (internamente un int)           |
| str         | Variable (cada carácter usa 8-32 bits) | Variable (cada carácter usa 8-32 bits) |

[Tipos de datos de Python y su tamaño](IMAGENES_AC2/PYTHON.png)

### 3.Java
|Tipo Java      | Tamaño de datos de 32 bits | Tamaño de datos de 64 bits  |
|---------------|----------------------------|-----------------------------|
| byte          | 08 bits                    | 08 bits                     |
| short         | 16 bits                    | 16 bits                     |
| int           | 32 bits                    | 32 bits                     |
| long          | 64 bits                    | 64 bits                     |
| float         | 32 bits                    | 32 bits                     |
| double        | 64 bits                    | 64 bits                     |
| boolean       | 08 bits                    | 08 bits                     |
| char          | 16 bits (Unicode)          | 16 bits (Unicode)           |

[Tipos de datos de java y su tamaño](IMAGENES_AC2/JAVA.png)

### 4.Kotlin
|Tipo Kotlin    | Tamaño de datos de 32 bits | Tamaño de datos de 64 bits  |
|---------------|----------------------------|-----------------------------|
| byte          | 08 bits                    | 08 bits                     |
| short         | 16 bits                    | 16 bits                     |
| int           | 32 bits                    | 32 bits                     |
| long          | 64 bits                    | 64 bits                     |
| float         | 32 bits                    | 32 bits                     |
| double        | 64 bits                    | 64 bits                     |
| boolean       | 08 bits                    | 08 bits                     |
| char          | 16 bits                    | 16 bits                     |

[Tipos de datos de kotlin y su tamaño](IMAGENES_AC2/KOTLIN.png)

## EJERCCIO 5  
Imagina que necesitas almacenar la siguiente información en un programa:

- Un identificador numérico (número entero)
- Una temperatura (valor de punto flotante)
- Un valor lógico (dato booleano)
- Un texto con 10 caracteres.

Se almacena la información cada 10 segundos durante 24 horas. Calcula cuánto espacio total se requiere en memoria para almacenar estos datos. Describe el procedimiento y muestra el resultado final.

**R/**
**Datos a almacenar:**  
- **Identificador numérico (número entero)**: 4 bytes
- **Temperatura (valor de punto flotante)**: 4 bytes
- **Valor lógico (dato booleano)**: 1 byte
- **Texto con 10 caracteres**: 10 bytes

**Paso 1: Calcular el tamaño de cada conjunto de datos**  

Sumamos el espacio que ocupa cada tipo de dato:
- Identificador numérico: 4 bytes
- Temperatura: 4 bytes
- Valor lógico: 1 byte
- Texto con 10 caracteres: 10 bytes

**Tamaño total por conjunto de datos**:  

4 bytes + 4 bytes + 1 byte + 10 bytes = 19 bytes

**Paso 2: Calcular cuántos conjuntos de datos se almacenan en 24 horas**  

En 24 horas, se almacenan datos cada 10 segundos. Primero, calculamos cuántos intervalos de 10 segundos hay en 24 horas:
24 horas × 60 minutos × 60 segundos = 86,400 segundos  

Luego, dividimos entre 10 segundos por intervalo:  
86,400 segundos / 10 segundos/intervalo = 8,640 intervalos  

**Paso 3: Calcular el espacio total en memoria**  

Multiplicamos el número de intervalos por el tamaño de cada conjunto de datos:  
8,640 intervalos × 19 bytes/intervalo = 164,160 bytes  

**Paso 4: Convertir a unidades más grandes**  

Convertimos el espacio a kilobytes (KB), dividiendo entre 1,024:  
164,160 bytes / 1,024 ≈ 160 KB  

**Resultado:**  

El espacio necesario es aproximadamente de 160 KB  

## EJERCCIO 6

**Conclucion**

En este ejercicio, aprendí cómo las computadoras representan y guardan la información. Convertir datos entre bases numéricas, como binario y decimal, me ayudó a entender cómo manejan los datos a nivel básico. También, al estudiar los tipos de datos y su tamaño en diferentes lenguajes de programación, vi la importancia de usar el espacio de almacenamiento de manera eficiente.

Lo más interesante fue darme cuenta de que todo lo que usamos en la tecnología digital, como texto, imágenes y sonidos, se reduce a combinaciones de 0 y 1. Esto demuestra lo importante que es el sistema binario para el funcionamiento de los dispositivos electrónicos. Además, al calcular el espacio necesario para almacenar datos en un día, me sorprendió la cantidad de memoria que se genera en poco tiempo y la necesidad de optimizar los recursos en los sistemas de computadoras.
