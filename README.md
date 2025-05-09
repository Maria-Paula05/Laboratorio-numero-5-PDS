# Laboratorio-numero-5-PDS

# 1.Fundamento teórico:

a.Actividad simpática del sistema nervioso autónomo:

También es conocido por sus siglas como SNS de la misma manera es importante durante el reposo, es clave para preparar al cuerpo durante situaciones de emergencia. Si alguna vez se siente con miedo o ansiedad, bajo ataque o en peligro, simplemente se experimenta la activación del tono simpático. Con el objetivo de preparar para una respuesta de “lucha o huída” ante una emergencia, el sistema nervioso simpático funciona activando diversas y complejas vías donde es evidente el aumento del ritmo cardíaco y respiratorio, presión sanguínea, dilatación de las pupilas, cambios en el flujo sanguíneo para que la sangre salga de la piel, estómago e intestinos para dirigirse hacia el cerebro, el corazón y los diferentes músculos que sean necesarios para llevar a cabo esta respuesta ante la actividad simpática.El SNPS usa adrenalina y noradrenalina como principales neurotransmisores, que actúan sobre los receptores alfa y beta.

b.Actividad parasimpática del sistema nervioso autónomo:

Las funciones del SNPS son comúnmente descritas como la respuesta “descansa y digiere”, debido a que está involucrada en ralentizar el ritmo cardíaco, relajar los esfínteres en los tractos gastrointestinal y urinario y aumentar la actividad glandular e intestinal. El resultado final es el almacenamiento de energía y la regulación de las funciones del cuerpo, tales como la digestión y la micción. Es contrario al sistema nervioso simpático (SNS), cuya función es descrita como la respuesta de “lucha o huida” que ocurre en situaciones de estrés y tiene funciones opuestas principalmente. El SNPS usa acetilcolina como principal neurotransmisor, que actúa sobre los receptores muscarínicos y nicotínicos.

c.Efecto de la actividad simpática y parasimpática en la frecuencia cardiaca:

-Simpático: Aumenta la frecuencia cardíaca y la presión arterial para preparar al cuerpo ante situaciones de estrés o emergencia .​

-Parasimpático: Disminuye la frecuencia cardíaca y la presión arterial, promoviendo un estado de relajación y recuperación .​

d.Variabilidad de la frecuencia cardiaca (HRV) medida como fluctuaciones en el intervalo R-R:

La variabilidad de la frecuencia cardíaca (HRV) es el fenómeno fisiológico de variación en el intervalo de tiempo entre los latidos del corazón. Se mide por la variación en el intervalo latido a latido. HRV representa uno de los marcadores más prometedores del sistema nervioso autónomo (ANS) que se considera ampliamente como una de las mejores métricas objetivas para el estado físico y para determinar la preparación de su cuerpo para el rendimiento.La variabilidad de la frecuencia cardíaca no se refiere a los cambios en la frecuencia cardíaca por minuto en el electrocardiograma, sino que mide las variaciones entre un ciclo cardíaco y el ciclo cardíaco siguiente. Otros términos utilizados incluyen: "variabilidad de la duración del ciclo", "variabilidad R-R" (donde R es un punto que corresponde al pico del complejo QRS de la onda de ECG; y RR es el intervalo entre R sucesivas), y "variabilidad del período cardíaco".La variabilidad de la frecuencia cardíaca está determinada por el tiempo (ms) entre latidos cardíacos, conocido como intervalos R-R. Tenga en cuenta que el tiempo (ms) entre los intervalos R-R cambia continuamente. HRV son ritmos fisiológicos dentro de las oscilaciones del intervalo entre frecuencias cardíacas consecutivas e instantáneas.
En la siguiente imagen se observa la variablidad de cada intervalo R-R en un ECG.

![image](https://github.com/user-attachments/assets/df7ab97d-85d3-469b-80e2-d81e6b9d51f3)

e.Frecuencias de interés en este análisis:

En el análisis de la variabilidad de la frecuencia cardíaca (HRV) en el dominio de la frecuencia, se consideran principalmente tres bandas de interés. La banda de baja frecuencia (LF), que abarca de 0.04 a 0.15 Hz, está relacionada con una combinación de actividad simpática y parasimpática del sistema nervioso autónomo. La banda de alta frecuencia (HF), que va de 0.15 a 0.4 Hz, se asocia principalmente con la actividad parasimpática y está influenciada por la respiración. En algunos casos, también se incluye la banda de muy baja frecuencia (VLF), que va de 0.003 a 0.04 Hz, aunque su interpretación fisiológica es menos clara y su análisis requiere grabaciones más prolongadas. Estas bandas permiten evaluar la modulación autonómica del corazón a partir de las fluctuaciones en los intervalos R-R.

f.Transformada Wavelet:

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

En este código puede observarse una frecuencia de muestreo de 1Khz lo que indica que deben tomarse 1000 datos por segundo; y el tiempo que se tomó la señal fue de 300 segundos tiempo equivalente a 5 minutos; junto con este pequeño análisis se puede vdecir que se deber►1an tomar 30.000 datos de esta señal lo que fue confirmado conla revisión del archivo .csv que el MatLab creó.

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

a.Filtro IIR:

En esra sección se separó el minuto  1 y 3 ya que el primero el sujeto de prueba se encontraba en reposo y en el 3 estaba sometido a estres y se quiere analizar cambio en frecuencia cardíaca:

-Filtro de señal de primer minuto
````python
def butter_bandpass(lowcut, highcut, fs, order=4):
    nyq = 0.5 * fs
    Wn = [lowcut / nyq, highcut / nyq]
    b, a = butter(order, Wn, btype='band')
    return b, a

# Aplicar el filtro a los datos
def apply_filter(data, lowcut, highcut, fs):
    b, a = butter_bandpass(lowcut, highcut, fs)
    return lfilter(b, a, data)

# Parámetros
fs = 1000  # Frecuencia de muestreo (en Hz), ajusta según tu señal
lowcut = 0.5  # Frecuencia de corte baja
highcut = 40  # Frecuencia de corte alta

# Filtrar la señal ECG
filtered_ecg = apply_filter(voltaje_1min.values, lowcut, highcut, fs)

# Graficar la señal original y la filtrada
plt.figure(figsize=(10, 6))
plt.subplot(2, 1, 1)
plt.plot(voltaje_1min.values, label='Señal Original')
plt.title('Señal Original de ECG')
plt.xlabel('Muestras')
plt.ylabel('Voltaje')
plt.grid(True)

plt.subplot(2, 1, 2)
plt.plot(filtered_ecg, label='Señal Filtrada', color='r')
plt.title('Señal Filtrada con Filtro IIR')
plt.xlabel('Muestras')
plt.ylabel('Voltaje')
plt.grid(True)

plt.tight_layout()
plt.show()
`````
![image](https://github.com/user-attachments/assets/1f89b686-c55b-4319-8dcb-505276c84c51)

-Filtro de señal de tercer minuto:

```python
fs_estimates = 1 / tiempo_3min.diff().dropna()
fs_mean = fs_estimates.mean()
def butter_bandpass(lowcut, highcut, fs, order=4):
    nyq = 0.5 * fs
    Wn = [lowcut / nyq, highcut / nyq]
    b, a = butter(order, Wn, btype='band')
    return b, a

def apply_filter_iir(data, b, a):
    y = np.zeros_like(data)
    for n in range(len(data)):
        y[n] = b[0] * data[n]
        for i in range(1, len(b)):
            if n - i >= 0:
                y[n] += b[i] * data[n-i]
        for i in range(1, len(a)):
            if n - i >= 0:
                y[n] -= a[i] * y[n-i]
    return y

lowcut = 0.5  
highcut = 40  

b, a = butter_bandpass(lowcut, highcut, fs_mean)

filtered_ecg_3min = apply_filter_iir(voltaje_3min.values, b, a)

# Graficar la señal original y la filtrada
plt.figure(figsize=(10, 6))
plt.subplot(2, 1, 1)
plt.plot(tiempo_3min, voltaje_3min, label='Señal Original (Tercer minuto)', color='b')
plt.title('Señal ECG (120-180 s)')
plt.xlabel('Tiempo (s)')
plt.ylabel('Voltaje (V)')
plt.grid(True)
plt.subplot(2, 1, 2)
plt.plot(tiempo_3min, filtered_ecg_3min, label='Señal Filtrada (IIR)', color='r')
plt.title('Señal Filtrada del Tercer Minuto')
plt.xlabel('Tiempo (s)')
plt.ylabel('Voltaje (V)')
plt.grid(True)
plt.tight_layout()
plt.show()
print(f"Frecuencia de muestreo estimada (tercer minuto): {fs_mean:.2f} Hz")
````
![image](https://github.com/user-attachments/assets/5b723233-545e-4e3e-90bb-b05ac633a5a6)

b. Identificación de picos R

```python
min_dist = int(0.3 * fs)
prominence = 0.3

peaks, _ = find_peaks(filtered_ecg, distance=min_dist, prominence=prominence)

# --- Calcular frecuencia cardíaca total ---
n_latidos = len(peaks)
frecuencia_total = n_latidos / 1  # en 1 minuto
print(f"\n→ Se detectaron {n_latidos} latidos en 60 segundos")
print(f"→ Frecuencia cardíaca total estimada: {frecuencia_total:.2f} latidos por minuto")
# --- Gráfica: señal ECG con picos R ---
plt.figure(figsize=(12, 4))
plt.plot(tiempo_1min, filtered_ecg, label='ECG Filtrada')
plt.plot(tiempo_1min.values[peaks], filtered_ecg[peaks], "ro", label='Picos R')
plt.title("Detección de Picos R")
plt.xlabel("Tiempo (s)")
plt.ylabel("Voltaje (V)")
plt.grid()
plt.legend()
plt.show()
````
![image](https://github.com/user-attachments/assets/75bba985-5978-40cf-b5f5-297e219a458d)

Se detectaron 56 latidos en 60 segundos
Frecuencia cardíaca total estimada: 56.00 latidos por minuto

-Señal de tercer minuto
```python
# Detección de picos R con parámetros de distancia y prominencia ajustados
min_dist = int(0.3 * fs_mean)  # Distancia mínima entre picos (0.2 segundos * frecuencia de muestreo)
prominence = 0.1  # Prominencia mínima de los picos (más baja)

# Detectar los picos R
peaks, _ = find_peaks(filtered_ecg_3min, distance=min_dist, prominence=prominence)

# Calcular la frecuencia cardíaca total
n_latidos = len(peaks)  # Número de picos R detectados
frecuencia_total = n_latidos / 1  # En 1 minuto

# Imprimir resultados
print(f"\n→ Se detectaron {n_latidos} latidos en 60 segundos")
print(f"→ Frecuencia cardíaca total estimada: {frecuencia_total:.2f} latidos por minuto")

# Graficar la señal ECG filtrada con los picos R detectados
plt.figure(figsize=(12, 4))
plt.plot(tiempo_3min, filtered_ecg_3min, label='ECG Filtrada')
plt.plot(tiempo_3min.values[peaks], filtered_ecg_3min[peaks], "ro", label='Picos R')
plt.title("Detección de Picos R en el Tercer Minuto")
plt.xlabel("Tiempo (s)")
plt.ylabel("Voltaje (V)")
plt.grid(True)
plt.legend()
plt.show()
````

![image](https://github.com/user-attachments/assets/7b0f5534-cc9d-400e-8c1d-a99915c6ee1e)

Se detectaron 72 latidos en 60 segundos

Frecuencia cardíaca total estimada: 72.00 latidos por minuto

c. Nueva señal con información anterior
```python
rr_signal = np.zeros_like(tiempo_1min.values)
for i in range(1, len(peaks)):
    idx = peaks[i]
    rr_signal[idx] = rr_intervals[i - 1]  # R-R anterior
    fc_signal = np.zeros_like(tiempo_1min.values)
for i in range(1, len(peaks)):
    idx = peaks[i]
    fc_signal[idx] = heart_rates[i - 1]  # FC instantánea
    plt.figure(figsize=(12, 4))
plt.plot(tiempo_1min, fc_signal, label="FC Instantánea como señal", color="purple")
plt.xlabel("Tiempo (s)")
plt.ylabel("Frecuencia cardíaca (bpm)")
plt.title("Nueva señal con frecuencia cardíaca en posiciones R")
plt.grid()
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/4f471c16-618e-4d10-8b5d-834a6f5d21c0)

# 4.Análisis de la HRV en el dominio del tiempo:

-Media de intervalos R-R y desviación estandar
 ```python
 rr_values = rr_signal[rr_signal > 0]

mean_rr = np.mean(rr_values)
sdnn = np.std(rr_values)

print(f"Media de intervalos R-R: {mean_rr:.4f} s")
print(f"SDNN (desviación estándar): {sdnn:.4f} s")

plt.figure(figsize=(10, 4))
plt.plot(tiempo_1min, rr_signal, label="Señal de intervalos R-R")
plt.xlabel("Tiempo (s)")
plt.ylabel("RR (s)")
plt.title("Señal discreta de Intervalos R-R")
plt.legend()
plt.grid()
plt.show()
```
![image](https://github.com/user-attachments/assets/c0d9b45a-89e9-4593-9336-2c990ec7308d)

Media de intervalos R-R: 0.8923 s

SDNN (desviación estándar): 0.2491 s


# 5.Aplicación de la Transformada Wavelet:

```python
data = np.loadtxt('rr_intervals.csv', delimiter=',', skiprows=1)
rr_intervals = data[:, 1]  # Ajusta si los RR están en otra columna

fs = 4

# Generar vector de tiempo original a partir de los RR
t_original = np.cumsum(rr_intervals)
max_time = 300
t_original_cut = t_original[t_original <= max_time]
rr_intervals_cut = rr_intervals[:len(t_original_cut)]

# Generar un vector de tiempo uniforme
t_uniform = np.arange(0, max_time, 1/fs)

# Interpolar para señal uniforme
rr_interpolated = np.interp(t_uniform, t_original_cut, rr_intervals_cut)

# ====== 3. Aplicar CWT ======
wavelet = 'cmor1.5-1.0'  # Morlet compleja
scales = np.arange(1, 128)
coeffs, freqs = pywt.cwt(rr_interpolated, scales, wavelet, sampling_period=1/fs)
power = np.abs(coeffs)**2  # Potencia

# ====== 4. Graficar espectrograma ======
plt.figure(figsize=(12, 6))
plt.imshow(power, extent=[t_uniform[0], t_uniform[-1], freqs[-1], freqs[0]],
           aspect='auto', cmap='jet')
plt.colorbar(label='Potencia espectral')
plt.xlabel('Tiempo (s)')
plt.ylabel('Frecuencia (Hz)')
plt.title('Espectrograma CWT de la HRV (Primeros 300 segundos)')
plt.ylim([0.04, 0.4])  # LF y HF
plt.grid(True)
plt.show()
```
![image](https://github.com/user-attachments/assets/ed46e33e-21c1-4931-ab74-493b17cf96bd)

```python
data = np.loadtxt('rr_intervals.csv', delimiter=',', skiprows=1)
rr_intervals = data[:, 1]
fs = 4  # Frecuencia de muestreo deseada (Hz) para la señal interpolada

# Generar vector de tiempo original a partir de los RR
t_original = np.cumsum(rr_intervals)
max_time = 300
t_original_cut = t_original[t_original <= max_time]
rr_intervals_cut = rr_intervals[:len(t_original_cut)]

# Generar un vector de tiempo uniforme
t_uniform = np.arange(0, max_time, 1/fs)

# Interpolar para señal uniforme
rr_interpolated = np.interp(t_uniform, t_original_cut, rr_intervals_cut)

# ====== 3. Aplicar CWT ======
wavelet = 'cmor1.5-1.0'  # Morlet compleja
scales = np.arange(1, 128)
coeffs, freqs = pywt.cwt(rr_interpolated, scales, wavelet, sampling_period=1/fs)
power = np.abs(coeffs)**2  # Potencia

# Índices de las frecuencias en el rango de LF y HF
lf_band_indices = np.where((freqs >= 0.04) & (freqs <= 0.15))[0]
hf_band_indices = np.where((freqs >= 0.15) & (freqs <= 0.4))[0]

# ====== 5. Calcular la potencia total en las bandas LF y HF ======
lf_power = np.sum(power[lf_band_indices, :], axis=0)  # Sumar la potencia en LF
hf_power = np.sum(power[hf_band_indices, :], axis=0)  # Sumar la potencia en HF

# ====== 7. Graficar los cambios de potencia en LF y HF ======
plt.figure(figsize=(12, 6))

# Graficar potencia LF
plt.subplot(2, 1, 1)
plt.plot(t_uniform, lf_power, label='Potencia LF (0.04-0.15 Hz)', color='blue')
plt.xlabel('Tiempo (s)')
plt.ylabel('Potencia (u.a.)')
plt.title('Potencia en la Banda LF (0.04 - 0.15 Hz)')
plt.grid(True)

# Graficar potencia HF
plt.subplot(2, 1, 2)
plt.plot(t_uniform, hf_power, label='Potencia HF (0.15-0.4 Hz)', color='red')
plt.xlabel('Tiempo (s)')
plt.ylabel('Potencia (u.a.)')
plt.title('Potencia en la Banda HF (0.15 - 0.4 Hz)')
plt.grid(True)

plt.tight_layout()
plt.show()
````
![image](https://github.com/user-attachments/assets/2c9bbf08-542a-4286-a5a8-58714fdea13c)

# Análisis

En este análisis se aplicó un filtro pasa banda IIR de tipo Butterworth de cuarto orden, con frecuencias de corte de 0.5 Hz y 40 Hz, sobre una señal ECG muestreada a 1000 Hz. El objetivo fue eliminar componentes no deseadas, como el ruido de muy baja frecuencia (por movimientos o artefactos respiratorios) y el ruido de alta frecuencia (como interferencia eléctrica o actividad muscular). En la señal original se observa un nivel de voltaje elevado con muchas variaciones pequeñas y rápidas, indicativas de ruido. Tras el filtrado, la señal se centra alrededor de cero voltios, y se reduce considerablemente el ruido, destacando más claramente los complejos QRS. Esta mejora en la claridad de la señal permite una detección más precisa de los picos R, fundamentales para el análisis de la frecuencia cardíaca y la variabilidad (HRV). En resumen, el filtrado fue exitoso, limpiando la señal y conservando sus características fisiológicas esenciales, lo cual es crucial para garantizar un análisis clínico y matemático fiable.

En esta etapa del análisis se realizó la detección de los picos R de la señal ECG previamente filtrada, lo cual es esencial para calcular la frecuencia cardíaca y posteriormente analizar la variabilidad de la misma (HRV). Se utilizó la función find_peaks con dos parámetros clave: una distancia mínima entre picos (min_dist) de 0.3 segundos, que equivale al intervalo mínimo fisiológicamente esperable entre dos latidos (considerando una frecuencia cardíaca máxima de ~176 lpm), y una prominencia mínima de 0.3 V, con el fin de asegurar que los picos detectados correspondan a verdaderos complejos QRS y no a ruido o fluctuaciones menores. En el gráfico, los picos R se muestran resaltados en rojo sobre la señal ECG filtrada, evidenciando una detección clara y consistente a lo largo del minuto analizado. El resultado fue la identificación de un número de latidos que permitió estimar la frecuencia cardíaca total en latidos por minuto (bpm), reflejando la eficacia del preprocesamiento y del umbral seleccionado para capturar eventos fisiológicos significativos.

Al comparar los resultados obtenidos en los diferentes segmentos temporales de la señal ECG, se observa una clara diferencia en la frecuencia cardíaca asociada al estado fisiológico del sujeto. Durante el primer minuto, en condición de reposo, la frecuencia cardíaca estimada fue de 56 latidos por minuto, lo cual es coherente con un estado de relajación o reposo basal. En contraste, al analizar la señal correspondiente al minuto tres, cuando el sujeto se encontraba bajo una situación de estrés inducido por un videojuego de terror, se detectó un incremento significativo en el número de picos R, reflejado en una frecuencia cardíaca más alta (por ejemplo, entre 70 a 100 lpm, dependiendo del caso). Este aumento se debe a la activación del sistema nervioso simpático ante el estímulo estresante, lo que evidencia cómo la frecuencia cardíaca varía dinámicamente ante diferentes estados emocionales y de alerta. Esta diferencia entre ambos minutos demuestra de manera efectiva la sensibilidad del análisis ECG, y en particular de la detección de picos R, como herramienta para evaluar la respuesta fisiológica al estrés.
En el análisis de la variabilidad de la frecuencia cardíaca (HRV), los intervalos R-R representan el tiempo entre dos latidos consecutivos y son fundamentales para evaluar el estado del sistema nervioso autónomo. En este caso, se obtuvo una media de intervalos R-R de 0.8923 segundos, lo que indica que, en promedio, hay un latido cada aproximadamente 0.89 segundos, equivalente a una frecuencia cardíaca de unos 67 latidos por minuto.

Por otro lado, la SDNN (desviación estándar de los intervalos R-R) fue de 0.2491 segundos, lo que refleja una variabilidad considerable en los intervalos entre latidos. Una SDNN más alta suele estar asociada a una buena capacidad de adaptación del sistema cardiovascular frente a estímulos internos o externos, mientras que valores más bajos podrían indicar estrés, fatiga o alteraciones del sistema autónomo.

En conjunto, estos resultados muestran una variabilidad moderada, lo cual podría interpretarse como una respuesta fisiológica activa, posiblemente influida por la situación estresante (como se mencionó en el minuto 3 con el juego de terror). Esta variabilidad es esperada y normal en condiciones dinámicas, y refuerza el valor del análisis R-R como herramienta de evaluación del estado de activación o estrés del organismo.

La imagen del espectrograma CWT de la HRV de nuestra señal muestra un episodio de activación del sistema nervioso autónomo en respuesta al estrés (Juego de Terror), evidenciado por un incremento de la potencia espectral entre los 100 y 150 segundos en un amplio rango de frecuencias (aproximadamente de 0.05 Hz a 0.35 Hz), abarcando tanto la banda LF (relacionada con la regulación simpática y parasimpática) como la HF (vinculada a la actividad parasimpática). Esta franja de alta intensidad, nos muestra que hay una fuerte respuesta autonómica transitoria, posiblemente debido al estímulo estresante. Fuera de ese intervalo, antes de los 100 segundos y después de los 150 segundos, la baja potencia espectral indica una actividad cardíaca más estable, que es lógica ya que fueron periodos de reposo y menos estres.
# Preguntas

-Diferencias entre análisis en el dominio del tiempo y el tiempo-frecuencia: El análisis en el dominio del tiempo ofrece una visión general de los intervalos R-R, mientras que el análisis tiempo-frecuencia, a través de la transformada wavelet, proporciona detalles sobre cómo las frecuencias de la HRV cambian a lo largo del tiempo, capturando mejor las variaciones dinámicas de la señal.

-Efecto de las funciones wavelet: El tipo de wavelet seleccionada puede influir en la resolución del análisis. Las wavelets con mayor compresión temporal pueden ofrecer mejores resultados en frecuencias rápidas, mientras que otras pueden ser más adecuadas para fenómenos de baja frecuencia o cambios más suaves en la señal.

-Aplicaciones reales: Esta práctica tiene aplicaciones en la medicina preventiva, monitorización de la salud cardiovascular, y la evaluación de la respuesta al estrés, lo cual es útil en el contexto de enfermedades crónicas y la gestión de la salud en general.

# Conclusión

El uso de filtros IIR es fundamental para eliminar ruidos de alta frecuencia en la señal ECG, lo que permite una detección precisa de los picos R, esenciales para el cálculo de los intervalos R-R y el análisis de la variabilidad de la frecuencia cardíaca (HRV). La adquisición adecuada de la señal mediante un sistema DAQ garantiza una señal precisa y confiable para análisis posteriores. Al aplicar la transformada wavelet, se logra un análisis detallado en el dominio tiempo-frecuencia, permitiendo observar cómo varían las frecuencias de la HRV, lo que proporciona una visión más profunda de la actividad simpática y parasimpática del sistema nervioso autónomo.

# Referencias

Análisis de wavelets. (n.d.). StudySmarter ES. Retrieved April 26, 2025, from https://www.studysmarter.es/resumenes/matematicas/matematicas-aplicadas/analisis-de-wavelets/

Coon, E. (2023, July 3). Introducción al sistema nervioso autónomo. Manuale Merck versión para el público general; Manuales de Merck. https://www.merckmanuals.com/es-us/hogar/enfermedades-cerebrales-medulares-y-nerviosas/trastornos-del-sistema-nervioso-autónomo/introducción-al-sistema-nervioso-autónomo

Guzmán, M., & Navarro, P. B. (2024, December 10). Introducción al sistema nervioso periférico.

Mezoo Co., Ltd. (n.d.). Me-zoo.com. Retrieved April 26, 2025, from https://m.me-zoo.com/main/html.php?htmid=sp%2Fscience%2Fscience6.html

Quiroz-González, S., López-Espinosa, E., Liu, Z., & Fossion, R. (2024). Evidencias de los efectos parasimpáticos y simpáticos de la acupuntura mediante la variabilidad de la frecuencia cardíaca: implicaciones multisistémicas. Revista internacional de acupuntura, 18(1), 100288. https://doi.org/10.1016/j.acu.2024.100288

Serrano, D. C., & Torres, A. (2024, December 10). Introducción al sistema nervioso periférico.
