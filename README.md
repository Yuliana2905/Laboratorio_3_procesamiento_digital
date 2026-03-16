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

