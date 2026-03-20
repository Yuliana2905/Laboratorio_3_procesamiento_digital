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
## Señal de voz de hombres 



<img width="717" height="516" alt="image" src="https://github.com/user-attachments/assets/ebfe05af-d01a-4219-8b2c-01a21dd535f8" />

<img width="727" height="546" alt="image" src="https://github.com/user-attachments/assets/67e4653c-aaf2-4423-b42b-ed105c23ff72" />

<img width="722" height="536" alt="image" src="https://github.com/user-attachments/assets/ebb68533-55c0-4963-b84b-edecc84a86da" />


## Señal de voz mujeres 

<img width="725" height="533" alt="image" src="https://github.com/user-attachments/assets/8d024c3e-600b-4404-b5f2-562dc2903b15" />

<img width="722" height="529" alt="image" src="https://github.com/user-attachments/assets/1515e963-e16a-4c3d-9e9d-b1111759dcda" />

<img width="724" height="528" alt="image" src="https://github.com/user-attachments/assets/1202985e-5727-437b-9dd2-8fda88ee640f" />


Se aplico la transformada rapida de Fourier FFT acada señal con el objetico de obtener su representacion en el dominio de la frecuencia, a partiide de esta transformacion se generaron los espectros de magnitud correspondientes, para una mejor visualización de los componentes espectrales los resultados dieron representadoe en escala semiligaritmica, lo cual permitio resaltar componentes de alta como baja amplitud.

En los espectros obtenidos se identificaron picos dominanres correspondientes a la frecuencia fundamental en cada señal, asi como la presencia de armónicos distribuidos a lo largo del espectro, se observ una mayor concentracion de energía en bajas frecuencias para los voces masculinas, mientras que las voces femenicas presentarpon una distribucion espectral con mayor contenido en frecuencias más altas.

```python
from scipy.fft import fft, fftfreq

resultados=[]

for i, señal in enumerate(señales):
    fs=frecuencias_muestreo[i]
    N=len(señal)

    fft_vals=fft(señal)
    freqs=fftfreq(N, 1/fs)
    mask=freqs>0 #frecuencias positivas
    freqs=freqs[mask]
    fft_vals=fft_vals[mask]
    magnitud=np.abs(fft_vals)
    resultados.append((freqs, magnitud))
    print(f"\nFFT Hombre {i+1}")
    print("Primeros 10 valores de frecuencia:")
    print(freqs[:5])
    print("Primeros 10 valores de magnitud:")
    print(magnitud[:5])


FFT Hombre 1
Primeros 10 valores de frecuencia:
[0.12238903 0.24477807 0.3671671  0.48955614 0.61194517]
Primeros 10 valores de magnitud:
[245128.16220818 246301.43903288  66779.20096766 172010.12909579
 149546.51756808]

FFT Hombre 2
Primeros 10 valores de frecuencia:
[0.11712556 0.23425113 0.35137669 0.46850225 0.58562782]
Primeros 10 valores de magnitud:
[ 97267.63534633 115253.04210141 108852.68008483 142645.45850787
  13060.71698605]

FFT Hombre 3
Primeros 10 valores de frecuencia:
[0.12772502 0.25545004 0.38317505 0.51090007 0.63862509]
Primeros 10 valores de magnitud:
[265656.62790157 397186.22697283 844857.6364096  710903.15710983
 105251.69233926]


FFT Mujer 1
Primeros 10 valores de frecuencia:
[0.1326639  0.26532779 0.39799169 0.53065559 0.66331949]
Primeros 10 valores de magnitud:
[402854.19688342 632663.6091195  647270.53713613 424112.69031802
 459557.16973216]

FFT Mujer 2
Primeros 10 valores de frecuencia:
[0.13702674 0.27405347 0.41108021 0.54810695 0.68513369]
Primeros 10 valores de magnitud:
[185575.20383242 138237.23694912 137726.3182503  300854.25949267
  77546.73802433]

FFT Mujer 3
Primeros 10 valores de frecuencia:
[0.12824055 0.25648109 0.38472164 0.51296218 0.64120273]
Primeros 10 valores de magnitud:
[139508.3856951  173468.29266628 179561.80456479  54818.52322979
  65485.21498979]
```

```phyton
for i, (freqs, magnitud) in enumerate(resultados):

    rango=(freqs>80) & (freqs<300)
    freqs_filtradas=freqs[rango]
    magnitud_filtrada=magnitud[rango]

    f0=freqs_filtradas[np.argmax(magnitud_filtrada)]

    print(f"Hombre {i+1} : Frecuencia fundamental: {f0:.2f} Hz")

Hombre 1 : Frecuencia fundamental: 216.26 Hz
Hombre 2 : Frecuencia fundamental: 215.04 Hz
Hombre 3 : Frecuencia fundamental: 110.48 Hz

Mujer 1 : Frecuencia fundamental: 269.84 Hz
Mujer 2 : Frecuencia fundamental: 275.56 Hz
Mujer 3 : Frecuencia fundamental: 238.14 Hz
```
```phyton
plt.semilogy()
for i,(freqs, magnitud) in enumerate(resultados):
    magnitud=magnitud+1e-10 # evitar log(0)

    #cálculo de F0
    rango=(freqs>80) & (freqs<300)
    freqs_filtradas=freqs[rango]
    magnitud_filtrada=magnitud[rango]
    f0=freqs_filtradas[np.argmax(magnitud_filtrada)]

    plt.semilogy(freqs, magnitud)

    plt.title(f"Hombre {i+1}-Espectro(semilogaritmica)")
    plt.xlabel("Frecuencia [Hz]")
    plt.ylabel("Magnitud (log)")
    plt.xlim(0, 1000)
    plt.grid()

    print(f"Mujer {i+1}: F0 = {f0:.2f}Hz")

    plt.show()

```
## Grafica espectro voz hombres

<img width="709" height="563" alt="image" src="https://github.com/user-attachments/assets/c07133cb-1530-4913-8f52-b85de972fcb2" />

<img width="712" height="563" alt="image" src="https://github.com/user-attachments/assets/f6dc8129-51fd-40c3-a839-555879ccc922" />

<img width="730" height="573" alt="image" src="https://github.com/user-attachments/assets/2d6ad098-6094-41b9-af9c-975c26b3a8e2" />

## Grafica espectro voz mujeres 

<img width="708" height="525" alt="image" src="https://github.com/user-attachments/assets/6010b1e9-10b0-4ce1-9161-de3be23b17ac" />

<img width="718" height="567" alt="image" src="https://github.com/user-attachments/assets/35765e52-fec7-47ec-b318-1d7e108a0751" />

<img width="731" height="570" alt="image" src="https://github.com/user-attachments/assets/37ce6fd3-3fee-47dd-9d5c-912e27fcd683" />


A partir del análisis espectra, se calcularon loas siguientres parámetros característicos para cada señal:

Frecuancia fundamental (FO): determina como la frecuencia con mayor magnitud dentro de rango específico (80-300 Hz para hombres y 150-500 Hz para mujeres) lo cual permitió evital la detección de armónicos o ruido.

Frecuencia media o centroide espectral: calculada como el promedio poderado de las frecuencias presentes en la señal, proporcionado una medida de las distribución de energía en el espectro.

Brillo: asociado directamente al centroide espectral, representa la percepción de claridad o agudeza de la voz 


intensidad (RMS): medida de la energía de la señal en el dominio del tiempo, relacionada con la ampkitud promedio de la señal.


```phyton
tabla_resultados=[]

for i, (freqs, magnitud) in enumerate(resultados):

    señal=señales[i]
    magnitud=np.abs(magnitud) + 1e-10

    rango=(freqs>150) & (freqs<500)
    freqs_filtradas=freqs[rango]
    magnitud_filtrada=magnitud[rango]
    f0=freqs_filtradas[np.argmax(magnitud_filtrada)]


    centroide=np.sum(freqs*magnitud)/np.sum(magnitud)
    rms=np.sqrt(np.mean(señal**2))
    brillo=centroide
    tabla_resultados.append([f"Mujer {i+1}", f0, centroide, brillo, rms])

```
```phyton
for fila in tabla_resultados:
    print(f"\n{fila[0]}")
    print(f"F0: {fila[1]:.2f} Hz")
    print(f"Frecuencia media: {fila[2]:.2f} Hz")
    print(f"Brillo: {fila[3]:.2f} Hz")
    print(f"Intensidad (RMS): {fila[4]:.4f}")


Hombre 1
F0: 216.26 Hz
Frecuencia media: 2328.94 Hz
Brillo: 2328.94 Hz
Intensidad (RMS): 46.9296

Hombre 2
F0: 215.04 Hz
Frecuencia media: 1003.64 Hz
Brillo: 1003.64 Hz
Intensidad (RMS): 31.6328

Hombre 3
F0: 110.48 Hz
Frecuencia media: 2571.51 Hz
Brillo: 2571.51 Hz
Intensidad (RMS): 28.5277
Mujer 1
F0: 269.84 Hz
Frecuencia media: 1322.48 Hz
Brillo: 1322.48 Hz
Intensidad (RMS): 33.4066

Mujer 2
F0: 275.56 Hz
Frecuencia media: 1358.21 Hz
Brillo: 1358.21 Hz
Intensidad (RMS): 28.1623

Mujer 3
F0: 238.14 Hz
Frecuencia media: 1064.55 Hz
Brillo: 1064.55 Hz
Intensidad (RMS): 27.8765
```

En los resultados obtenidos evidencian que las voces masculinas presentan frecuancias fundamentales mas bajas en cojmparacion con las voces femeninas, lo cual es cosistente con las diferencias fisiologicas en las cuerdas vocales.

el analisis del centroide espectral permitio identificar una moyor concentración de energía en frecuencias bajas para las voces masculinas, mientras que las voces femeninas mostraron valores mas elevados, asociados a un mayor contenido de frecuencias altas, la intensidad de las señales vario entre los distintos hablantes, lo cual se atribuya a diferencias de energía vocal duranyte las grabaciones y la distancia del micrófono.

En el caso de las voces femeninas, las frecuencias fundamentales se encuentran dentro del rango esperado (165–255 Hz), con valores ligeramente superiores en algunos casos, lo cual puede atribuirse a variaciones individuales en la voz o a la presencia de componentes armónicos dominantes, para las voces masculinas, se observa que una de las señales (Hombre 3) presenta una frecuencia fundamental de 110.48 Hz, consistente con el rango típico masculino (85–180 Hz). Sin embargo, las otras dos señales presentan valores cercanos a 215 Hz, lo cual sugiere la posible detección de armónicos en lugar de la frecuencia fundamental real, fenómeno común en el análisis espectral cuando la energía de los armónicos supera la del componente fundamental.


### PARTE B – Medición de Jitter y Shimmer 

###### 1. Seleccione una de las grabaciones realizadas en la Parte A por cada género 
(una voz de hombre y una de mujer). 
- Aplique un filtro pasa-banda en el rango de la voz (80–400 Hz para 
hombres, 150–500 Hz para mujeres) para eliminar ruido no deseado.


```phyton
from scipy.signal import butter, filtfilt, find_peaks
# Filtro 
def bandpass(signal, fs, low, high):
    b, a = butter(4, [low/(fs/2), high/(fs/2)], btype='band')
    return filtfilt(b, a, signal)
# Señal hombre 1
signal = señales[0]
fs = frecuencias_muestreo[0]
# Filtrar rango hombre
signal_f = bandpass(signal, fs, 80, 400)
```
### calculos a mano Filtro pasabanda

![capture_temp](https://github.com/user-attachments/assets/b743a38c-7a05-4d24-9a71-603efff735f4)


##### 2. Medición del Jitter (variación en la frecuencia fundamental):
- Detecte los periodos de vibración de la señal (usando cruces por cero o picos sucesivos). 
- Calcule los periodos Ti de la señal de voz. 
- Obtenga el jitter absoluto:

```phyton

jitter_abs = np.mean(np.abs(np.diff(T)))

```


 <img width="524" height="147" alt="image" src="https://github.com/user-attachments/assets/7e34ee44-ffa9-448c-b5bf-f5f476f32166" />
 
- Calcule el jitter relativo (%):

```phyton

jitter_rel = (jitter_abs / np.mean(T)) * 100

```

<img width="327" height="86" alt="image" src="https://github.com/user-attachments/assets/d41d5e56-9ef6-40a2-a828-1150dce5e1a9" />

###### 3. Medición del Shimmer (variación en la amplitud): 
- Detecte los picos de amplitud Ai en cada ciclo. 
- Obtenga el shimmer absoluto:


<img width="565" height="135" alt="image" src="https://github.com/user-attachments/assets/e2bc5541-70fe-4b86-ad16-5536dd9af6f7" />


```phyton
shimmer_abs = np.mean(np.abs(np.diff(A)))
```


- Calcule el shimmer relativo (%):
<img width="639" height="126" alt="image" src="https://github.com/user-attachments/assets/e1bf0258-2b53-4c57-a8fc-42b8bb019c8a" />

```phyton
shimmer_rel = (shimmer_abs / np.mean(A)) * 100
```


#### Valores obtenidos:

Hombres

<img width="254" height="50" alt="image" src="https://github.com/user-attachments/assets/a737e067-11f9-4a4f-89e0-ebeb535cbb26" />

Mujer

<img width="334" height="88" alt="image" src="https://github.com/user-attachments/assets/dab53fc3-e85b-4bc6-9a43-ab1f6e69bd7d" />


###### 4. Presente los valores obtenidos de jitter y shimmer para cada una de las 6 grabaciones (3 hombres, 3 mujeres).

```phyton
import numpy as np
from scipy.io import wavfile
from scipy.signal import butter, filtfilt, find_peaks
def bandpass(signal, fs, low, high):
    b, a = butter(4, [low/(fs/2), high/(fs/2)], btype='band')
    return filtfilt(b, a, signal)
def jitter_shimmer(signal, fs, low, high):
    signal_f = bandpass(signal, fs, low, high)
    peaks, _ = find_peaks(signal_f, height=0)
    if len(peaks) < 3:
        return None, None
    t = peaks / fs
    T = np.diff(t)
    A = signal_f[peaks]
    jitter = np.mean(np.abs(np.diff(T))) / np.mean(T) * 100
    shimmer = np.mean(np.abs(np.diff(A))) / np.mean(A) * 100
    return jitter, shimmer
archivos_hombres = ["AUDIO HOMBRE 1 (1).wav", "HOMBRE 2.wav", "HOMBRE 3.wav"]
archivos_mujeres = ["AUDIO MUJER 1.wav", "MUJER 2.wav", "MUJER 3.wav"]
print("RESULTADOS JITTER Y SHIMMER HOMBRES ")
for i, archivo in enumerate(archivos_hombres):
    fs, señal = wavfile.read(archivo)
    if len(señal.shape) > 1:
        señal = señal[:,0]
    jitter, shimmer = jitter_shimmer(señal, fs, 80, 400)
    print(f"\nHombre {i+1}")
    print(f"Jitter (%): {jitter:.4f}")
    print(f"Shimmer (%): {shimmer:.4f}")
print("\n RESULTADOS JITTER Y SHIMMER MUJERES ")
for i, archivo in enumerate(archivos_mujeres):
    fs, señal = wavfile.read(archivo)
    if len(señal.shape) > 1:
        señal = señal[:,0]
    jitter, shimmer = jitter_shimmer(señal, fs, 150, 500)
    print(f"\nMujer {i+1}")
    print(f"Jitter (%): {jitter:.4f}")
    print(f"Shimmer (%): {shimmer:.4f}")
```

## Valores obtenidos 
<img width="306" height="467" alt="image" src="https://github.com/user-attachments/assets/5c51d372-21c0-4ce3-a300-0d87887318bc" />

##### Hombre 1

El valor de jitter obtenido para el Hombre 1 (36.4693%) es considerablemente alto respecto a los valores normales, lo que indica una gran variabilidad en la frecuencia de la voz y, por tanto, una inestabilidad en la vibración de las cuerdas vocales. De igual forma, el shimmer (88.2101%) también es extremadamente elevado, evidenciando una fuerte variación en la amplitud de la señal. Estos resultados sugieren que la señal presenta irregularidades importantes, probablemente asociadas a ruido, condiciones de grabación no controladas o ausencia de una vocal sostenida adecuada, por lo que no representan un comportamiento fisiológico normal.

##### Hombre 2

Para el Hombre 2, el jitter (32.0216%) sigue siendo muy superior a los rangos esperados, indicando inestabilidad en la frecuencia de la señal de voz. El shimmer (99.1944%) es igualmente elevado, lo que refleja una gran variabilidad en la amplitud. En conjunto, estos valores evidencian una señal altamente irregular, lo que sugiere la presencia de factores externos como ruido o errores en la adquisición de la señal, limitando su validez para un análisis clínico confiable.

##### Hombre 3

En el caso del Hombre 3, el jitter (33.7516%) mantiene la tendencia de valores elevados, indicando variaciones significativas en el periodo de vibración. El shimmer (120.6437%) es el más alto entre los hombres, lo que evidencia una inestabilidad muy marcada en la amplitud de la señal. Estos resultados refuerzan la idea de que la señal analizada presenta alteraciones importantes, posiblemente derivadas de condiciones no ideales de grabación o procesamiento.

##### Mujer 1

La Mujer 1 presenta un jitter de 17.0481%, el cual, aunque menor que en los hombres, sigue siendo considerablemente alto en comparación con los valores normales. El shimmer (46.6908%) también supera ampliamente los rangos esperados, indicando variabilidad en la amplitud de la señal. Esto sugiere que la voz analizada presenta inestabilidad, posiblemente influenciada por factores externos más que por condiciones fisiológicas reales.

##### Mujer 2

Para la Mujer 2, el jitter (16.1499%) muestra una ligera disminución respecto a las otras grabaciones, pero continúa siendo elevado. El shimmer (47.8819%) mantiene un nivel alto, indicando variaciones en la intensidad de la señal. En conjunto, estos valores reflejan una señal con irregularidades, posiblemente asociadas a la calidad de la grabación o al método de análisis.

##### Mujer 3

En el caso de la Mujer 3, el jitter (18.6766%) vuelve a incrementarse ligeramente, indicando variabilidad en la frecuencia de la voz. El shimmer (62.3753%) también es elevado, mostrando inestabilidad en la amplitud. Estos resultados, aunque menores que en los hombres, siguen estando por encima de los rangos normales, lo que sugiere que la señal no es completamente representativa de una voz fisiológicamente estable.

# SNR 
Aunque las señales originales ya contienen ruido debido al proceso de adquisición, se decidió añadir ruido adicional de forma controlada con el fin de evaluar la sensibilidad del análisis frente a la degradación de la señal. Esto permitió evidenciar cómo el ruido afecta la identificación de la frecuencia fundamental y altera parámetros como jitter y shimmer, demostrando la importancia de trabajar con señales de buena calidad.
### HOMBRES
1
<img width="708" height="493" alt="image" src="https://github.com/user-attachments/assets/2d6f9b39-d337-47d7-b010-c4974edf9872" />
2
<img width="690" height="445" alt="image" src="https://github.com/user-attachments/assets/d8428574-2da0-42dc-8df2-22071ecefba2" />
3
<img width="613" height="482" alt="image" src="https://github.com/user-attachments/assets/ab78d380-0e14-40eb-a100-192235b9ca41" />

### MUJERES
1

<img width="652" height="461" alt="image" src="https://github.com/user-attachments/assets/661c0c48-c3a6-4dce-9646-45ffc281b12d" />

2

<img width="656" height="499" alt="image" src="https://github.com/user-attachments/assets/10be62fd-d1c6-4e8b-a9ab-d35d517e2c8f" />


3

<img width="634" height="461" alt="image" src="https://github.com/user-attachments/assets/4c31cb95-05ca-4370-a420-9c5ea6320b87" />


En el análisis realizado se evidencian diferencias claras entre las voces masculinas y femeninas tanto en el dominio del tiempo como en el dominio de la frecuencia. Las voces masculinas presentan una frecuencia fundamental (F0) menor, lo que se traduce en un tono más grave, mientras que las voces femeninas muestran una F0 mayor, generando un tono más agudo. Esto se debe a diferencias fisiológicas en las cuerdas vocales, como su longitud y masa.

En el dominio del tiempo, las señales femeninas tienden a presentar oscilaciones más rápidas, mientras que las masculinas muestran variaciones más lentas. En el dominio de la frecuencia, esto se refleja en que las voces femeninas concentran su energía en frecuencias más altas, mientras que las masculinas lo hacen en frecuencias más bajas.

Adicionalmente, parámetros como el centroide espectral (brillo) suelen ser mayores en las voces femeninas, indicando una mayor presencia de componentes de alta frecuencia. En cuanto a la intensidad (RMS), no se observa una diferencia tan marcada por género, ya que depende más de la forma en que se realizó la grabación.

Finalmente, el análisis con ruido (SNR) evidencia que tanto las voces masculinas como femeninas pueden verse afectadas por interferencias, dificultando la identificación de características como la frecuencia fundamental y alterando la estabilidad de la señal.

## PARTE C – Comparación y conclusiones 
Comparar los resultados obtenidos entre las voces masculinas y femeninas.  
1. ¿Qué diferencias se observan en la frecuencia fundamental?

Se observa que las voces femeninas presentan frecuencias fundamentales mas altas en comparacion con las voces masculinas, en los resultados otenuudos las mijeres presentas valores FO entre aproximadamente 238 y 276 HZ los cual se encuentra dentro del rango esperado para la voz femenina por otro lad, las voces masculinas deberian ubicarse en un rango mas bajo entre 85 y 180 Hz sin embargo en algunos valores se obtivo 178 Hz esto sugiere pposibles errores en la detección, asociados a la identificacion de armonicos en lugar de frecuencias reales, este diferencias se debe a factores fisiologicos, ya que las mujeres poseen cuerdas vocales mas cortas y delgadas lo que genera una mayor frecuencias de vibracion y un tomo más agudo.


2. ¿Qué otras diferencias notan en términos de brillo, media o intensidad?

Se evidencia que las voces femeninas presentan valores elevados de frecuencia media 1064 a 1358 Hz lo que indica una mayor concentracion de energía en frecuencias altas, esto se traduce a una precepción de voz mas brillante o aguda, en las voces masculinas se observan valores incluso mas altos en algunos casos superiores a 2000 hz esto se puede atribuir a ruidos, irregularidades de la reñal o caracteristicas particulares de la voz qiue incrementan la frecuencia.
En terminos de intensidad, se observan variaciones entre los hablamtes algunas voces masculinas presentas RMS mas altos indicando mayor energía en la señal, en las voces femeninas se muestran valores mas moderados y homogeneos.
Estas diferencias pueden deberse afactores como la fuerza con la que se emite la voz, la distancia del microfono o las condiciones de grabación, la intensidad no depende unicamente del género, sino tambien de las condiciones experimentales.
   
3. Redactar conclusiones sobre el comportamiento de la voz en hombres y mujeres a partir de los análisis realizados.
   
-A partir del análisis realizado en el dominio de la frecuencia y del cálculo de parámetros espectrales, se evidencian diferencias claras entre las voces masculinas y femeninas. En general, las voces masculinas presentan una frecuencia fundamental (F0) menor, lo cual se asocia con la mayor longitud y masa de las cuerdas vocales. Por el contrario, las voces femeninas muestran valores de F0 más altos, generando un tono más agudo.

En cuanto a las características espectrales, se observó que el centroide espectral (brillo) tiende a ser mayor en las voces femeninas, lo que indica una mayor concentración de energía en frecuencias altas. Asimismo, la intensidad de la señal (RMS) puede variar entre individuos, pero no presenta una diferencia tan marcada por género como la frecuencia fundamental.

Respecto a la estabilidad de la señal, los valores de jitter y shimmer permiten evaluar la regularidad en la vibración de las cuerdas vocales. En condiciones normales, estos valores se mantienen bajos, lo que indica una producción vocal estable. Las variaciones observadas entre las grabaciones pueden estar asociadas a factores como la calidad de la grabación, ruido ambiental o diferencias individuales en la producción de la voz.

5. Discuta la importancia clínica del jitter y shimmer en el análisis de la voz.

El jitter y el shimmer son parámetros ampliamente utilizados en el análisis clínico de la voz, ya que permiten evaluar la estabilidad y calidad de la vibración de las cuerdas vocales. El jitter mide las variaciones en la frecuencia fundamental, mientras que el shimmer cuantifica las variaciones en la amplitud de la señal.
Desde el punto de vista clínico, valores elevados de jitter pueden indicar irregularidades en el periodo de vibración, lo cual puede estar asociado a trastornos como disfonías, fatiga vocal o alteraciones neuromusculares. De manera similar, un shimmer elevado puede reflejar inestabilidad en la amplitud de la señal, lo que puede relacionarse con patologías que afectan el control de la voz.
Estos parámetros son especialmente útiles en la detección temprana y seguimiento de enfermedades vocales, ya que permiten cuantificar cambios que no siempre son perceptibles de forma auditiva. Además, son utilizados en la evaluación de pacientes antes y después de tratamientos médicos o terapias de rehabilitación vocal.
## PREGUNTAS PARA LA DISCUSIÓN 

- ¿Cómo es la frecuencia fundamental de la densidad espectral de potencia asociada a una señal de voz masculina con respecto a la que se obtiene a partir de una señal de voz femenina, mayor o menor? ¿Qué hay del valor RMS?

La frecuencia fundamental de la voz masculina es menor que la voz femenina, esto se debe a que las cuerdad vocales masculinas son mas largas y más gruesas, lo que produce una vibración mpas lenta por lo tanto frecuencias ,as bajas, en contraste las voces femeninas presentana frecuencias fundamentales mas altas debido a cuerdas vocales más cortas y delgadas en terminos tipicos los hombres tiene una frecuencia entre 85 y 180 Hz miesntras que las muijeres entre 165-255 Hz

En el caso del valor RMS intensidas a diferencia de la frecuencia fundamental el RMS depende principalmente de la energía de la señal, la intensidad con la que se habla, la distancia al microfono, las condiciones de grabacion, por lo tanto pueden haber voces masculinas con mayor RMS o voces femeninas con mayor RMS, no existe una diferencias sistemática entre géneros, ya que  este depende principalmente de la intensidad de la señal y condiciones externas 

  
-¿Qué limitaciones plantea el uso de características como shimmer y jitter para la detección de patologías como disartrias y afasias?


El uso de parámetros como el jitter y el shimmer presenta varias limitaciones en la detección de patologías del habla como las disartrias y las afasias, debido a que estos indicadores evalúan únicamente la estabilidad de la vibración de las cuerdas vocales y no otros aspectos complejos del lenguaje.
En primer lugar, tanto el jitter como el shimmer se centran en características acústicas de la señal, por lo que son más sensibles a alteraciones en la fonación. Sin embargo, patologías como la afasia están relacionadas principalmente con procesos cognitivos y lingüísticos (comprensión y producción del lenguaje), lo que implica que estos parámetros no son suficientes para su identificación.
En el caso de la disartria, aunque sí existe un componente motor que afecta la producción del habla, esta condición involucra múltiples factores como la articulación, la respiración y la coordinación neuromuscular. Por lo tanto, el jitter y el shimmer solo capturan una parte limitada del problema, sin reflejar completamente la severidad o el tipo de alteración.
Otra limitación importante es la sensibilidad al ruido y a la calidad de la grabación. Variaciones en el entorno, el micrófono o la señal pueden alterar significativamente los valores de jitter y shimmer, generando resultados poco confiables o difíciles de interpretar.
Además, existe una alta variabilidad interindividual, ya que factores como la edad, el género y las características propias de cada hablante influyen en estos parámetros, lo que dificulta establecer umbrales universales para diagnóstico clínico.

# Diagramas de flujo

## Parte A

<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/b0f97905-c3e7-4c12-b3a5-18be7ec820b7" />


## Parte B

<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/7dc56c60-3733-49b3-babf-fb0df4d8becc" />


## Bibliografia 

-Oppenheim, A. V., Willsky, A. S., & Nawab, S. H. (1997). Signals and Systems. Prentice Hall.


-Rabiner, L. R., & Schafer, R. W. (1978). Digital Processing of Speech Signals. Prentice Hall.


-Deller, J. R., Proakis, J. G., & Hansen, J. H. (2000). Discrete-Time Processing of Speech Signals. IEEE Press.


-Alim, S. A., & Rashid, N. K. A. (2018). Some commonly used speech feature extraction algorithms. IntechOpen.


-Iser, B., Minker, W., & Schmidt, G. (2008). Bandwidth Extension of Speech Signals. Springer





