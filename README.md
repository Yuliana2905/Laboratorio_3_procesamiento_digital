# Laboratorio 3 procesamiento_digital
# Análisis espectral de la voz
## Integrantes:
### - Liseth Yuliana Clavijo Mesa
### - Adriana Valentina Alarcon Ramirez
### Marzo 2026

# Introduccion:

La voz humana es una señal acústica compleja generada por la vibración de las cuerdas vocales y modulada por el tracto vocal. Esta señal contiene información importante relacionada con características fisiológicas, lingüísticas y emocionales del hablante. Debido a esto, el análisis de la voz se ha convertido en un campo de gran interés dentro del procesamiento digital de señales, ya que permite estudiar y extraer parámetros relevantes que describen su comportamiento y estructura. 

En el análisis de señales de voz es común estudiar tanto su comportamiento en el dominio del tiempo como en el dominio de la frecuencia. El análisis en frecuencia permite identificar los componentes espectrales que conforman la señal, lo cual facilita la extracción de características como la frecuencia fundamental, la frecuencia media, el brillo espectral y la intensidad de la señal. Estas características permiten describir propiedades importantes de la voz y establecer diferencias entre distintos hablantes. 

Una de las herramientas más utilizadas para realizar este tipo de análisis es la Transformada de Fourier, la cual permite descomponer una señal en sus componentes de frecuencia. A partir de esta transformación es posible observar el espectro de la señal y calcular parámetros que describen su comportamiento espectral. Este tipo de análisis es ampliamente utilizado en aplicaciones como reconocimiento de voz, identificación de hablantes y análisis clínico de la voz. 

En esta práctica de laboratorio se realiza la adquisición y análisis de diferentes señales de voz, con el objetivo de estudiar sus características espectrales y comparar las diferencias existentes entre voces masculinas y femeninas. Para ello se emplean herramientas de procesamiento digital de señales que permiten calcular parámetros como la frecuencia fundamental, la frecuencia media, el brillo, la intensidad, así como medidas de estabilidad vocal como el jitter y el shimmer. A partir de estos resultados se busca comprender mejor el comportamiento espectral de la voz humana y su importancia en aplicaciones biomédicas y tecnológicas.

# Marco teórico
## Señales de voz


<img width="1440" height="990" alt="image" src="https://github.com/user-attachments/assets/253e21e6-5edd-4136-8efc-9b2a3380aa06" />


La voz humana es una señal acústica generada por la vibración de las cuerdas vocales y modulada por el tracto vocal, el cual incluye estructuras como la faringe, la cavidad oral y la cavidad nasal. Estas vibraciones producen ondas sonoras que contienen información sobre el hablante, como su tono, timbre e intensidad. Debido a estas características, las señales de voz pueden ser analizadas mediante herramientas del procesamiento digital de señales para estudiar sus propiedades físicas y espectrales.

Las señales de voz presentan un comportamiento complejo debido a la combinación de componentes periódicos y no periódicos. Por esta razón, su análisis permite extraer características que ayudan a describir su estructura y comportamiento, las cuales pueden emplearse en aplicaciones como reconocimiento de voz, identificación de hablantes y análisis clínico de trastornos del habla.

## Análisis de señales en el dominio del tiempo y la frecuencia


<img width="874" height="403" alt="image" src="https://github.com/user-attachments/assets/93fe5dee-ec2e-4cf8-851a-4f284cd0ede4" />


El análisis de una señal puede realizarse en diferentes dominios. En el dominio del tiempo, se observa cómo varía la amplitud de la señal con respecto al tiempo, lo que permite identificar características como duración, presencia de pausas y variaciones de intensidad.
Por otro lado, el dominio de la frecuencia permite analizar los diferentes componentes de frecuencia que forman la señal. Este tipo de análisis es fundamental en el estudio de señales de voz, ya que permite identificar la distribución de energía en el espectro y determinar parámetros que describen sus propiedades acústicas.

## Transformada de Fourier

La Transformada de Fourier es una herramienta matemática ampliamente utilizada en el procesamiento digital de señales. Su función principal es descomponer una señal en sus componentes de frecuencia, permitiendo observar qué frecuencias están presentes en la señal y con qué intensidad aparecen.
En el análisis de señales de voz, la Transformada de Fourier permite obtener el espectro de frecuencias, que muestra la distribución de energía de la señal en función de la frecuencia. A partir de este espectro es posible identificar picos espectrales y calcular características importantes de la voz.

## Frecuencia fundamental (F0)

La frecuencia fundamental, conocida como   F0 , corresponde a la frecuencia más baja generada por la vibración periódica de las cuerdas vocales. Esta frecuencia determina el tono o altura de la voz, es decir, si la voz se percibe como grave o aguda.

Las diferencias fisiológicas entre hombres y mujeres producen variaciones en la frecuencia fundamental. En general, las voces masculinas presentan valores de frecuencia fundamental más bajos que las voces femeninas, debido a que las cuerdas vocales de los hombres suelen ser más largas y gruesas.

## Centroide espectral y brillo

El centroide espectral es una medida que representa el centro de masa del espectro de frecuencias de una señal. Este parámetro describe cómo se distribuye la energía en el espectro y está relacionado con la percepción del brillo o timbre de la voz.
Cuando el centroide espectral tiene valores altos, significa que la mayor parte de la energía de la señal se encuentra concentrada en frecuencias altas. En cambio, valores bajos indican que la energía está concentrada en frecuencias más bajas.

## Intensidad y energía de la señal

La intensidad de una señal de voz está relacionada con la energía o potencia que posee la señal. Una forma común de medir esta característica es mediante el valor RMS (Root Mean Square), el cual representa el valor promedio de la amplitud de la señal y se asocia con la percepción de volumen de la voz.

Este parámetro permite comparar diferentes grabaciones y analizar variaciones en la intensidad de la voz entre distintos hablantes.

## Jitter y Shimmer


<img width="474" height="381" alt="image" src="https://github.com/user-attachments/assets/924d09ca-5f60-43cd-a5da-d9daf697a631" />

El jitter y el shimmer son parámetros que describen la estabilidad de la voz.
El jitter mide la variación de la frecuencia fundamental entre ciclos consecutivos de vibración de las cuerdas vocales. Es decir, evalúa qué tan constante es el periodo de la señal.
El shimmer, por otro lado, mide la variación de la amplitud entre ciclos consecutivos. Este parámetro refleja cambios en la intensidad de la señal producidos por irregularidades en la vibración de las cuerdas vocales.
Estos parámetros son ampliamente utilizados en el análisis clínico de la voz, ya que valores elevados pueden indicar inestabilidad en la producción vocal o posibles alteraciones en el sistema fonador.




