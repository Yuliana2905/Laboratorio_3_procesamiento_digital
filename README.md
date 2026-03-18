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


# Objetivos

# Objetivo General: 
-Emplear técnicas de análisis espectral para la diferenciación o clasificación de señales de voz según el género. 
# Objetivos Específicos :
-Capturar y procesar señales de voz masculinas y femeninas. 
-Aplicar la Transformada de Fourier como herramienta de análisis espectral de la voz. 
-Extraer parámetros característicos de la señal de voz: frecuencia fundamental, frecuencia media, brillo, intensidad, jitter y shimmer. 
-Comparar las diferencias principales entre señales de voz de hombres y mujeres a partir de su análisis en frecuencia. 
-Desarrollar conclusiones sobre el comportamiento espectral de la voz humana en función del género.

# Procedimiento y resultados
### PARTE A – Adquisición de las señales de voz 
Para el desarrollo de esta práctica, se realizador grabaciones de voz correspondientes a seis individuo, distribuidos en tres hombres y tres mujeres. Cada participante pronunció la misma frase con la duración aproximada de siete segundos, con el fin de garantizar condiciones comparables entre las señales.

Las grabaciones fueron realizada utilizando dispositivos móviles, manteniendo parámetros de adquisición similares, especialmente en términos de frecuencias de muestreo o condiciones ambientales, se procuró minimizar la presencia de ruido externo y evitar la saturación de la señal durante el proceso de captura 

Cada archivo fue almacenado en formato .wav y nombrado de manera identificable según el género y numero del hablante.

```python
pip install numpy matplotlib scipy librosa
```

Las señales adquiridas fueron importadas a Google Colab (phyton) y fueron respresentadas en el doinio del tiempo, estas gragicas permitieron observar la variación de amplitud en función del tiempo para cada señal, estas graficas permitieron observar la variacion de la amplitud en funcion del tiempo para cada señal, se evidencio que todas las señales presentan una duracion aproximada de siete segundos con variaciones en la amplitud asociadas a la intensidad vocal de cada hablante, asi mismo se identificaron pequeñas pausas y posibles componentes de ruido en algunas grabaciones que se atribuyen a condiciones del entorno durabte la adquisición.

```python
import numpy as np
import matplotlib.pyplot as plt
from scipy.io import wavfile

archivos=["AUDIO HOMBRE 1 (1).wav", "HOMBRE 2.wav", "HOMBRE 3.wav"]
señales=[]
frecuencias_muestreo=[]

for archivo in archivos:
    fs, señal=wavfile.read(archivo)

    # convertir a mono si es estéreo
    if len(señal.shape)>1:
        señal=señal[:,0]

    señales.append(señal)
    frecuencias_muestreo.append(fs)

for i, señal in enumerate(señales):
    fs = frecuencias_muestreo[i]
    t = np.arange(len(señal)) / fs

    plt.figure()
    plt.plot(t, señal)
    plt.title(f"Hombre {i+1} - Dominio del tiempo")
    plt.xlabel("Tiempo [s]")
    plt.ylabel("Amplitud")
    plt.show()


```
# Señal de voz de hombres 



<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/ebfe05af-d01a-4219-8b2c-01a21dd535f8" />

<img width="727" height="546" alt="image" src="https://github.com/user-attachments/assets/67e4653c-aaf2-4423-b42b-ed105c23ff72" />

<img width="722" height="536" alt="image" src="https://github.com/user-attachments/assets/ebb68533-55c0-4963-b84b-edecc84a86da" />





4. Importar las señales de voz en Python y graficarlas en el dominio del tiempo. 
5. Calcular la Transformada de Fourier de cada señal y graficar su espectro de 
magnitudes frecuenciales. 
6. Identificar y reportar las siguientes características de cada señal: 
a. Frecuencia fundamental. 
b. Frecuencia media. 
c. Brillo. 
d. Intensidad (energía).

### PARTE B – Medición de Jitter y Shimmer 
1. Seleccione una de las grabaciones realizadas en la Parte A por cada género 
(una voz de hombre y una de mujer). 
- Aplique un filtro pasa-banda en el rango de la voz (80–400 Hz para 
hombres, 150–500 Hz para mujeres) para eliminar ruido no deseado. 
2. Medición del Jitter (variación en la frecuencia fundamental):


- Detecte los periodos de vibración de la señal (usando cruces por cero o picos sucesivos). 
- Calcule los periodos Ti de la señal de voz. 
- Obtenga el jitter absoluto:

 <img width="524" height="147" alt="image" src="https://github.com/user-attachments/assets/7e34ee44-ffa9-448c-b5bf-f5f476f32166" />

- Calcule el jitter relativo (%):

<img width="327" height="86" alt="image" src="https://github.com/user-attachments/assets/d41d5e56-9ef6-40a2-a828-1150dce5e1a9" />

3. Medición del Shimmer (variación en la amplitud): 
- Detecte los picos de amplitud Ai en cada ciclo. 
- Obtenga el shimmer absoluto:

<img width="565" height="135" alt="image" src="https://github.com/user-attachments/assets/e2bc5541-70fe-4b86-ad16-5536dd9af6f7" />


- Calcule el shimmer relativo (%):

<img width="639" height="126" alt="image" src="https://github.com/user-attachments/assets/e1bf0258-2b53-4c57-a8fc-42b8bb019c8a" />


4. Presente los valores obtenidos de jitter y shimmer para cada una de las 6 grabaciones (3 hombres, 3 mujeres).

## PARTE C – Comparación y conclusiones 
Comparar los resultados obtenidos entre las voces masculinas y femeninas.  
1. ¿Qué diferencias se observan en la frecuencia fundamental? 
2. ¿Qué otras diferencias notan en términos de brillo, media o intensidad? 
3. Redactar conclusiones sobre el comportamiento de la voz en hombres y 
mujeres a partir de los análisis realizados. 
4. Discuta la importancia clínica del jitter y shimmer en el análisis de la voz.

## PREGUNTAS PARA LA DISCUSIÓN 
- ¿Cómo es la frecuencia fundamental de la densidad espectral de potencia asociada a una señal de voz masculina con respecto a la que se obtiene a partir de una señal de voz femenina, mayor o menor? ¿Qué hay del valor RMS? 
-¿Qué limitaciones plantea el uso de características como shimmer y jitter para la detección de patologías como disartrias y afasias?

# Diagramas de flujo

## Parte A

## Parte B

## Bibliografia 

-Oppenheim, A. V., Willsky, A. S., & Nawab, S. H. (1997). Signals and Systems. Prentice Hall.


-Rabiner, L. R., & Schafer, R. W. (1978). Digital Processing of Speech Signals. Prentice Hall.


-Deller, J. R., Proakis, J. G., & Hansen, J. H. (2000). Discrete-Time Processing of Speech Signals. IEEE Press.


-Alim, S. A., & Rashid, N. K. A. (2018). Some commonly used speech feature extraction algorithms. IntechOpen.


-Iser, B., Minker, W., & Schmidt, G. (2008). Bandwidth Extension of Speech Signals. Springer




## Bibliografia 




