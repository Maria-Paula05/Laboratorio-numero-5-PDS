)# Laboratorio-numero-5-PDS
# 1.Fundamento teórico:

a.Actividad simpática del sistema nervioso autónomo:

También es conocido por sus siglas como SNS de la misma manera es importante durante el reposo, es clave para preparar al cuerpo durante situaciones de emergencia. Si alguna vez se siente con miedo o ansiedad, bajo ataque o en peligro, simplemente se experimenta la activación del tono simpático. Con el objetivo de preparar para una respuesta de “lucha o huída” ante una emergencia, el sistema nervioso simpático funciona activando diversas y complejas vías donde es evidente el aumento del ritmo cardíaco y respiratorio, presión sanguínea, dilatación de las pupilas, cambios en el flujo sanguíneo para que la sangre salga de la piel, estómago e intestinos para dirigirse hacia el cerebro, el corazón y los diferentes músculos que sean necesarios para llevar a cabo esta respuesta ante la actividad simpática.El SNPS usa adrenalina y noradrenalina como principales neurotransmisores, que actúan sobre los receptores alfa y beta.

b.Actividad parasimpática del sistema nervioso autónomo:

Las funciones del SNPS son comúnmente descritas como la respuesta “descansa y digiere”, debido a que está involucrada en ralentizar el ritmo cardíaco, relajar los esfínteres en los tractos gastrointestinal y urinario y aumentar la actividad glandular e intestinal. El resultado final es el almacenamiento de energía y la regulación de las funciones del cuerpo, tales como la digestión y la micción. Es contrario al sistema nervioso simpático (SNS), cuya función es descrita como la respuesta de “lucha o huida” que ocurre en situaciones de estrés y tiene funciones opuestas principalmente. El SNPS usa acetilcolina como principal neurotransmisor, que actúa sobre los receptores muscarínicos y nicotínicos.

c.Efecto de la actividad simpática y parasimpática en la frecuencia cardiaca:

-Simpático: Aumenta la frecuencia cardíaca y la presión arterial para preparar al cuerpo ante situaciones de estrés o emergencia .​

-Parasimpático: Disminuye la frecuencia cardíaca y la presión arterial, promoviendo un estado de relajación y recuperación .​

c.Variabilidad de la frecuencia cardiaca (HRV) medida como fluctuaciones en el intervalo R-R:

La variabilidad de la frecuencia cardíaca (HRV) es el fenómeno fisiológico de variación en el intervalo de tiempo entre los latidos del corazón. Se mide por la variación en el intervalo latido a latido. HRV representa uno de los marcadores más prometedores del sistema nervioso autónomo (ANS) que se considera ampliamente como una de las mejores métricas objetivas para el estado físico y para determinar la preparación de su cuerpo para el rendimiento.La variabilidad de la frecuencia cardíaca no se refiere a los cambios en la frecuencia cardíaca por minuto en el electrocardiograma, sino que mide las variaciones entre un ciclo cardíaco y el ciclo cardíaco siguiente. Otros términos utilizados incluyen: "variabilidad de la duración del ciclo", "variabilidad R-R" (donde R es un punto que corresponde al pico del complejo QRS de la onda de ECG; y RR es el intervalo entre R sucesivas), y "variabilidad del período cardíaco".La variabilidad de la frecuencia cardíaca está determinada por el tiempo (ms) entre latidos cardíacos, conocido como intervalos R-R. Tenga en cuenta que el tiempo (ms) entre los intervalos R-R cambia continuamente. HRV son ritmos fisiológicos dentro de las oscilaciones del intervalo entre frecuencias cardíacas consecutivas e instantáneas.
En la siguiente imagen se observa la variablidad de cada intervalo R-R en un ECG.
![image](https://github.com/user-attachments/assets/df7ab97d-85d3-469b-80e2-d81e6b9d51f3)

d.Frecuencias de interés en este análisis:
En el análisis de la variabilidad de la frecuencia cardíaca (HRV) en el dominio de la frecuencia, se consideran principalmente tres bandas de interés. La banda de baja frecuencia (LF), que abarca de 0.04 a 0.15 Hz, está relacionada con una combinación de actividad simpática y parasimpática del sistema nervioso autónomo. La banda de alta frecuencia (HF), que va de 0.15 a 0.4 Hz, se asocia principalmente con la actividad parasimpática y está influenciada por la respiración. En algunos casos, también se incluye la banda de muy baja frecuencia (VLF), que va de 0.003 a 0.04 Hz, aunque su interpretación fisiológica es menos clara y su análisis requiere grabaciones más prolongadas. Estas bandas permiten evaluar la modulación autonómica del corazón a partir de las fluctuaciones en los intervalos R-R.
e.Transformada Wavelet:


-Definición:La transformada wavelet es una herramienta matemática que permite descomponer una señal en componentes de diferentes escalas o resoluciones, utilizando funciones denominadas wavelets, que son ondas de corta duración con energía concentrada en el tiempo. A diferencia de la transformada de Fourier, que representa una señal en términos de senos y cosenos (infinitamente largos), la transformada wavelet ofrece una mejor resolución temporal y frecuencial simultáneamente, lo que la hace ideal para analizar señales no estacionarias como las biológicas.

-Usos de transformada Wavelet:Se utiliza en el procesamiento de señales biológicas para:​

Detección de ondas R en señales ECG.

Eliminación de ruido o artefactos en señales como EMG o EEG.

Compresión de señales biológicas para almacenamiento eficiente.

Análisis de variabilidad de frecuencia cardiaca (HRV).

Caracterización de patrones en señales cerebrales o musculares.

-Tipos de wavelets utilizadas en señales biológicas

Entre los tipos de wavelets más utilizados en el análisis de señales biológicas se encuentran varias familias con propiedades distintas. Las Daubechies (dbN) son ampliamente empleadas en señales ECG debido a su buena localización temporal y su capacidad para detectar transitorios. Las Symlet (symN), una variante más simétrica de las Daubechies, son útiles cuando se requiere una mejor reconstrucción de la señal. Las Coiflet (coifN) ofrecen más momentos nulos, lo que permite un análisis más detallado de variaciones suaves. Las Biorthogonal (biorN.N) son empleadas especialmente en compresión y eliminación de ruido gracias a su simetría y capacidad de reconstrucción exacta. Además, algunas wavelets específicas se utilizan por su forma característica: la Morlet, una wavelet compleja con una onda senoidal modulada por una gaussiana, es útil para estudiar componentes oscilatorios como los ritmos cerebrales; la Haar, la más simple, funciona como una función escalón y es eficaz para detectar cambios abruptos; y la Mexican Hat o sombrero mexicano, derivada de una gaussiana, es excelente para detectar picos en señales como el ECG. La elección del tipo de wavelet depende del tipo de señal y del objetivo del análisis, ya sea detección, filtrado, compresión o estudio espectral.

-Diagrama de flujo 


![image](https://github.com/user-attachments/assets/fce332eb-a546-4d40-b88d-96d4cea3838e)

# 2.Adquisición de la señal EMG:

Para lograr tomar la señal de una manera correcta y con una frecuencia de muestreo considerable se usó el sistema de adquisición DAQ el cual fue conectado al sensor mediante conexiones simples y también al computador; el código configurado para adquirir correctamente la señal fue creado en MatLab al cual para que  funcionará se instaló una librería propia de DAQ y el código utilizado es el  siguiente:

```python
rado
grid on;

% ======= INICIO DE ADQUISICIÓN =======
disp('Iniciando adquisición ECG...');
startTime = datetime('now');

for i = 1:numReads
    data = read(d, samplesPerRead, "OutputFormat", "Matrix");
    
    % Tiempo relativo de cada muestra
    t0 = seconds(datetime('now') - startTime);
    t = t0 + (0:samplesPerRead-1)' / sampleRate;
    
    % Acumular datos
    timeVec = [timeVec; t];
    signalVec = [signalVec; data];

    % Actualizar gráfica
    set(h, 'XData', timeVec, 'YData', signalVec);
    drawnow;
end

% ======= GUARDAR LOS DATOS =======
disp('Adquisición finalizada. Guardando archivo...');
T = table(timeVec, signalVec, 'VariableNames', {'Tiempo_s', 'Voltaje_V'});
writetable(T, outputFile);
disp(['ECG guardado en: ', outputFile]);

% ======= LIBERAR DAQ =======
clear d;
```

En este código puede observarse una frecuencia de muestreo de 1Khz lo que indica que deben tomarse 1000 datos por segundo; y el tiempo que se tomó la señal fue de 300 segundos tiempo equivalente a 5 minutos; junto con este pequeño análisis se puede vdecir que se deber►1an tomar 30.000 datos de esta señal lo que fue confirmado conla revisión del archivo .csv que el MatLab creó.A continuación puede descargarse el archivo:

[Señal ECG. csv](https://github.com/Maria-Paula05/Laboratorio-numero-5-PDS/blob/main/emg_signal.csv)

Adicional a esto, se calculó la frecuencia estimada del primer minuto con esta fracción de código,lo que indica que la frecuencia fue capturadade forma correcta:

```python
file_path = "ecg_signal.csv"
df = pd.read_csv(file_path)
tiempo = df.iloc[:, 0]  # Primera columna (Tiempo)
voltaje = df.iloc[:, 1]  # Segunda columna (Voltaje)
# Filtrar solo el primer minuto (tiempo <= 60 s)
mask = tiempo <= 60
tiempo_1min = tiempo[mask]
voltaje_1min = voltaje[mask]
fs_estimates = 1 / tiempo_1min.diff().dropna()
fs_mean = fs_estimates.mean()
plt.figure(figsize=(10, 4))
plt.plot(tiempo_1min, voltaje_1min, label="Señal ECG (Primer minuto)", color="b")
plt.xlabel("Tiempo (s)")
plt.ylabel("Voltaje (V)")
plt.title("Señal ECG (0-60 s)")
plt.legend()
plt.grid(True)
plt.show()
```
En esta imagen puede verse graficada la señal ECG del primer minuto y además de esto la frecuencia estimada:

![image](https://github.com/user-attachments/assets/073c0c78-be1a-4182-b925-64153d27b214)

Frecuencia de muestreo estimada (primer minuto): 990.19 Hz

# 3.Pre-procesamiento de la señal:

# a.Filtro IIR



# b.Ecuación en diferencia del filtro



# d. Identificación de picos R 

# e. Calculo de intervalos R-R

# f. Nueva señal con información anterior


# c.Filtro de la señal aplicado a parametros inciales =0






# 4.Análisis de la HRV en el dominio del tiempo:

 # a. Media de intervalos R-R

 # b. Desviación estandar 


# 5.Aplicación de la Transformada Wavelet:



¿Qué diferencias se observan entre los análisis en el dominio del tiempo y el 
dominio tiempo-frecuencia?
- ¿Qué efecto tiene el uso de diferentes funciones wavelet en los resultados del 
análisis?
- ¿Qué aplicaciones reales tiene esta práctica?
# Referencias


References
Análisis de wavelets. (n.d.). StudySmarter ES. Retrieved April 26, 2025, from https://www.studysmarter.es/resumenes/matematicas/matematicas-aplicadas/analisis-de-wavelets/

Coon, E. (2023, July 3). Introducción al sistema nervioso autónomo. Manuale Merck versión para el público general; Manuales de Merck. https://www.merckmanuals.com/es-us/hogar/enfermedades-cerebrales-medulares-y-nerviosas/trastornos-del-sistema-nervioso-autónomo/introducción-al-sistema-nervioso-autónomo

Guzmán, M., & Navarro, P. B. (2024, December 10). Introducción al sistema nervioso periférico.

Mezoo Co., Ltd. (n.d.). Me-zoo.com. Retrieved April 26, 2025, from https://m.me-zoo.com/main/html.php?htmid=sp%2Fscience%2Fscience6.html

Quiroz-González, S., López-Espinosa, E., Liu, Z., & Fossion, R. (2024). Evidencias de los efectos parasimpáticos y simpáticos de la acupuntura mediante la variabilidad de la frecuencia cardíaca: implicaciones multisistémicas. Revista internacional de acupuntura, 18(1), 100288. https://doi.org/10.1016/j.acu.2024.100288

Serrano, D. C., & Torres, A. (2024, December 10). Introducción al sistema nervioso periférico.
