# ACTIVIDAD 1

## 1.¿Qué es un computador? Escribe una definición oficial y la referencia bibliográfica.

**R/**  
Un computador es una máquina electrónica que está diseñada para realizar tareas específicas. En muchos países se le conoce como computadora u ordenador, pero todas estas palabras se refieren a lo mismo.

### Referencias
[¿Qué es un computador?](https://edu.gcfglobal.org/es/informatica-basica/que-es-un-computador/1/)

## 2. Arquitecturas de un computador: dar una breve definición de qué es una arquitectura de computador. Describir cómo están construidas y en qué equipos modernos se pueden encontrar.  

**R/**    
Se trata de un conjunto de reglas, principios y estándares que definen la estructura y el diseño de los componentes de hardware y software que conforman un sistema informático. Esta disciplina abarca desde el nivel más bajo, como los circuitos electrónicos y la lógica digital, hasta el nivel más alto, como lo son los sistemas operativos y las aplicaciones.

Los principales componentes de la arquitectura de una computadora tienen que ver con las partes que forman un ordenador. Entre ellos se encuentran:  

**CPU:** puede apreciarse como el cerebro de la computadora. Se encarga de ejecutar las instrucciones de los programas y realizar operaciones tanto matemáticas como lógicas. Se compone fundamentalmente por la Unidad de Control (UC) y la Unidad Aritmético-Lógica (ALU).  

**Bus:** tiene que ver con los canales de comunicación que permiten la transferencia de datos entre la CPU, la memoria y los dispositivos de entrada/salida. Usualmente, se dividen en tres tipos: el bus de datos, el de direcciones y el bus de control.  

**Memoria principal:** se trata del espacio de almacenamiento temporal, donde se guardan las instrucciones de los programas y los datos que están siendo procesados. Se divide en celdas o posiciones de memoria, cada una con una dirección única que permite acceder a la información almacenada.   

**Unidad de Entrada/Salida (E/S):** son los dispositivos que permiten la interacción entre el usuario y la computadora. Incluye teclados, mouse o ratón, pantallas, impresoras, discos duros, unidades USB y otros periféricos.  

**Reloj:** consiste en un componente que genera pulsos eléctricos a intervalos regulares, marcando el ritmo de las operaciones de la CPU y sincronizando todos los componentes del sistema.  

**Sistema Operativo:** hace referencia a un software esencial que actúa como intermediario entre el usuario y el hardware. Gestiona los recursos de la computadora, permitiendo la ejecución de programas y tareas.  

Hoy en día existen diversos modelos de arquitectura, cada uno con características distintivas. A continuación, se presentan algunos de los más populares:  

- **Arquitectura de Von Neumann**  
Fue propuesto por el matemático John Von Neumann en la década de 1940. Es una de las arquitecturas fundamentales en el campo, sirvió para la creación de la computadora EDVAC, que ha servido como fundamento para el diseño de ordenadores actuales. Se basa en la idea de tener una unidad central de procesamiento (CPU) que accede a una memoria compartida para almacenar tanto datos como programas. Las instrucciones y datos se guardan en la misma memoria y se recuperan a través de un bus (o canal) común.  
- **Arquitectura Harvard**  
Es un modelo similar a la arquitectura de Von Neumann, pero este se caracteriza por utilizar memorias físicamente separadas para almacenar las instrucciones del programa y los datos de manera independiente. Esto permite que la CPU acceda simultáneamente a ambos, mejorando el rendimiento en ciertas aplicaciones específicas. Se ha usado principalmente en aplicaciones donde se requiere un alto rendimiento en el procesamiento de señales o en tareas específicas donde el acceso simultáneo a instrucciones y datos es ventajoso.  
- **Arquitectura RISC (Reduced Instruction Set Computer)**  
Es un enfoque de diseño de procesadores y computadoras que se caracteriza por utilizar un conjunto de instrucciones reducido y altamente optimizado. Los procesadores RISC ejecutan instrucciones en un solo ciclo de reloj, lo que los hace más eficientes en operaciones simples y repetitivas. Además, pueden alcanzar altos niveles de rendimiento, siendo particularmente útiles en aplicaciones que requieren un procesamiento intensivo, como servidores y supercomputadoras. Su efectividad la ha convertido en la base para muchos procesadores modernos.  
- **Arquitectura CISC (Complex Instruction Set Computer)**  
A diferencia de RISC, los procesadores CISC utilizan un conjunto de instrucciones más amplio y diverso. Estas instrucciones pueden realizar tareas más complejas en un solo ciclo de reloj, lo que facilita la programación, pero puede afectar el rendimiento en ciertos escenarios. Por esta razón, a lo largo del tiempo, se han desarrollado técnicas para mejorar la ejecución de instrucciones CISC, como la segmentación (pipeline) y la ejecución fuera de orden (out-of-order execution).  
- **Arquitectura paralela**  
Es un enfoque de diseño de computadoras que se basa en la utilización de múltiples unidades de procesamiento trabajando en paralelo para realizar tareas y operaciones de manera simultánea. Esto puede lograrse mediante el uso de procesadores multinúcleo o la creación de sistemas con varios procesadores trabajando juntos. Su principal objetivo es mejorar el rendimiento y la eficiencia del sistema informático al dividir las tareas en partes más pequeñas y asignarlas a diferentes procesadores para que trabajen en conjunto.  
- **Arquitectura de la computación en la nube**  
También conocida como arquitectura de nube. Consiste en una estructura tecnológica que permite el acceso a recursos informáticos a través de internet, como almacenamiento, potencia de procesamiento y aplicaciones, sin que los usuarios tengan que poseer o administrar físicamente los equipos y servidores que los proveen. Esta arquitectura es esencial para la provisión de servicios bajo demanda y la escalabilidad de aplicaciones.  

En la actualidad CISC tiene a x86 como su mayor exponente, con AMD y sobre todo Intel a la cabeza de su desarrollo. Hay muchos ejemplos históricos como los PDP, Motorola 68000, Intel 4004 o Intel 8086, quizá los más representativos. Prácticamente cualquier ordenador de sobremesa o portátil desde los años 80 ha utilizado un procesador x86.  

Un procesador de tipo RISC es más simple tanto en software (instrucciones) como en hardware (registros de memoria), lo cual hace que sea un dispositivo notablemente más barato que otras CPU. En la actualidad el mayor ejemplo de procesador RISC son los productos ARM, utilizados ampliamente en dispositivos móviles pero también en otros campos como los supercomputadores. ARM será el principal protagonista de una de nuestras próximas entradas de esta saga  

### Referencias
- [¿Qué es arquitectura de computadoras?](https://global.tiffin.edu/blog/que-es-arquitectura-de-computadoras)
- [Intel 4004: Cuarenta años para la historia](https://www.xataka.com/componentes/intel-4004-cuarenta-anos-para-la-historia)
- [CISC frente a RISC: Una batalla en blanco y negro](https://www.xataka.com/componentes/cisc-frente-a-risc-una-batalla-en-blanco-y-negro)

## 3.¿Qué es el hardware? Incluye los más relevantes, te voy a dar algunos elementos, pero si encuentras más, los puedes incluir.    
### a. CPU. Escribe una definición y sus partes más relevantes.   
    - ALU. Definición y función.  
    - Unidad de control. Definición y función.  
    - Registros. Definición y función.  
    - Buses. Definición y función.  
### b. Memoria  
     - Registros  
    - Caché  
    - Principal (RAM)  
    - Secundaria (Disco duro y unidades externas de almacenamiento)  
### c. Dispositivos de entrada / salida  
### d. Buses de datos  

**R/**  
¿Qué es el hardware?  
El hardware se refiere a los componentes físicos y tangibles de un sistema informático. Incluye elementos como la CPU, la memoria, los dispositivos de entrada y salida, y los buses de datos.  

### a. CPU  
La Unidad Central de Procesamiento (CPU) es el componente principal del hardware que ejecuta instrucciones de los programas.  
- **ALU (Unidad Aritmético-Lógica)**: Se encarga de realizar operaciones matemáticas y lógicas esenciales para el funcionamiento del sistema.  
- **Unidad de control**: Dirige la ejecución de instrucciones, coordinando el flujo de datos dentro de la CPU y entre otros componentes.  
- **Registros**: Son pequeños espacios de memoria dentro de la CPU que almacenan datos temporalmente para procesamiento rápido.  
- **Buses**: Son canales de comunicación que transportan datos, direcciones y señales de control entre la CPU y otros dispositivos.  

### b. Memoria  
La memoria almacena temporal o permanentemente los datos y programas necesarios para el funcionamiento del sistema.  
- **Registros**: Ubicados en la CPU, permiten el acceso rápido a datos críticos.  
- **Caché**: Memoria de alta velocidad que almacena datos utilizados frecuentemente para acelerar el procesamiento.  
- **Principal (RAM)**: Memoria de acceso aleatorio utilizada para cargar y ejecutar programas en tiempo real.  
- **Secundaria**: Dispositivos de almacenamiento como discos duros y unidades externas donde se guardan datos permanentemente.  

### c. Dispositivos de entrada / salida* 
Permiten la comunicación entre el usuario y la computadora. Los dispositivos de entrada incluyen teclados y ratones, mientras que los de salida incluyen monitores e impresoras.  

### d. Buses de datos  
Son los conductos que transportan información entre los distintos componentes del hardware. Incluyen buses de datos, de direcciones y de control.  

### Referencias
- [Qué es el hardware](https://es.wikipedia.org/wiki/Hardware)
- [Unidad Central de Procesamiento (CPU)](https://aws.amazon.com/es/what-is/cpu/)
- [Registros en la CPU](https://es.wikipedia.org/wiki/Unidad_central_de_procesamiento)
- [Buses del sistema](https://es.wikipedia.org/wiki/Bus_(inform%C3%A1tica))
- [Memoria en informática](https://es.wikipedia.org/wiki/Memoria_inform%C3%A1tica)
- [Dispositivos de entrada y salida](https://es.wikipedia.org/wiki/Dispositivo_de_entrada_salida)
- [Almacenamiento de datos](https://es.wikipedia.org/wiki/Almacenamiento_de_datos_computacionales)

## 4. ¿Qué es el software?  
    a. Software de sistema   
    b. Software de aplicación   
    c. Software de desarrollo  

**R/**  
**¿Qué es el software?**  
El software es el conjunto de programas, datos y procedimientos que permiten la realización de tareas específicas en un sistema informático.  

**a. Software de sistema**  
Es el software encargado de gestionar los recursos del hardware y proporcionar servicios básicos a otros programas. Incluye sistemas operativos y utilidades .  
 
**b. Software de aplicación**  
Son los programas diseñados para realizar tareas específicas para los usuarios, como procesadores de texto, navegadores web y aplicaciones multimedia.  

**c. Software de desarrollo**  
Incluye herramientas utilizadas para la creación de programas, como compiladores, editores de texto y entornos de desarrollo integrado (IDE).  

### Referencias
- [Software](https://es.wikipedia.org/wiki/Software)
- [Software de sistema](https://es.wikipedia.org/wiki/Software_de_sistema)
- [Software de aplicación](https://es.wikipedia.org/wiki/Software_de_aplicaci%C3%B3n)
- [Software de programación](https://es.wikipedia.org/wiki/Software_de_programaci%C3%B3n)

## 5. Funcionamiento del computador:  
    a. ¿Qué procesos se llevan a cabo cuando se enciende una computadora?  
    b. ¿Qué sucede desde que ingreso un dato a través del teclado, hasta que veo el resultado de la operación en la pantalla?  
    c. ¿Cómo se codifican los datos internamente en el computador?  
    d. ¿Cuáles son las unidades de medida de datos en un computador? Bit, Byte, etc.  

**R/**  
**a. ¿Qué procesos se llevan a cabo cuando se enciende una computadora?**  

Cuando se enciende una computadora, el proceso de arranque se inicia con el "POST" (Power-On Self-Test). Este proceso revisa el hardware básico de la computadora, como la memoria RAM, el procesador, y la tarjeta gráfica. Después, el BIOS (Basic Input/Output System) o UEFI (Unified Extensible Firmware Interface) toma el control, buscando un sistema operativo para cargar desde el disco duro o SSD. Una vez encontrado el sistema operativo, este se carga en la memoria RAM y comienza a ejecutarse.    

**b. ¿Qué sucede desde que ingreso un dato a través del teclado, hasta que veo el resultado de la operación en la pantalla?**  

Cuando se presiona una tecla en el teclado, una señal eléctrica es enviada al procesador, que a través del controlador de teclado interpreta qué tecla fue presionada. El procesador envía los datos al sistema operativo, que los pasa al programa correspondiente (por ejemplo, una aplicación o navegador). El programa procesa la entrada de datos y produce un resultado, que es finalmente enviado a la tarjeta gráfica. La tarjeta gráfica convierte estos datos en imágenes que se muestran en la pantalla.  

**c. ¿Cómo se codifican los datos internamente en el computador?**  

Los datos en un computador se codifican principalmente en binario, utilizando el sistema de numeración base 2. Cada dato, ya sea texto, imagen o sonido, se convierte en una serie de bits (dígitos binarios). Por ejemplo, las letras se codifican utilizando tablas de codificación como ASCII (American Standard Code for Information Interchange), que asigna un valor binario a cada carácter. Las imágenes y sonidos también se codifican en binario, representando píxeles en imágenes o ondas de sonido en archivos.  

**d. ¿Cuáles son las unidades de medida de datos en un computador? Bit, Byte, etc.**  

Las unidades de medida de datos en un computador incluyen:  

- **Bit (b)**: Es la unidad más pequeña de información en un computador, representando un valor de 0 o 1.  
- **Byte (B)**: Equivale a 8 bits. Un byte es suficiente para representar un carácter de texto.  
- **Kilobyte (KB)**: 1 KB = 1024 bytes.  
- **Megabyte (MB)**: 1 MB = 1024 KB.  
- **Gigabyte (GB)**: 1 GB = 1024 MB.  
- **Terabyte (TB)**: 1 TB = 1024 GB.  

### Referencias:
- [Fuentes de encendido y BIOS](https://www.geeksforgeeks.org/booting-process-in-computers/)
- [Proceso de entrada y salida en una computadora](https://www.explainthatstuff.com/how-computers-work.html)
- [Codificación binaria de datos](https://www.computerhope.com/issues/ch001586.htm)
- [Unidades de medida en informática](https://www.khanacademy.org/computing/computer-science/understanding-computers/a/data-representation)


