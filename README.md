# Laboratorio 9: AMPLIFICADOR OPERACIONAL
Nombre: Caillamara Leonardo
## 1. OBJETIVOS

### Objetivo general:
* Elaborar simulaciones de amplificadores operacionales con el fin de que el estudiante comprenda el uso y majo de estos.  
### Objetivos específicos:
*	Hacer uso del software de simulación Multisim para la simulación de circuitos propuestos.
*	Evidenciar que ocurre con la señal de entrada cuando esta sale del amplificador operacional.
*	Identificar aspectos importantes que se deben tomar en cuenta en el uso de amplificadores operacionales

## 2. MARCO TEÓRICO
### Amplificador Operacional

Un amplificador operacional es un componente circuital el cual tiene múltiples usos. En general es usado como, sumador, inversor, e integrador de señales.  Consiste en aplicar un voltaje de entrada el cual será amplificado o reducido dependiendo de la ganancia que este tenga. Los amplificadores operacionales pueden ser de dos tipos. 

* Amplificadores operacionales de lazo abierto
* Amplificadores de lazo cerrado

Los amplificadores de lazo abierto son aquellos que no tienen ningún voltaje de retorno, pero al momento de usarlo su ganancia es extremadamente grande.

Un amplificador de lazo cerrado es aquel que si tiene voltaje de retorno y dependiendo de su reactancia de entrada en relación con la reactancia de retorno será posible modificar la ganancia según se requiera.

![](https://github.com/ArielAGH/Laboratorio9/blob/main/Img/ModeloAmplificador.gif)

![](https://github.com/ArielAGH/Laboratorio9/blob/main/Img/Amplificador.jpg)

![](https://github.com/ArielAGH/Laboratorio9/blob/main/Img/Modelo2.png)

Físicamente el amplificador operacional es encontrado dentro de un circuito integrado como se aprecia en la figura. De manera general para todos los casos un amplificador operacional usa 5 pines de los ocho que tienen estos circuitos los cuales se indican a continuación.

Pin 2: entrada inversora.

Pin 3: entrada no inversora.

Pin 4: alimentación negativa en CC.

Pin 6: Salida de la señal. 

Pin 7: alimentación positiva en CC.

#### Amplificador operacional como inversor

![](https://github.com/ArielAGH/Laboratorio9/blob/main/Img/ModeloComoInversor.png)

Esta configuración provoca que la señal de entrada se invierta en su salida y amplificarla, pero dependiendo de los resistores Rf y Rin es posible invertir únicamente la señal.

#### Amplificador operacional como sumador


![](https://github.com/ArielAGH/Laboratorio9/blob/main/Img/ModeloComoSumador.png)

Esta configuración tiene como salida la suma de todos los voltajes de entrada multiplicada por la ganancia.

#### Amplificador operacional como integrador

![](https://github.com/ArielAGH/Laboratorio9/blob/main/Img/ModeloComoIntegrador.png)

En este tipo de configuración ocurre una disminución de ganancia es decir que la señal en vez de salir amplificada se reduce y dependiendo de su señal de entrada tendrá una señal de salida distinta.   

## 3. EQUIPOS Y MATERIALES

* **Multisim y Proteus:** Programas de simulación de circuitos.
* **Protoboard:** Es una placa de pruebas en la que se pueden insertar elementos electrónicos y cables con los que se arman circuitos sin la necesidad de soldar ninguno de los componentes.
* **Resistencias eléctricas:** Elemento eléctrico que se opone al paso de corriente.
* **Cables puente:** Cables de ayuda para realizar conexiones provisionales.
* **Multímetro:** Es un instrumento analógico o digital portátil que se usa para medir directamente magnitudes eléctricas.
* **Batería o fuente energética:** Dispositivo que provee energía a un circuito al cual es conectado.

## 4. PROCEDIMIENTO

* Construya en el protoboard cada uno de los circuitos de la figura. Muestre simultáneamente las señales de entrada y salida en un osciloscopio. Capture las formas de onda. 
* Determine y analice la relación entre las señales de entrada y salida en cada uno de los circuitos indicados en la figura.
* En todos los casos emplee un amplificador LM741.

![](https://github.com/ArielAGH/Laboratorio9/blob/main/Img/3Modelos.png)

## 5. RESULTADOS
### Resultados obtenidos para el circuito

Circuito 1

![](https://github.com/ArielAGH/Laboratorio9/blob/main/Img/Circuito1.jpg)

Circuito 2

![](https://github.com/ArielAGH/Laboratorio9/blob/main/Img/Circuito2.jpg)

Circuito 3

![](https://github.com/ArielAGH/Laboratorio9/blob/main/Img/Circuito3.jpg)

## 6. ANÁLISIS DE RESULTADOS

Del circuito uno y tres es posible observar que la forma de onda de entrada en la misma que la de salida, pero invertida y amplificada. Invertida porque la configuración de ambos circuitos es la de un amplificador inversor y la de un amplificador sumador e inversor.

En el circuito dos es posible darnos cuenta   si ingresa una forma de onda cuadrada se obtiene una triangular. Esta configuración corresponde a la de un circuito integrador cuya característica es la de que su ganancia es mínima por lo que se obtendrá una reducción de voltaje.

En general se puede decir que cuando un amplificador está configurado para ser inversor si la señal de entrada es positiva en su salida será negativa y viceversa.

## 7. PREGUNTAS

### Anote parámetros técnicos importantes de un amplificador operacional que deben ser tomados en cuenta al momento de utilizarlos en un proyecto.

Para que un amplificador operacional opere correctamente debe estar conectado correctamente como se indica en su propia datasheet, pero principalmente debe tener una alimentaciones positivas y negativas en los pines correspondientes que en el caso de esta práctica serán el pin cuatro para su alimentación negativa y el pin siete para su alimentación positiva.

Al momento de conectar los pines 2 y 3 se debe asegurar de qué tipo de configuración se va a implementar, ambos pines son distintos ya que uno tiene una entrada inversora y el otro no. 

Si el amplificador es de lazo cerrado se debe colocar una carga con el fin de que la corriente de entrada no se dirija a tierra automáticamente sin pasar por el amplificador.

### Investigue las características de amplificadores operacionales distintos a los utilizados en esta práctica.

Existen varios tipo y configuraciones de amplificadores operaciones estas son:

* Amplificador como comparador. - esta configuración es la más simple de todas ya que dependiendo del pin donde esté conectado el voltaje de entrada, el amplificador entregará un voltaje de salida positivo o negativo   que proviene de cada alimentación.
* Amplificador como no inversor. -  Este amplificador únicamente amplifica la señal mas no la invierte, es decir la señal de entada se mantiene en fase con la de salida.

### Investigue otras aplicaciones con circuitos más complejos que utilizan amplificadores operacionales.

Una de las aplicaciones más comunes es la de audio que por lo general se una un amplificador operacional LM 386 el cual dependiendo del circuito se obtiene una ganancia de 20 a 200 unidades  

Una aplicación muy interesante de amplificadores de lazo abierto es su implementación en circuitos de sensores. 


## 8. CONCLUSIONES

En conclusión, el amplificador operacional tiene una infinidad de usos según el circuito lo necesite. Corresponde un estudio más a profundidad para su completa comprensión y uso.

En un amplificador operacional dependiendo de su señal de entrada y su configuración es posible tener un aumento o disminución de voltaje además de un cambio de forma o la inversión de la señal.

La correcta implementación del amplificador operacional brinda una respuesta acorde con lo deseado caso contrario cabe la posibilidad de que se provoque un desperfecto en el circuito.

## 9. BIBLIOGRAFÍA

* Durán, J. (2012). *Electrotecnia*. Barcelona: Editorial Lexus.
* García, A. (2013). *Amplificadores operacionales y su uso en la electrónica*. Obtenido de: http://panamahitek.com/amplificadores-operacionales-y-su-uso-en-la-electronica/ 
* García, V. (2010). *El amplificador operacional*. Obtenido de: https://www.diarioelectronicohoy.com/blog/el-amplificador-operacional
* Thomas, L. (2007). *Principios de circuitos eléctricos*. México: Editorial Pearson.
* Sadiku, M. (2006). *Fundamentos de circuitos eléctricos*. México: McGraw Hill Interamericana.
