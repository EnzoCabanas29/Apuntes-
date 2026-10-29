# Resumen de Comunicaciones: Electricidad, Magnetismo y Ondas Electromagnéticas

## Índice

- [Clase 2](#clase-2)
- [Clase 3](#clase-3)
- [Clase 4](#clase-4)
- [Clase 5](#clase-5)
- [Clase 6](#clase-6)
- [Clase 7](#clase-7)
- [Clase 8](#clase-8)
- [Clase 9](#clase-9)
- [Clase 10](#clase-10)
---

<a id="clase-2"></a>
# Clase 2

## Índice de la Clase 2

- [1. Antecedentes históricos y conceptos base](#c2-1)
- [2. Electromagnetismo básico](#c2-2)
- [3. Espectro electromagnético](#c2-3)
- [4. Señales analógicas y digitales](#c2-4)
- [5. Amplificación y regeneración](#c2-5)
- [6. Amplitud, frecuencia y fase](#c2-6)
- [7. Onda cuadrada y tren de pulsos](#c2-7)
- [8. Transmisión de datos y valores de señal](#c2-8)

---

<a id="c2-1"></a>
## 1. Antecedentes históricos y conceptos base

### 1.1 Antecedentes históricos

- **Oersted (1820):** la corriente eléctrica genera un campo magnético.
- **Faraday (1831):** un campo magnético variable genera corriente eléctrica (inducción).
- **Maxwell (1860):** unificó estos fenómenos en la teoría de campos electromagnéticos.

<a id="11-antecedentes-historicos"></a>
### 1.2 Conceptos base

- La electricidad está asociada a cargas eléctricas con signos positivo y negativo.
- El magnetismo siempre es bipolar; no existen monopolos magnéticos.
- Los campos eléctricos y magnéticos son vectoriales.

<a id="13-ecuaciones-de-maxwell---forma-de-heaviside"></a>
### 1.3 Ecuaciones de Maxwell - forma de Heaviside

1. Gauss para el campo eléctrico:  
   $\nabla \cdot \mathbf{E} = \frac{\rho}{\varepsilon_0}$
2. Gauss para el campo magnético:  
   $\nabla \cdot \mathbf{B} = 0$
3. Ley de Faraday:  
   $\nabla \times \mathbf{E} = -\frac{\partial \mathbf{B}}{\partial t}$
4. Ley de Ampère-Maxwell:  
   $\nabla \times \mathbf{B} = \mu_0 \mathbf{J} + \mu_0 \varepsilon_0 \frac{\partial \mathbf{E}}{\partial t}$

> En forma oral: “Las dos ecuaciones de Gauss indican de dónde nacen los campos; Faraday dice que un campo magnético variable genera un campo eléctrico; y Ampère-Maxwell indica que una corriente o un campo eléctrico variable genera un campo magnético. Con esto se explica la radio.”

---

<a id="c2-2"></a>
## 2. Electromagnetismo básico

- **Relación fundamental:** cargas en movimiento generan campo magnético; un campo magnético variable genera campo eléctrico. El resultado es un campo electromagnético que se propaga en el vacío.
- **Ley de Ohm:** $V = I \cdot R$
- **Onda electromagnética:** $\mathbf{E} \perp \mathbf{B} \perp$ dirección de propagación.
- **Vector de Poynting:** $\mathbf{S} = \frac{1}{\mu_0} \mathbf{E} \times \mathbf{B}$
- **Parámetros principales:**  
  $c = 3 \cdot 10^8\,\text{m/s}$,  
  $f = \frac{1}{T}$,  
  $\lambda = \frac{c}{f} = c \cdot T$

---

<a id="c2-3"></a>
## 3. Espectro electromagnético

El espectro electromagnético se ordena de mayor frecuencia a menor frecuencia, y por ende de menor longitud de onda a mayor longitud de onda.

| Tipo de onda | Longitud de onda $\lambda$ | Frecuencia $f$ | Observación |
| :--- | :--- | :--- | :--- |
| Rayos gamma | $<10^{-12}$ m | $>10^{20}$ Hz | Ionizantes |
| Rayos X | $10^{-12}$ a $10^{-8}$ m | $10^{16}$ a $10^{20}$ Hz | Ionizantes |
| Ultravioleta (UV) | $10^{-8}$ a $10^{-7}$ m | $10^{15}$ a $10^{16}$ Hz | Ionizantes |
| Luz visible | $4\cdot10^{-7}$ a $7\cdot10^{-7}$ m | $4.3\cdot10^{14}$ a $7.5\cdot10^{14}$ Hz | No ionizante |
| Infrarrojo (IR) | $10^{-6}$ a $10^{-3}$ m | $10^{11}$ a $10^{14}$ Hz | No ionizante |
| Microondas | $10^{-3}$ a $10^{-1}$ m | $10^{9}$ a $10^{11}$ Hz | No ionizante |
| Radio | $10^{-1}$ a $10^{4}$ m | $10^{4}$ a $10^{9}$ Hz | No ionizante |

- **Relación clave:** $\lambda = \frac{c}{f}$
- **A medida que aumenta la frecuencia, disminuye la longitud de onda.**
- **Ionizantes:** UV, rayos X y rayos gamma. Tienen energía suficiente para arrancar electrones y alterar moléculas, incluso el ADN.
- **No ionizantes:** luz visible, IR, microondas y radio. No tienen suficiente energía para ionizar.

---

<a id="c2-4"></a>
## 4. Señales analógicas y digitales

### 4.1 Señal analógica

Una señal analógica varía en el tiempo de forma continua. Puede tomar infinitos valores dentro de un rango.

Ejemplo: una onda senoidal que representa la voz humana.

### 4.2 Señal digital

Una señal digital solo puede tomar un número finito de valores preestablecidos, normalmente 0 y 1.

Ejemplo: audio comprimido, datos de un archivo o señales lógica de un circuito digital.

### 4.3 Origen de las señales analógicas sobre redes digitales

Para llevar una señal analógica a una red digital se usa un **CODEC** (codificador-decodificador).

- **Ejemplo:** llamada telefónica
  - Teléfono analógico → CODEC → red digital → CODEC → teléfono analógico

### 4.4 Módem

Un **módem** modula y demodula la señal para que pueda viajar por un medio analógico.

- Se usa para transportar datos digitales sobre una portadora analógica.
- Ejemplo: internet por línea telefónica antigua.

### 4.5 Fenómenos que afectan la transmisión

| Fenómeno | ¿Qué es? | Ejemplo |
| :--- | :--- | :--- |
| Atenuación | Pérdida de potencia a medida que la señal recorre el medio | Un cable largo entrega menos nivel de señal |
| Distorsión | Las frecuencias no llegan iguales; la señal se deforma | Voz metálica o señal alterada |
| Ruido | Señales no deseadas que se superponen | Interferencia, ruido térmico |
| Retardo | Tiempo que tarda la señal en llegar | Retraso en una llamada o enlace satelital |
| Capacidad insuficiente | El canal no soporta la cantidad de información que se quiere enviar | Vídeo HD sobre un canal demasiado lento |
| Ancho de banda insuficiente | El canal no tiene rango de frecuencias suficiente | La señal se comprime o se pierde detalle |

> El ancho de banda es el rango de frecuencias que puede transmitir un canal. Cuanto mayor es el ancho de banda, mayor suele ser la capacidad de transmisión.

---

<a id="c2-5"></a>
## 5. Amplificación y regeneración

- **Amplificador:** $V_{salida} = G \cdot V_{entrada}$  
  Amplifica la señal, pero también amplifica el ruido. Se usa en redes analógicas.
- **Repetidor regenerativo:**
  - Umbral: $V_1 = 1$, $V_0 = 0$
  - Regenera el pulso limpio y elimina ruido.
  - Se usa principalmente en redes digitales y fibra óptica.
- **Señal sinusoidal:**  
  $v(t) = A \cdot \sin(2\pi f t + \phi)$  
  Ejemplo: $v(t) = 311\sin(2\pi 50 t)$

---

<a id="c2-6"></a>
## 6. Amplitud, frecuencia y fase

La forma general de una señal sinusoidal es:

$$
v(t) = A \sin(2\pi f t + \phi)
$$

Donde:

- **A:** amplitud, representa la intensidad o nivel de la señal en voltios.
- **f:** frecuencia, indica qué tan rápido varía la señal en Hz.
- **$\phi$:** fase, indica desde dónde comienza la señal, en radianes o grados.

| Parámetro | Analogía con una ola | Unidad |
| :--- | :--- | :--- |
| Amplitud | Altura de la onda | V |
| Frecuencia | Cada cuánto se repite la onda | Hz |
| Fase | Punto de inicio respecto al eje | rad |

---

<a id="c2-7"></a>
## 7. Onda cuadrada y tren de pulsos

- **Onda cuadrada:**  
  $v(t) = +A$ si $0 < t < T/2$, y $v(t) = -A$ si $T/2 < t < T$  
  Tiene un duty cycle del 50% y se usa como reloj digital.
- **Tren de pulsos:**  
  $\tau$ = ancho del pulso, $T$ = periodo, $D = \frac{\tau}{T} \cdot 100$  
  En general $\tau \ll T$, con un duty cycle típico del 1% al 10%. Se usa en radar.
- **Ancho de banda aproximado:**  
  $BW \approx \frac{1}{\tau}$

> Toda onda cuadrada es un tren de pulsos con duty cycle del 50%, pero no todo tren de pulsos es una onda cuadrada.

---

<a id="c2-8"></a>
## 8. Transmisión de datos y valores de señal

### 8.1 Comunicación serie vs paralela

| Característica | Comunicación serie | Comunicación paralela |
| :--- | :--- | :--- |
| Bits transmitidos | 1 por vez | N por vez |
| Cables necesarios | Pocos | Muchos |
| Costo | Bajo | Alto |
| Distancia | Larga | Corta |
| Complejidad | Mayor en electrónica | Más simple, pero difícil sincronizar |
| Ejemplos | USB, HDMI, Ethernet, Bluetooth, 4G/5G | IDE, LPT, buses antiguos |

**Resumen:** hoy casi toda la transmisión se hace en serie porque es más barata, más confiable y mejor para largas distancias.

### 8.2 Valor eficaz RMS

Es el valor equivalente en continua de una señal alterna: es la tensión que produciría el mismo efecto de potencia o calor que una corriente continua.

$$
V_{RMS} = \frac{V_{pico}}{\sqrt{2}} \approx 0.707 \cdot V_{pico}
$$

Ejemplo: los 220 V de la red eléctrica son RMS, por lo que el valor de pico real es:

$$
V_{pico} = 220 \cdot \sqrt{2} = 311\,V
$$

### 8.3 Valor medio $Y_m$

El valor medio es el promedio de la señal en un periodo completo. Para una senoidal pura, el valor medio total es cero porque la parte positiva y la negativa se cancelan.

Por eso se suele hablar del valor medio rectificado:

$$
Y_m = \frac{2 \cdot V_{pico}}{\pi} \approx 0.637 \cdot V_{pico}
$$

### 8.4 Factor de forma $FF$

El factor de forma mide qué tan distinta es una señal respecto a una onda continua; indica la forma de la onda y su "redondez" o "cuadratura".

$$
FF = \frac{V_{RMS}}{Y_m}
$$

Valores típicos:

- **Senoidal:** $FF = \frac{0.707}{0.637} \approx 1.11$
- **Cuadrada:** $FF = 1$
- **Triangular:** $FF \approx 1.15$

### 8.5 Resumen de fórmulas

$$
\begin{aligned}
V_{RMS} &= \frac{V_{pico}}{\sqrt{2}} \\
Y_m &= \frac{2 \cdot V_{pico}}{\pi} \\
FF &= \frac{V_{RMS}}{Y_m}
\end{aligned}
$$

---

<a id="clase-3"></a>
# Clase 3: Series de Fourier y señales periódicas

## Índice de la Clase 3

- [1. ¿Por qué importa en telecom?](#c3-1)
- [2. Condiciones de Dirichlet](#c3-2)
- [3. Forma trigonométrica de Fourier](#c3-3)
- [4. Onda cuadrada impar](#c3-4)
- [5. Forma compleja de Fourier](#c3-5)
- [6. Tiempo vs frecuencia](#c3-6)
- [7. Ejercicio resuelto](#c3-7)
- [8. Velocidad de modulación y transmisión](#c3-8)
- [9. BER y rendimiento](#c3-9)
- [10. Cierre con GeoGebra](#c3-10)

---

<a id="c3-1"></a>
## 1. ¿Por qué importa en telecom?
La Serie de Fourier es fundamental porque permite estudiar una señal compleja como combinación de senoidales simples. En telecomunicaciones esto sirve para:

- transmisión eficiente
- filtrado de ruido e interferencias
- análisis del ancho de banda
- estudio de modulación y demodulación
- mejora tecnológica y diagnóstico de señales

Idea clave: la dualidad tiempo-frecuencia.
- En el dominio del tiempo se observa la forma de la señal.
- En el dominio de la frecuencia se observan las senoides que la componen.

---

<a id="c3-2"></a>
## 2. Condiciones de Dirichlet
Una función $f(t)$ puede desarrollarse en serie de Fourier si cumple:

1. $f(t)$ es periódica, con período $T$
2. está definida salvo en un número finito de puntos
3. tiene un número finito de máximos y mínimos en un período
4. $f(t)$ y $f'(t)$ son continuas por partes

Estas condiciones aseguran que la serie converja en casi todos los puntos.

---

<a id="c3-3"></a>
## 3. Forma trigonométrica de Fourier
La forma general es:

$$
f(t)=a_0+
\sum_{n=1}^{\infty}\left[a_n\cos(n\omega_0 t)+b_n\sin(n\omega_0 t)\right]
$$

donde:

$$
\omega_0=\frac{2\pi}{T}=2\pi f_0
$$

y los coeficientes son:

$$
a_0=\frac{1}{T}\int_{-T/2}^{T/2} f(t)\,dt
$$

$$
a_n=\frac{2}{T}\int_{-T/2}^{T/2} f(t)\cos(n\omega_0 t)\,dt
$$

$$
b_n=\frac{2}{T}\int_{-T/2}^{T/2} f(t)\sin(n\omega_0 t)\,dt
$$

### Paridad útil
- Si $f(t)$ es par:
  $$
  \int_{-a}^{a} f(t)\,dt = 2\int_0^a f(t)\,dt
  $$
- Si $f(t)$ es impar:
  $$
  \int_{-a}^{a} f(t)\,dt = 0
  $$

Esto simplifica mucho los cálculos.

---

<a id="c3-4"></a>
## 4. Ejemplo: onda cuadrada impar
Una onda cuadrada impar cumple:

$$
f(t)=-f(-t)
$$

Entonces:

$$
a_0=0, \qquad a_n=0
$$

y solo aparecen términos en seno:

$$
f(t)=\sum_{n\text{ impar}} \frac{4}{n\pi}\sin(n\omega_0 t)
$$

Desarrollando:

$$
f(t)\approx \frac{4}{\pi}\sin(\omega_0 t)+\frac{4}{3\pi}\sin(3\omega_0 t)+\frac{4}{5\pi}\sin(5\omega_0 t)+\cdots
$$

Esto muestra que una onda cuadrada está formada por infinitas armónicas impares.

### Fenómeno de Gibbs
En las discontinuidades aparece un sobrepico aproximado del 9%, aunque agreguemos más armónicas. Esto se conoce como fenómeno de Gibbs.

---

<a id="c3-5"></a>
## 5. Forma compleja de Fourier
Usando la identidad de Euler,

$$
e^{jt} = \cos t + j\sin t
$$

la señal puede escribirse como

$$
f(t) = \sum_{n=-\infty}^{+\infty} C_n e^{j n \omega_0 t}
$$

donde

$$
C_n = \frac{1}{T}\int_{-T/2}^{T/2} f(t)e^{-j n \omega_0 t}\,dt
$$

Esta forma es muy útil porque expresa la amplitud y la fase de cada componente armónica.

### Tren rectangular
Para un pulso rectangular de amplitud $A$, ancho $\tau$ y período $T$,

$$
|C_n| = A\frac{\tau}{T}
\left|\frac{\sin\left(n\omega_0\tau/2\right)}{n\omega_0\tau/2}\right|
$$

o equivalentemente,

$$
|C_n| = A\frac{\tau}{T}\left|\operatorname{sinc}\left(\frac{n\omega_0\tau}{2}\right)\right|
$$

con

$$
\operatorname{sinc}(x)=\frac{\sin x}{x}
$$

### Fórmulas útiles
- Número de armónicas relevantes:

  $$
  N = \frac{T}{\tau}
  $$

- Amplitud máxima del espectro:

  $$
  |C_0| = A\frac{\tau}{T}
  $$

Si $\tau$ es pequeño, el espectro es ancho; si $\tau$ es grande, el espectro es más estrecho.

---

<a id="c3-6"></a>
## 6. Tiempo vs frecuencia
- En el tiempo: vemos pulsos, forma de onda, amplitud versus $t$
- En la frecuencia: vemos rayas o componentes armónicas separadas por $f_0$
- El espectro de un tren de pulsos tiene una envolvente sinc

La separación entre líneas del espectro es:

$$
\Delta f = f_0 = \frac{1}{T}
$$

Esto es clave en telecomunicaciones porque determina el ancho de banda y la capacidad de transmisión.

---

<a id="c3-7"></a>
## 7. Ejercicio resuelto (pág. 22)
Datos:
- $FRP=1000\ \text{pps}$
- $T=\frac{1}{1000}=0.001\ \text{s}$
- $V_m=2000\ \text{baudios}$
- $\tau=\frac{1}{V_m}=0.5\times10^{-4}\ \text{s}$
- $A=1\ \text{V}$

### 1) Período
$$
T=0.001\ \text{s}
$$

### 2) Duración del pulso
$$
\tau=0.5\times10^{-4}\ \text{s}
$$

### 3) Número de armónicas
$$
N=\frac{T}{\tau}=\frac{0.001}{0.5\times10^{-4}}=20
$$

### 4) Frecuencia fundamental
$$
f_0=\frac{1}{T}=\frac{1}{0.001}=1000\ \text{Hz}
$$

### 5) Ancho de banda
$$
BW\approx N\cdot f_0 = 20\cdot1000 = 20000\ \text{Hz}=20\ \text{kHz}
$$

### 6) Amplitud máxima
$$
|C_0|=A\frac{\tau}{T}=1\cdot\frac{0.5\times10^{-4}}{0.001}=0.05\ \text{V}
$$

Conclusión: el espectro es sinc y el primer cero aparece en la armónica 20.

---

<a id="c3-8"></a>
## 8. Velocidad de modulación y transmisión
La velocidad de símbolos es:

$$
V_m=\frac{\text{número de cambios}}{\text{tiempo}}\quad [\text{baudios}]
$$

La velocidad de transmisión en bits es:

$$
V_t=\frac{1}{\tau}\log_2(n)\quad [\text{bps}]
$$

donde $n$ es el número de niveles.

### Importante
- más niveles $\Rightarrow$ más bits por cambio
- mayor eficiencia espectral
- pero también mayor complejidad y sensibilidad al ruido

---

<a id="c3-9"></a>
## 9. BER y rendimiento
### BER
$$
BER=\frac{\text{bits con errores}}{\text{bits transmitidos}}
$$

Valores típicos:
- muy bueno: $10^{-9}$ a $10^{-10}$
- bueno: $10^{-6}$
- degradado: $10^{-3}$ a $10^{-5}$
- dañado: $>10^{-3}$

### Rendimiento
$$
\text{Rendimiento}=\frac{\text{bits útiles}}{\text{bits totales}}
$$

---

<a id="c3-10"></a>
## 10. Cierre con GeoGebra
Una señal sinusoidal general es:

$$
f(t)=A\sin(\omega t+\phi)
$$

donde:
- $A$ = amplitud
- $\omega$ = frecuencia angular
- $\phi$ = fase

En Fourier:
- $A$ representa la amplitud del armónico $|C_n|$
- $\omega=n\omega_0$
- $\phi$ representa la fase del coeficiente complejo

### Interpretación visual
- aumentar $A$ → estiramiento vertical
- aumentar $\omega$ → más ciclos por unidad de tiempo
- aumentar $\phi$ → desplazamiento horizontal (adelanto o retraso)

---

## Resumen final
- La serie de Fourier descompone una señal periódica en armónicas.
- La frecuencia fundamental es

  $$
  f_0 = \frac{1}{T}
  $$

- La forma trigonométrica es

  $$
  f(t) = a_0 + \sum_{n=1}^{\infty}\left[a_n\cos(n\omega_0 t)+b_n\sin(n\omega_0 t)\right]
  $$

- La forma compleja es

  $$
  f(t) = \sum_{n=-\infty}^{+\infty} C_n e^{j n \omega_0 t}
  $$

- Un tren rectangular tiene un espectro con envolvente sinc.
- El ancho de banda depende del ancho del pulso $\tau$ y del período $T$.
- Este análisis es fundamental para la transmisión, el filtrado y el diagnóstico en telecomunicaciones.

---

<a id="clase-4"></a>
# Clase 4: Espectro de pulsos, enlaces y espectro electromagnético

## Índice de la Clase 4

- [1. Espectro de pulsos](#c4-1)
- [2. Cálculo de enlaces y decibelios](#c4-2)
- [3. Unidades con referencia fija](#c4-3)
- [4. Balance de potencia](#c4-4)
- [5. Ejercicio resuelto](#c4-5)
- [6. Espectro electromagnético](#c4-6)

---

<a id="c4-1"></a>
## 1. Espectro de pulsos

### 1.1 Parámetros básicos

El ancho del pulso es la inversa de la velocidad de modulación:

$$
\mathit{tau} = V_m^{-1} = \frac{1}{V_m}\quad [s]
$$

El período de repetición es la inversa de la frecuencia de repetición de pulsos:

$$
T = FRP^{-1} = \frac{1}{FRP}\quad [s]
$$

### 1.2 Ancho de banda y armónicas

El ancho de banda aproximado depende del ancho del pulso:

$$
AB = \tau^{-1} = \frac{1}{\tau} = V_m\quad [Hz]
$$

Cuanto más angosto es el pulso, mayor ancho de banda se necesita.

La cantidad aproximada de armónicas dentro del lóbulo principal es:

$$
N_{\text{armónicas}} = \frac{T}{\tau}
$$

Para una amplitud de pulso $A$, la amplitud de cada línea espectral se aproxima mediante:

$$
C_n = A\frac{\tau}{T}
$$

En el caso particular de $A=1\,V$:

$$
C_n = \frac{\tau}{T}\quad [V]
$$

### 1.3 Relación clave

Cuando $A=1$:

$$
C_n\,N_{\text{armónicas}}
= \left(\frac{\tau}{T}\right)\left(\frac{T}{\tau}\right)=1
$$

---

<a id="c4-2"></a>
## 2. Cálculo de enlaces y decibelios

### 2.1 Atenuación y ganancia

La relación lineal entre la potencia de salida y la de entrada es:

$$
R = \frac{P_s}{P_e}
$$

- **Atenuación:** $P_s<P_e$, por lo tanto $0<R<1$.
- **Ganancia:** $P_s>P_e$, por lo tanto $R>1$.

Un atenuador reduce la potencia. Algunos ejemplos son una resistencia, un cable largo o el espacio libre.

### 2.2 Elementos en cascada

Las ganancias y pérdidas lineales se multiplican:

$$
G_{\text{tot}} = \prod_{i=1}^{n}G_i
$$

Por ejemplo:

$$
G_{\text{tot}}=G_1\,G_2\,G_3
$$

Si hay pérdidas y ganancias mezcladas, se aplica la misma regla.

### 2.3 Decibelios

Para potencia, la relación se expresa como:

$$
G_{\text{dB}}=10\log_{10}\left(\frac{P_s}{P_e}\right)
$$

- Si $P_s>P_e$, el resultado es positivo y representa una ganancia.
- Si $P_s<P_e$, el resultado es negativo y representa una pérdida.

En lineal las relaciones se multiplican; en decibelios se suman:

$$
G_{\text{tot,dB}}=\sum_{i=1}^{n}G_{i,\text{dB}}
$$

La conversión inversa es:

$$
P_s=P_e\,10^{G_{\text{dB}}/10}
$$

---

<a id="c4-3"></a>
## 3. Unidades con referencia fija

Estas unidades comparan una potencia o tensión con un valor de referencia fijo.

### 3.1 dBm

La referencia es $1\,mW$:

$$
P_{\text{dBm}}=10\log_{10}\left(\frac{P[mW]}{1\,mW}\right)
$$

$$
0\,\text{dBm}=1\,mW
$$

### 3.2 dBW

La referencia es $1\,W$:

$$
P_{\text{dBW}}=10\log_{10}\left(\frac{P[W]}{1\,W}\right)
$$

$$
0\,\text{dBW}=1\,W=30\,\text{dBm}
$$

### 3.3 dBu

La referencia de tensión es $0.775\,V_{\text{RMS}}$:

$$
V_{\text{dBu}}=20\log_{10}\left(\frac{V[V]}{0.775\,V}\right)
$$

Ese valor genera $1\,mW$ sobre una resistencia de $600\,\Omega$:

$$
0\,\text{dBu}=0.775\,V_{\text{RMS}}=0\,\text{dBm}=1\,mW
$$

### 3.4 dBmV

La referencia es $1\,mV$ y se utiliza principalmente en televisión y cable coaxial:

$$
V_{\text{dBmV}}=20\log_{10}\left(\frac{V[mV]}{1\,mV}\right)
$$

### 3.5 Regla de oro

- Para **potencia**: $10\log_{10}$.
- Para **tensión**: $20\log_{10}$.

La razón es que $P=V^2/R$:

$$
10\log_{10}\left(\frac{P_s}{P_e}\right)
=10\log_{10}\left[\left(\frac{V_s}{V_e}\right)^2\right]
=20\log_{10}\left(\frac{V_s}{V_e}\right)
$$

### 3.6 Conversión rápida

| Relación lineal | Ganancia o pérdida |
| :---: | :---: |
| $\times 0.001$ | $-30\,\text{dB}$ |
| $\times 0.01$ | $-20\,\text{dB}$ |
| $\times 0.1$ | $-10\,\text{dB}$ |
| $\times 0.5$ | $-3\,\text{dB}$ |
| $\times 1$ | $0\,\text{dB}$ |
| $\times 2$ | $+3\,\text{dB}$ |
| $\times 4$ | $+6\,\text{dB}$ |
| $\times 10$ | $+10\,\text{dB}$ |
| $\times 100$ | $+20\,\text{dB}$ |
| $\times 1000$ | $+30\,\text{dB}$ |

---

<a id="c4-4"></a>
## 4. Balance de potencia

### 4.1 Enlace por cable o fibra

Esquema:

$$
Tx\longrightarrow\text{cable}\longrightarrow Amp
\longrightarrow\text{cable}\longrightarrow Rx
$$

La potencia recibida se calcula en dB como la suma de ganancias menos la suma de pérdidas:

$$
P_{Rx}=P_{Tx}+Amp-
\left(At_{\text{cable}}+At_{\text{empalmes}}+At_{\text{conectores}}+FD\right)
$$

La condición para que el enlace funcione es:

$$
P_{Rx}\geq S_{Rx}
$$

Donde:

$$
\begin{aligned}
At_{\text{cable}}&=\alpha L \\
At_{\text{empalmes}}&=N_{\text{empalmes}}At_{\text{empalme}} \\
At_{\text{conectores}}&=N_{\text{conectores}}At_{\text{conector}}
\end{aligned}
$$

- $P_{Tx}$: potencia transmitida, en dBm.
- $Amp$: ganancia del amplificador, en dB.
- $FD$: factor de diseño o margen de seguridad, normalmente entre $3$ y $6\,dB$.
- $S_{Rx}$: sensibilidad del receptor, en dBm.

Si $P_{Rx}<S_{Rx}$, el enlace no funciona. Las alternativas son aumentar la ganancia, reducir la distancia o agregar un repetidor.

### 4.2 Enlace satelital

Esquema:

$$
\mathrm{Tierra}\xrightarrow{\text{Up-Link}}\text{Satélite}
\xrightarrow{\text{Down-Link}}\text{Tierra}
$$

La ecuación incorpora las ganancias de las antenas y la ganancia del satélite:

$$
P_{Rx}=P_{Tx}+Amp_{\text{sat}}+G_{\text{antenas}}
-\left(At_{\text{atmósfera}}+At_{\text{cables}}+At_{\text{empalmes}}
+At_{\text{conectores}}+FD\right)
$$

La ganancia total de las antenas es:

$$
G_{\text{antenas}}=G_{Tx}+G_{Rx}
$$

Y la condición de enlace sigue siendo:

$$
P_{Rx}\geq S_{Rx}
$$

La atenuación atmosférica incluye el espacio libre, la lluvia y el aire. El satélite actúa como repetidor, mientras que las antenas parabólicas concentran energía y aportan ganancia.

> **Regla general:** todo lo que ayuda menos todo lo que frena debe superar la sensibilidad del receptor.

---

<a id="c4-5"></a>
## 5. Ejercicio resuelto: balance de potencia

### 5.1 Enunciado

Un enlace de $1800\,m$ utiliza un coaxial con una atenuación de $0.5\,dB/100\,m$ y transmite $P_{Tx}=2\,W$. ¿Qué sensibilidad máxima, expresada en mW, puede admitir el receptor?

Datos:

$$
L=1800\,m,\qquad \alpha=0.5\,\frac{dB}{100\,m},\qquad P_{Tx}=2\,W
$$

Se consideran nulas las pérdidas de empalmes, conectores y el factor de diseño, y no hay amplificador.

### 5.2 Resolución

**1. Atenuación del cable**

$$
At_{\text{cable}}=1800\,m\left(\frac{0.5\,dB}{100\,m}\right)=9\,dB
$$

**2. Conversión de la potencia transmitida**

$$
P_{Tx}=2\,W=2000\,mW
$$

$$
P_{Tx}=10\log_{10}(2000)=33.01\,dBm
$$

**3. Potencia que llega al receptor**

$$
P_{Rx}=33.01-9=24.01\,dBm
$$

**4. Conversión a mW**

$$
P_{Rx}=10^{24.01/10}=251.7\,mW
$$

Por lo tanto, la sensibilidad debe cumplir:

$$
S_{Rx}\leq251.7\,mW
$$

Por ejemplo, un receptor con sensibilidad de $200\,mW$ funciona; uno de $500\,mW$ no alcanza el nivel recibido.

### 5.3 Atajo sin dBm

Una pérdida de $9\,dB$ equivale a una relación lineal de:

$$
10^{-9/10}=0.1259
$$

Entonces:

$$
P_{Rx}=2\,W\times0.1259=0.2517\,W=251.7\,mW
$$

---

<a id="c4-6"></a>
## 6. Espectro electromagnético

### 6.1 Longitud de onda

La longitud de onda es la distancia que avanza una onda durante un período, o la distancia entre dos puntos equivalentes consecutivos.

$$
\lambda=vT=\frac{v}{f}
$$

En el vacío, $v=c$:

$$
c=3\times10^8\,m/s,\qquad \lambda=\frac{c}{f}
$$

Para calcular rápidamente con $f$ en MHz:

$$
\lambda[m]\approx\frac{300}{f[MHz]}
$$

Ejemplos:

$$
\begin{aligned}
100\,MHz&\Rightarrow\lambda=3\,m \\
300\,MHz&\Rightarrow\lambda=1\,m \\
900\,MHz&\Rightarrow\lambda\approx0.33\,m=33\,cm \\
2.4\,GHz&=2400\,MHz\Rightarrow\lambda=12.5\,cm
\end{aligned}
$$

Regla clave:

$$
f\uparrow\Rightarrow\lambda\downarrow\Rightarrow\text{antena más pequeña}
$$

### 6.2 Bandas de frecuencia

| Banda | Abreviatura | Frecuencia | Longitud de onda aproximada |
| :--- | :---: | :--- | :--- |
| Por debajo de ELF | -- | $<3\,Hz$ | $>100000\,km$ |
| Extra baja frecuencia | ELF | $3$--$30\,Hz$ | $100000$--$10000\,km$ |
| Super baja frecuencia | SLF | $30$--$300\,Hz$ | $10000$--$1000\,km$ |
| Ultra baja frecuencia | ULF | $300$--$3000\,Hz$ | $1000$--$100\,km$ |
| Muy baja frecuencia | VLF | $3$--$30\,kHz$ | $100$--$10\,km$ |
| Baja frecuencia | LF | $30$--$300\,kHz$ | $10$--$1\,km$ |
| Media frecuencia | MF | $300$--$3000\,kHz$ | $1\,km$--$100\,m$ |
| Alta frecuencia | HF | $3$--$30\,MHz$ | $100$--$10\,m$ |
| Muy alta frecuencia | VHF | $30$--$300\,MHz$ | $10$--$1\,m$ |
| Ultra alta frecuencia | UHF | $300$--$3000\,MHz$ | $1\,m$--$100\,mm$ |
| Super alta frecuencia | SHF | $3$--$30\,GHz$ | $100$--$10\,mm$ |
| Extra alta frecuencia | EHF | $30$--$300\,GHz$ | $10$--$1\,mm$ |
| Por encima de EHF | -- | $>300\,GHz$ | $<1\,mm$ |

### 6.3 Aplicaciones para recordar

| Banda | Aplicaciones frecuentes |
| :--- | :--- |
| VLF | Comunicaciones con submarinos |
| LF/MF | Radio AM |
| HF | Onda corta y radioaficionados |
| VHF | Radio FM, televisión aérea y aeronáutica |
| UHF | Televisión digital y celulares 4G |
| SHF/EHF | Microondas, WiFi de 5 GHz, satélite y radar |

Como referencia adicional:

| Aplicación o banda de uso | Frecuencia o longitud de onda aproximada |
| :--- | :--- |
| Comunicaciones submarinas | $<30\,kHz$, longitudes de onda mayores a $10\,km$ |
| Radio AM | Alrededor de MF, longitudes de onda menores a $650\,m$ |
| Radio de onda corta | HF, longitudes de onda menores a $180\,m$ |
| Radio FM | VHF, longitudes de onda menores a $10\,m$ |
| Radar y televisión | UHF, longitudes de onda menores a $1\,m$ |
| Microondas | Frecuencias mayores a $1\,GHz$ |
| Luz visible | Aproximadamente $384$--$750\,THz$ |
| Ultravioleta | Frecuencias mayores a aproximadamente $1.5\,PHz$ |
| Rayos X | Frecuencias mayores a aproximadamente $30\,PHz$ |
| Rayos gamma | Frecuencias mayores a aproximadamente $30\,EHz$ |

$$
2.4\,GHz\Rightarrow\lambda=12.5\,cm,\qquad
5\,GHz\Rightarrow\lambda=6\,cm
$$

> **Nota para el parcial:** el apunte del profesor ubica celular, microondas y satélite dentro de “infrarrojo cercano”. Técnicamente, las comunicaciones celulares se encuentran principalmente en UHF/SHF, aproximadamente entre $300\,MHz$ y $30\,GHz$.

---


<a id="clase-5"></a>
# Clase 5

## Índice de la Clase 5

- [1. Banda base y códigos de línea](#c5-1)
- [2. Criterios que debe cumplir un código de línea](#c5-2)
- [3. Clasificación de los códigos de línea](#c5-3)
- [4. Códigos más importantes](#c5-4)
- [5. HDB3 y B8ZS](#c5-5)
- [6. Teoría de la información y Shannon](#c5-6)

---

<a id="c5-1"></a>
## 1. Banda base y códigos de línea

### 1.1 ¿Qué es banda base?

Se llama banda base a la señal digital original, tal como sale del codificador o del equipo emisor, sin ser llevada a una frecuencia portadora ni sometida a un proceso de modulación.

- No se “monta” sobre una onda portadora.
- Se transmite directamente por el medio físico o por la línea de enlace.
- Es la señal que se genera en el nivel digital antes de cualquier adaptación de canal.

En otras palabras, si una computadora o un sistema digital genera un flujo binario, la banda base es ese flujo antes de ser modulado para radio, fibra u otros medios.

### 1.2 ¿Qué es un código de línea?

Un código de línea es la forma en que se representan los bits 0 y 1 mediante niveles de tensión o corriente en una línea física.

Su objetivo es adaptar la secuencia binaria al canal para que pueda viajar de forma segura y reutilizable. Un código de línea no solo “escribe” bits, sino que también condiciona:

- la presencia o ausencia de componente continua,
- la capacidad de sincronizar el reloj,
- la detección de fallas de línea,
- el ancho de banda que requiere la señal.

---

<a id="c5-2"></a>
## 2. Criterios que debe cumplir un código de línea

Un código de línea ideal debe cumplir, como mínimo, tres condiciones fundamentales:

### 2.1 Eliminar la componente continua (DC)

La componente continua no puede pasar por algunos elementos del sistema, como transformadores o acoplos capacitivos.

Además, una DC no lleva información útil; es energía desperdiciada. Por eso, un buen código evita que la señal quede en 0V o en un nivel constante durante mucho tiempo.

### 2.2 Permitir detección de presencia de línea

El receptor debe saber si la línea sigue viva aunque el flujo de datos sea largo o esté formado por muchos ceros.

Si la línea se queda en 0V durante mucho tiempo, el receptor puede confundirlo con:

- un cable cortado,
- una pérdida de señal,
- o un largo bloque de ceros que no tiene transición.

### 2.3 Permitir sincronismo

El receptor debe poder recuperar el reloj $T_b$ a partir de las transiciones de la señal. Si no hay cambios suficientes, no puede saber dónde termina un bit y empieza el siguiente.

Por eso, los códigos de línea suelen buscar que haya muchas transiciones con una frecuencia útil para sincronizar el reloj.

> Regla práctica: un código es mejor cuando, además de representar bits, deja “marcas” temporales en la señal.

---

<a id="c5-3"></a>
## 3. Clasificación de los códigos de línea

### 3.1 Según la polaridad

- **Unipolar:** usa dos niveles, por ejemplo $0V$ y $+V$
  - Ejemplo: $0 
ightarrow 0V$, $1 
ightarrow +V$
  - Tiene mucha componente DC.

- **Polar:** usa dos niveles opuestos, por ejemplo $+V$ y $-V$
  - Ejemplo: $0 
ightarrow -V$, $1 
ightarrow +V$
  - Balancea mejor la DC si hay igual cantidad de 1 y 0.

- **Bipolar:** usa tres niveles, por ejemplo $+V$, $0V$, $-V$
  - Ejemplo: AMI
  - Tiene mejor comportamiento respecto a la DC y a la detección de errores.

### 3.2 Según el ancho de pulso

- **NRZ (Non Return to Zero):** el pulso ocupa todo el intervalo del bit $T_b$
  - Ventaja: poco ancho de banda
  - Desventaja: si llega una racha larga de igual bit, hay pocas transiciones y se pierde el sincronismo

- **RZ (Return to Zero):** el pulso vuelve a cero antes de terminar el bit
  - Ventaja: más transiciones, mejor sincronismo
  - Desventaja: requiere más ancho de banda

- **Bifase:** hay transición obligatoria dentro del bit
  - Mejora el sincronismo
  - Generalmente exige más ancho de banda

---

<a id="c5-4"></a>
## 4. Códigos más importantes

### 4.1 Unipolar NRZ

- $1 = +V$
- $0 = 0V$
- Pulso de duración $T_b$

Ventajas:
- Simplemente implementable.

Desventajas:
- Tiene gran componente continua.
- No permite sincronismo fiable con muchas repeticiones del mismo bit.
- No detecta bien la presencia de línea.

### 4.2 Polar NRZ

- $1 = +V$
- $0 = -V$
- El pulso dura todo el bit.

Ventajas:
- Mejor que el unipolar.
- Si hay igual cantidad de 1 y 0, la componente DC se compensa.

Desventajas:
- En una racha larga de 1 o 0 no hay transición, por lo que el sincronismo se degrada.

### 4.3 Bipolar AMI (Alternate Mark Inversion)

Regla:

- $0 = 0V$
- $1 = +V$ o $-V$ alternando, según la secuencia

Ejemplo:

$$ 1\ 1\ 1\ 1 \rightarrow +V, -V, +V, -V$$

Ventajas:
- Elimina la DC en promedio.
- Es simple y muy usado.

Desventajas:
- Si aparecen muchos ceros seguidos, la línea queda a 0V durante un tiempo largo.
- Se pierde sincronismo.
- No se detecta presencia de línea correctamente.

Por eso aparecen técnicas de sustitución como HDB3 y B8ZS.

### 4.4 Manchester

Este es uno de los códigos más importantes y se usa en Ethernet.

Regla:

- En cada bit hay una transición obligatoria en el centro del intervalo.
- Si el bit es 1, la transición es de nivel alto a bajo.
- Si el bit es 0, la transición es de bajo a alto.

Formalmente:

- $1$: transición de $+V$ a $-V$ a mitad de $T_b$
- $0$: transición de $-V$ a $+V$ a mitad de $T_b$

Ventajas:
- No tiene DC.
- Garantiza sincronismo en cada bit.
- Detecta presencia de línea.

Desventajas:
- Requiere el doble de ancho de banda que NRZ.

$$ BW \approx \frac{2}{T_b} $$

### 4.5 Manchester diferencial

Es una variante de Manchester en la que la información no depende de la polaridad absoluta, sino de la presencia o ausencia de transición al inicio del bit.

Regla general:

- $1$: solo hay transición al centro del bit.
- $0$: hay transición al inicio y al centro del bit.

Ventajas:
- Tiene las mismas ventajas de Manchester.
- Es más robusto frente a variaciones de polaridad y ruido.

### 4.6 Miller (Delay Modulation)

Es un código con buen equilibrio entre ancho de banda y sincronismo.

Regla:

- $1$: hay transición a mitad del intervalo $T_b$
- $0$: no hay transición, salvo que el siguiente bit también sea 0; en ese caso hay transición al inicio del intervalo

Ventajas:
- No tiene DC.
- Tiene sincronismo razonable.
- Detecta presencia de línea.
- Tiene mejor eficiencia espectral que Manchester.

Desventajas:
- No es tan simple de interpretar como Manchester.

### 4.7 Resumen comparativo

| Código | DC | Sincronismo | Detección de línea | Ancho de banda |
| :--- | :---: | :---: | :---: | :--- |
| Unipolar NRZ | No | No | No | Bajo |
| Polar NRZ | Casi nula si está balanceado | No | Sí | Bajo |
| AMI | Sí, se elimina | No con muchos ceros | No con muchos ceros | Bajo |
| Manchester | Sí | Sí | Sí | Alto |
| Miller | Sí | Sí | Sí | Medio-bajo |

> Regla de memoria: si te preguntan “qué código cumple todo pero consume poco ancho de banda”, la respuesta es Miller. Si te preguntan “qué código cumple todo sin importar el ancho de banda”, la respuesta es Manchester.

---

<a id="c5-5"></a>
## 5. HDB3 y B8ZS

### 5.1 ¿Por qué nacen?

AMI es bueno porque elimina la DC, pero falla cuando aparecen muchas secuencias de ceros consecutivos. Entonces la línea queda en $0V$ durante un tiempo prolongado.

Esto provoca:

- pérdida de sincronismo,
- imposibilidad de detectar si el cable sigue conectado,
- y en general una mala recuperación del reloj.

Para evitarlo se usan códigos de sustitución como:

- **HDB3:** High Density Bipolar 3 Zeros
- **B8ZS:** Bipolar with 8-Zero Substitution

### 5.2 HDB3

HDB3 reemplaza bloques de cuatro ceros consecutivos por una secuencia especial que mantiene la alternancia de polaridad y evita la continua.

#### Regla general

Cada vez que hay `0000`, se reemplaza según la cantidad de unos desde la última violación.

- Si hay un número impar de unos desde la última violación, se reemplaza por `000V`
- Si hay un número par de unos desde la última violación, se reemplaza por `B00V`

Donde:

- $V$ = violación de la regla AMI
- $B$ = bit de relleno, con polaridad opuesta al último 1

#### Objetivo

Que las violaciones $V$ alternen siempre su polaridad, por ejemplo:

$$ +, -, +, - 	ext{ ...}$$

Esto mantiene la componente continua en cero.

#### Ejemplo conceptual

Si se tiene la secuencia:

$$ 1\ 0000\ 1\ 0000$$

y el último 1 transmitido era negativo, entonces se puede interpretar la línea como una alternancia en la que las violaciones se producen con polaridades alternadas y no se acumula DC.

#### Receptor

Cuando el receptor detecta una violación, sabe que no está frente a un dato normal sino a una secuencia especial de reemplazo.

- `000V` se interpreta como un bloque de cuatro ceros.
- `B00V` también se interpreta como cuatro ceros, eliminando el relleno.

### 5.3 B8ZS

B8ZS se usa principalmente en sistemas T1/DS1.

Su idea es similar a HDB3, pero reemplaza bloques de ocho ceros por una secuencia con violaciones para evitar que la línea quede en reposo.

Regla principal:

- si aparecen 8 ceros seguidos, se insertan violaciones para evitar una línea “muerta”
- la secuencia se construye de forma que la polaridad de las violaciones alterna.

Se usa por la misma razón que HDB3: preservar la sincronización y evitar DC.

### 5.4 Comparación rápida

| Código | Problema que corrige | Idea principal |
| :--- | :--- | :--- |
| AMI | muchos 0 seguidos | alterna + y - |
| HDB3 | AMI con rachas largas de ceros | reemplaza 0000 por secuencia especial |
| B8ZS | 8 ceros seguidos | reemplaza bloques largos por violaciones |

---

<a id="c5-6"></a>
## 6. Teoría de la información y Shannon

### 6.1 ¿Qué es la información según Shannon?

La información no depende de “lo importante” que sea el mensaje, sino de su probabilidad. Cuanto menos probable es un suceso, más información transmite.

La cantidad de información asociada a un símbolo $S$ es:

$$ I(S) = \log_2\left(\frac{1}{P(S)}\right) = -\log_2 P(S) $$

Si la probabilidad es alta, la información es baja. Si la probabilidad es muy baja, la información es alta.

Ejemplos:

- “Mañana va a salir el sol” tiene poca información.
- “Habrá un eclipse total” tiene mucha información.

Unidad:

- bit si se usa logaritmo en base 2,
- hartley si se usa base 10,
- nat si se usa base $e$.

### 6.2 Cambio de base de logaritmos

Como en calculadora normalmente hay logaritmos en base 10 o naturales, se usa:

$$ \log_2(x) = \frac{\log_{10}(x)}{\log_{10}(2)} = \frac{\ln(x)}{\ln(2)} $$

Ejemplo clave:

$$ \log_2(8) = 3 $$

porque $2^3 = 8$.

### 6.3 Probabilidad

La probabilidad se calcula como:

$$ P = \frac{\text{casos favorables}}{\text{casos posibles}} $$

#### Ejemplos clásicos

1. Moneda cara:
   - $P(cara) = 1/2 = 0.5$
   - $I = \log_2(2) = 1$ bit

2. Dado sale un 6:
   - $P(6) = 1/6$
   - $I = \log_2(6) \approx 2.58$ bits

3. Dos dados suman 7:
   - $P = 6/36 = 1/6$
   - $I \approx 2.58$ bits

4. Dos dados suman 2:
   - $P = 1/36$
   - $I = \log_2(36) \approx 5.17$ bits

### 6.4 Entropía

La entropía de una fuente es la información promedio que aporta cada símbolo.

$$ H = -\sum_i P_i \log_2(P_i) $$

Donde:

- $H$ = entropía,
- $P_i$ = probabilidad del símbolo $i$,
- la unidad es bits/símbolo.

#### Ejemplo: moneda justa

Si $P(cara)=P(seca)=0.5$:

$$ H = -[0.5\log_2(0.5)+0.5\log_2(0.5)] = 1\ \text{bit/símbolo} $$

Esto es la máxima entropía para dos símbolos equiprobables.

#### Ejemplo: moneda cargada

Si $P(cara)=0.9$ y $P(seca)=0.1$:

$$ H = -[0.9\log_2(0.9)+0.1\log_2(0.1)] \approx 0.469\ \text{bits/símbolo} $$

La entropía baja porque ya casi sabés qué va a salir.

### 6.5 Tasa de información

La tasa de información relaciona la entropía con la velocidad de aparición de los símbolos.

$$ R = \frac{H}{\tau} = H \cdot V_m $$

Donde:

- $H$ = entropía [bits/símbolo]
- $\tau$ = duración media del símbolo [s/símbolo]
- $V_m = 1/\tau$ = velocidad de modulación [símbolos/s]
- $R$ = tasa de información [bits/s]

### 6.6 Teorema de Shannon para la capacidad del canal

La capacidad máxima de un canal es:

$$ C = B \cdot \log_2(1 + S/N) $$

Donde:

- $C$ = capacidad del canal [bits/s]
- $B$ = ancho de banda [Hz]
- $S/N$ = relación señal a ruido (en lineal, no en dB)

#### Regla clave

- Si $R < C$, el sistema puede diseñarse para operar sin errores.
- Si $R > C$, el canal no alcanza para esa tasa de información; habrá errores.

### 6.7 Ejercicio clásico de telégrafo

Supongamos un telégrafo con dos símbolos:

- punto: $P_1 = 0.4$, $t_1 = 0.1s$
- raya: $P_2 = 0.6$, $t_2 = 0.3s$

#### Entropía

$$ H = -0.4\log_2(0.4)-0.6\log_2(0.6) \approx 0.97\ \text{bits/símbolo} $$

#### Duración media

$$ \tau = 0.4(0.1)+0.6(0.3)=0.22s $$

#### Velocidad de modulación

$$ V_m = \frac{1}{0.22} \approx 4.54\ \text{baudios} $$

#### Tasa de información

$$ R = \frac{H}{\tau} = \frac{0.97}{0.22} \approx 4.41\ \text{bits/s} $$

Comparando con la capacidad del canal:

- si $C = 10$ bits/s, entonces $R < C$ y hay margen;
- si $C = 3$ bits/s, entonces $R > C$ y el canal no alcanza.

### 6.8 Resumen final de Shannon

- $H$ mide cuánta información aporta un símbolo en promedio.
- $R$ mide cuánta información se transmite por segundo.
- $C$ mide cuánto puede soportar el canal.
- La condición fundamental es:

$$ R < C $$

Si $R$ supera a $C$, el sistema va a tener errores inevitables.

---

<a id="clase-6"></a>
# Clase 6

## Índice de la Clase 6

- [1. Ancho de banda](#c6-1)
- [2. Filtros y su clasificación](#c6-2)
- [3. Filtros pasivos y activos](#c6-3)
- [4. Teorema de Nyquist](#c6-4)
- [5. Capacidad del canal sin ruido](#c6-5)
- [6. Teorema de Shannon-Hartley](#c6-6)
- [7. Ejemplo de capacidad en un canal telefónico](#c6-7)

<a id="c6-1"></a>
## 1. Ancho de banda

- El **ancho de banda** es el rango de frecuencias que un canal o dispositivo deja pasar con una atenuación aceptable.
- Se mide sobre la curva de respuesta en frecuencia, en los puntos donde la ganancia cae **−3 dB** respecto del máximo.
- $f_1$ y $f_2$ son las frecuencias de corte inferior y superior, y $f_c$ es la frecuencia central:

$$\Delta f = f_2 - f_1$$

- El espectro acústico de la **voz** y de la **música** ocupa rangos distintos. El **canal telefónico** se limita aproximadamente a **300 Hz – 3,3 kHz**, mientras que la música (radio AM, FM, CD-audio) necesita un ancho de banda mayor.

<a id="c6-2"></a>
## 2. Filtros y su clasificación

Los filtros son dispositivos que dejan pasar ciertas frecuencias y rechazan otras. Se clasifican en:

- **Pasa bajos**: pasan las frecuencias por debajo de $f_c$.
- **Pasa altos**: pasan las frecuencias por encima de $f_c$.
- **Pasa banda**: pasan las frecuencias entre $F_{ci}$ y $F_{cs}$.
- **Elimina banda**: rechazan las frecuencias entre $F_{ci}$ y $F_{cs}$.

Conceptos asociados:

- **Banda de paso**: frecuencias que atraviesan el filtro.
- **Banda de rechazo**: frecuencias que se atenúan.
- **Frecuencia de corte** ($f_c$): punto donde la ganancia cae −3 dB.
- Los filtros pueden ser **ideales** (transición abrupta) o **reales** (transición gradual).
- **Factor Q**: mide la **selectividad** del filtro.

<a id="c6-3"></a>
## 3. Filtros pasivos y activos

**Pasivos**: están formados por componentes que no entregan energía.

- Resistencias
- Bobinas
- Capacitores
- Cristal (se modela con un circuito equivalente con $L$, $C_1$, $C_2$ y $C_3$)

Configuraciones típicas con impedancias en serie ($Z_s$) y en paralelo ($Z_p$): filtro en **T** y filtro en **π**. La señal pasante sigue hacia la salida y la señal no deseada se deriva a tierra.

**Activos**: incorporan un **amplificador operacional** con una **red de realimentación**, además de las impedancias $Z_s$ y $Z_p$.

<a id="c6-4"></a>
## 4. Teorema de Nyquist

- Se trata de un canal **sin ruido**.
- Surge del trabajo de H. Nyquist, *Certain Topics in Telegraph Transmission Theory*. Shannon lo retoma en *Communication in the Presence of Noise*.
- Considerando el ancho de banda, la frecuencia de Nyquist debe cumplir:

$$f_N > 2\, f_{max}$$

$$f_N > 2\, \Delta f$$

<a id="c6-5"></a>
## 5. Capacidad del canal sin ruido

Para una señal **binaria** en un canal ideal sin ruido:

$$C = V_{max} = 2\,B \quad [\text{bps}]$$

Para una señal **multinivel** con $n$ niveles:

$$C = V_{max} = 2\,B \log_2 n \quad [\text{bps}]$$

Donde $B$ es el ancho de banda y $n$ la cantidad de niveles de señal.

<a id="c6-6"></a>
## 6. Teorema de Shannon-Hartley

El **ruido aditivo** se suma a la señal en el canal de comunicaciones. En una señal multinivel (por ejemplo, tribits con 8 niveles entre 0 V y 7 V) el ruido puede hacer que el receptor confunda un nivel con otro y se produzcan **errores**.

**Relación señal/ruido:**

$$\frac{S}{N} = \frac{\text{potencia de la señal}}{\text{potencia de ruido}}$$

Shannon demostró que la **máxima cantidad de niveles** depende del ruido:

$$n_{max} = \sqrt{1 + \frac{S}{N}}$$

Reemplazando en la capacidad multinivel del canal ideal:

$$C = 2B \log_2 \sqrt{1 + \frac{S}{N}}$$

Queda la **capacidad del canal** (Shannon-Hartley):

$$C = B \log_2\left(1 + \frac{S}{N}\right) \quad [\text{bps}]$$

<a id="c6-7"></a>
## 7. Ejemplo de capacidad en un canal telefónico

**Enunciado:** en un canal telefónico la relación $S/N$ típica es de 30 dB, con $F_{ci} = 300\ \text{Hz}$ y $F_{cs} = 3300\ \text{Hz}$. ¿Cuál es el límite superior de la tasa de transmisión de datos confiable?

**Ancho de banda:**

$$B = F_{cs} - F_{ci} = 3300 - 300 = 3000\ \text{Hz} = 3\ \text{kHz}$$

**Relación señal/ruido en veces:**

$$\text{dB} = 10 \log \frac{S}{N} \;\Rightarrow\; \frac{S}{N} = 10^{30/10} = 1000$$

**Capacidad:**

$$C = B \log_2\left(1 + \frac{S}{N}\right) = 3000 \cdot \log_2(1 + 1000) \approx 29\,901\ \text{bps}$$

---

<a id="clase-7"></a>
# Clase 7

## Índice de la Clase 7

- [1. Errores en la transmisión de datos](#c7-1)
- [2. Ruido y distorsión](#c7-2)
- [3. Tipos de ruido](#c7-3)
- [4. Efectos del ruido blanco sobre las señales](#c7-4)
- [5. Tipos de errores](#c7-5)
- [6. Métodos de detección y corrección de errores](#c7-6)
- [7. Control de paridad](#c7-7)
- [8. Suma de verificación](#c7-8)
- [9. Control por Redundancia Cíclica CRC](#c7-9)
- [10. Ejemplo de CRC](#c7-10)
- [11. Corrección de errores](#c7-11)
- [12. Distancia de Hamming](#c7-12)
- [13. Código de Hamming](#c7-13)

<a id="c7-1"></a>
## 1. Errores en la transmisión de datos

Causas de errores:

- **Ruido**: se suma a la señal.
- **Atenuación**.
- **Distorsión**.
- **Tasa de información mayor a la capacidad del canal** ($T > C$).
- **Ancho de banda insuficiente**.

<a id="c7-2"></a>
## 2. Ruido y distorsión

- El ruido es una tensión aleatoria que se superpone a la señal útil. Tiene un **valor medio** ($\bar{X}$) alrededor del cual fluctúa.
- Según su origen, el ruido puede ser **endógeno** o **exógeno** (ver sección siguiente).

<a id="c7-3"></a>
## 3. Tipos de ruido

**Endógeno** (generado dentro del propio sistema):

- Térmico
- De disparo
- De tránsito

**Exógeno** (generado fuera del sistema):

- Generado por sistemas creados por el hombre
- Generado por sistemas naturales

<a id="c7-4"></a>
## 4. Efectos del ruido blanco sobre las señales

- El ruido se suma tanto a señales **analógicas** como **digitales**, y la señal resultante queda deformada.
- En una señal digital, el **ruido impulsivo** puede llevar la señal por encima o por debajo del **umbral de detección** y producir **errores de bit**.
- Ejemplo: en la secuencia transmitida `0 1 0 1 0 1`, el ruido impulsivo provoca errores en el 1.° y en el 4.° bit.

<a id="c7-5"></a>
## 5. Tipos de errores

- Errores **aislados o simples**.
- Errores **en ráfagas**.
- Errores **agrupados**.

Según su efecto, un mensaje con errores puede seguir siendo **inteligible para el usuario**, o bien los errores pueden **cambiar el contenido** del mensaje (por ejemplo, un byte que pasa a representar otro número).

<a id="c7-6"></a>
## 6. Métodos de detección y corrección de errores

**Detección**

- **Control de paridad**: vertical (VRC), longitudinal (LRC), bidimensional o de doble paridad, cíclica o entrelazada.
- **Código polinomial** (CRC).

**Corrección**

- **Códigos autocorrectivos**: Hamming, Hagelbarger, Bose-Chaudhuri.
- **Técnicas especiales de transmisión**: corrección de errores hacia adelante (**FEC**) y requerimiento automático de repetición (**ARQ**).

<a id="c7-7"></a>
## 7. Control de paridad

Se agrega un **bit de paridad** al dato transmitido:

- **Paridad par**: el bit se elige para que la cantidad total de unos sea **par**.
- **Paridad impar**: el bit se elige para que la cantidad total de unos sea **impar**.

**Vertical (VRC, *Vertical Redundancy Check*)**

- Se agrega un bit de paridad a cada carácter: 7 bits de datos + 1 bit de paridad.
- Ejemplo: dato `0110101` (cuatro unos). Para paridad par se agrega un `0`. Para paridad impar se agrega un `1`.

**Longitudinal o bidimensional (LRC, *Longitudinal Redundancy Check*)**

- Además de la paridad vertical de cada carácter, se calcula un **byte de paridad longitudinal** (BCC) sobre el bloque de datos, bit a bit.
- Al recibir, el error aparece como una fila y una columna con paridad incorrecta, y su **intersección** indica el bit errado.

**Entrelazada o cíclica**

- El bit de paridad se genera a partir de los bits de información del carácter transmitido, tomándolos de forma entrelazada (ejemplo de la clase: carácter `0 1 0 1 0 1`).

<a id="c7-8"></a>
## 8. Suma de verificación

**Checksum** con suma en complemento a 1 (el acarreo final se suma al resultado). Ejemplo con cuatro palabras de 4 bits:

| Palabra | Valor |
|---|---|
| A | `1010` |
| B | `1011` |
| C | `1100` |
| D | `1101` |

| Paso | Operación | Resultado (con acarreo sumado) |
|---|---|---|
| A + B | `1010 + 1011 = 10101` | `0110` |
| (A + B) + C | `0110 + 1100 = 10010` | `0011` |
| (A + B + C) + D | `0011 + 1101 = 10000` | `0001` |

**Complemento a 1** de `0001` → `1110`, que es la suma de verificación **a transmitir**.

<a id="c7-9"></a>
## 9. Control por Redundancia Cíclica CRC

Se llama también **polinómico** porque un mensaje como `11011011` se asimila a un polinomio:

$$1\cdot x^7 + 1\cdot x^6 + 0\cdot x^5 + 1\cdot x^4 + 1\cdot x^3 + 0\cdot x^2 + 1\cdot x^1 + 1$$

**Procedimiento:**

1. Definir el polinomio $M(x)$ de grado $n$, que es el mensaje a transmitir.
2. Definir el polinomio generador $G(x)$ de grado $r$. Debe cumplirse $n \gg r$.
3. Generar el polinomio de $(n + r)$ bits: $x^r M(x)$.
4. Dividir $x^r M(x)$ por $G(x)$ usando **álgebra de módulo 2**.
5. De la división se obtiene el resto $R(x)$, que tiene $r$ bits o menos.
6. Obtener el polinomio a transmitir $T(x)$, restando (módulo 2) el resto $R(x)$ a $x^r M(x)$.

**Pasos matemáticos:**

$$\frac{x^r M(x)}{G(x)} = C(x) + \frac{R(x)}{G(x)}$$

donde $C(x)$ es el cociente, que no tiene utilidad.

$$T(x) = x^r M(x) + R(x)$$

- $T(x)$ es **siempre divisible** por $G(x)$.
- Si se introducen errores en la transmisión, se recibe:

$$T'(x) = T(x) + E(x)$$

El receptor divide lo recibido por $G(x)$: si el resto es **cero**, no se detectan errores.

<a id="c7-10"></a>
## 10. Ejemplo de CRC

Datos: $M(x) = 11010011101100$ y $G(x) = x^3 + x + 1 = 1011$ (por lo tanto $r = 3$).

**Generación en el transmisor**

- Se agregan $r = 3$ ceros: `11010011101100 000`.
- Se divide módulo 2 (la resta es una **XOR**) por `1011`.
- El resto es `100`.
- Se transmite `11010011101100 100`.

**Comprobación en el receptor**

- Se divide `11010011101100 100` por `1011`.
- El resto es `000`, entonces no hay error.

Tabla de verdad de la XOR usada en cada paso:

| $A$ | $B$ | $A \oplus B$ |
|:-:|:-:|:-:|
| 1 | 1 | 0 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 0 | 0 | 0 |

<a id="c7-11"></a>
## 11. Corrección de errores

**Estrategias:**

- **Corrección hacia atrás** (ARQ): cuando el receptor detecta el error, **solicita al transmisor la repetición**.
- **Corrección hacia adelante** (FEC, *Forward Error Control*): usa **códigos autocorrectores** en el receptor, que corrigen sin pedir retransmisión.

Ejemplo de operación FEC con dos series de mensajes ($D_x$ y $R_x$):

| Serie $D_x$ | Serie $R_x$ | Operación |
|---|---|---|
| Sin error | Sin error | Se imprime el carácter |
| Con error | Sin error | Se imprime el carácter de la serie $R_x$ |
| Sin error | Con error | Se imprime el carácter de la serie $D_x$ |
| Con error | Con error | Se imprime un carácter especial que indica error en la recepción |

<a id="c7-12"></a>
## 12. Distancia de Hamming

Richard Hamming postuló este concepto en los laboratorios Bell (1950).

- **Distancia de Hamming** ($d$): número de bits en que difieren dos secuencias binarias $S_1$ y $S_2$ de la misma longitud.
- Conociendo $d$ se sabe cuántos bits se pueden **detectar** o **corregir**:

$$\text{Detectar} = d - 1$$

$$\text{Corregir} = \frac{d - 1}{2}$$

| Distancia de Hamming | Detección | Corrección |
|:-:|:-:|:-:|
| 1 | no | no |
| 2 | uno | no |
| 3 | dos | uno |
| 4 | tres | uno |

<a id="c7-13"></a>
## 13. Código de Hamming

Los bits de **paridad** ocupan las posiciones que son potencias de 2 (1, 2, 4, 8) y los bits de **datos** ocupan el resto.

| Posición | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Bit | P1 | P2 | D1 | P3 | D2 | D3 | D4 | P4 | D5 | D6 | D7 |

Cada bit de paridad controla las posiciones cuyo número binario tiene en 1 el bit correspondiente (por ejemplo, P1 controla 1, 3, 5, 7, 9, 11). Los ejemplos de la clase usan **paridad par**.

**Ejemplo Hamming(11,7)** (el (7,4) es análogo, con 4 bits de datos)

- Dato a transmitir: `1000101` (D1 a D7).
- Se calculan: P1 = 1, P2 = 0, P3 = 0, P4 = 0.
- Dato transmitido: `10100000101`.

**Detección y corrección del error**

- Dato a recibir: `10100000101`.
- Dato recibido: `10100001101` (error en el bit 8).
- Paridad recibida (P4-P3-P2-P1) = `1001`.
- Paridad calculada (P4-P3-P2-P1) = `0001`.
- La XOR de ambas da `1000`, que en decimal es **8**: esa es la **posición del error**. Se invierte ese bit y el dato queda corregido.

---

<a id="clase-8"></a>
# Clase 8

## Índice de la Clase 8

- [1. Clasificación de los medios alámbricos](#c8-1)
- [2. Cables de cobre y modelo eléctrico](#c8-2)
- [3. Líneas de cobre desnudos](#c8-3)
- [4. Pares trenzados y multipares](#c8-4)
- [5. Cables UTP y cableado estructurado](#c8-5)
- [6. Ventajas y desventajas del UTP](#c8-6)
- [7. Cables coaxiles](#c8-7)
- [8. Guías de onda](#c8-8)
- [9. Ley de Snell](#c8-9)
- [10. Tipos de fibra óptica](#c8-10)
- [11. Ventanas de transmisión](#c8-11)
- [12. Pérdidas por dispersión y acoplamiento](#c8-12)
- [13. Categorías, colores y conectores](#c8-13)
- [14. Ventajas y desventajas de la fibra óptica](#c8-14)
- [15. LED y láser](#c8-15)
- [16. Mediciones en fibra óptica](#c8-16)
- [17. Cables multifibra](#c8-17)
- [18. Cables submarinos](#c8-18)

<a id="c8-1"></a>
## 1. Clasificación de los medios alámbricos

**Cables de cobre**

- Líneas de cobre desnudos
- Cables de par trenzado
- Cables multipar
- Cables de pares trenzados blindados y sin blindar
- Cables coaxiales

**Guías de onda**

**Fibras ópticas**

- Láser – LED
- Multimodo – Monomodo

<a id="c8-2"></a>
## 2. Cables de cobre y modelo eléctrico

Una línea de cobre se modela con parámetros distribuidos: **R** (resistencia), **L** (inductancia), **G** (conductancia) y **C** (capacitancia).

Impedancia característica:

$$Z = \sqrt{\frac{R + j L \omega}{G + j C \omega}}$$

Con:

$$\omega = 2\pi f \qquad L = \frac{\Phi\, n}{I} \qquad C = \frac{Q}{V}$$

<a id="c8-3"></a>
## 3. Líneas de cobre desnudos

Conductores tendidos sobre postes con aisladores, usados históricamente en telefonía y telegrafía. Los materiales y diámetros usuales son:

| Material | Diámetros de conductor |
|---|---|
| Cobre | 3, 4 y 5 mm |
| Bronce | 1,5, 2 y 3 mm |
| Hierro galvanizado | 2, 3, 4 y 5 mm |

Cada par conduce corrientes en sentido contrario, por lo que los campos electromagnéticos generados se oponen.

<a id="c8-4"></a>
## 4. Pares trenzados y multipares

- En el **par trenzado**, las corrientes circulan en sentido contrario y crean campos electromagnéticos opuestos que **se anulan entre sí**, lo que reduce la interferencia.
- El **cable multipar** agrupa $N$ conductores aislados y consta de:
  - Conductores aislados
  - Dieléctrico
  - Blindaje de aluminio
  - Cubierta protectora de polietileno
  - Cable de hierro galvanizado de sostén (en cables aéreos)
- Los conductores se identifican por **código de colores**: blanco, azul, anaranjado, verde, marrón, gris y rojo.

<a id="c8-5"></a>
## 5. Cables UTP y cableado estructurado

- **UTP** (*Unshielded Twisted Pair*): sin apantallar.
- **STP** (*Shielded Twisted Pair*): apantallado, con cubierta protectora.
- Cuatro pares trenzados, ocho cables en total.
- Conector **RJ-45** (macho y hembra). Orden de cable derecho: blanco naranja, naranja, blanco verde, azul, blanco azul, verde, blanco marrón, marrón.

**Parámetros por categoría / clase**

| Parámetro | 5e / D | 6 / E | 6A / E<sub>A</sub> | 7 / F | 7A / F<sub>A</sub> |
|---|:-:|:-:|:-:|:-:|:-:|
| Frecuencia [MHz] | 1 - 100 | 1 - 250 | 1 - 500 | 1 - 600 | 1 - 1000 |
| Atenuación [dB] | 24 | 21,3 / 21,7 | 20,9 | 20,8 | 20,3 |
| Pérdida NEXT [dB] | 30,1 | 39,9 | 39,9 | 62,9 | 65 |
| Pérdida ACRF [dB] | 17,4 | 23,3 | 23,3 / 25,5 | 44,4 | 47,4 |
| Pérdida de retorno [dB] | 10 | 12 | 12 | 12 | 12 |
| Delay de propagación [ns] | 548 | 548 | 548 | 548 | 548 |

<a id="c8-6"></a>
## 6. Ventajas y desventajas del UTP

**Ventajas del UTP**

- Económico
- Flexible
- Fácil de utilizar

**Desventajas**

- Interferencias por ruido
- Distancia limitada (100 m)

**Mitigación con STP**

- Reduce interferencias
- Misma distancia máxima
- Más caro que el UTP

<a id="c8-7"></a>
## 7. Cables coaxiles

**Estructura** (de afuera hacia adentro): vaina exterior, conductor externo o malla, dieléctrico o aislador, conductor interno o central.

**Fórmulas**

Capacidad por metro:

$$C = \frac{24{,}16\,\varepsilon}{\log \frac{D}{d}} \quad \left[\frac{\text{pF}}{\text{m}}\right]$$

Impedancia característica:

$$Z = \frac{138\ \Omega}{\sqrt{K}} \log \frac{D}{d}$$

Relación de ondas estacionarias (ROE), con $P_r$ potencia reflejada y $P_i$ potencia incidente:

$$ROE = \frac{1 + \sqrt{P_r / P_i}}{1 - \sqrt{P_r / P_i}}$$

Donde $D$ es el diámetro interno del conductor externo, $d$ el diámetro del conductor interno y $K$ la constante dieléctrica.

**Características por tipo.** Todos tienen impedancia $Z_0 = 50\ \Omega$, capacidad $C = 101\ \text{pF/m}$ y velocidad de propagación $V_0 = 66\ \%$.

| Coaxial | Tensión máx. [kV] | 10 MHz | 50 MHz | 100 MHz | 200 MHz | 400 MHz | 1000 MHz |
|---|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| RG174 A/U | 1,5 | 12,80 | 23,0 | 29,2 | 39,4 | 61,0 | 98,4 |
| RG122/U | 1,9 | 5,90 | 14,2 | 23,0 | 36,1 | 56,0 | 95,2 |
| RG58 C/U | 1,9 | 4,90 | 12,0 | 17,0 | 26,0 | 38,0 | 65,0 |
| RG223/U | 1,9 | 4,30 | 10,0 | 14,0 | 20,0 | 29,0 | 45,0 |
| RG223/U (otra variante) | 1,9 | 3,90 | 9,5 | 15,8 | 23,0 | 33,0 | 54,2 |
| RG213/U | 5,0 | 2,00 | 4,9 | 7,0 | 10,5 | 15,5 | 26,0 |
| RG9 B/U | 5,0 | 2,20 | 5,4 | 7,6 | 11,5 | 17,5 | 30,0 |
| RG214/U | 5,0 | 2,20 | 5,4 | 7,6 | 10,9 | 17,0 | 28,9 |
| RG218/U | 11,0 | 0,75 | 1,8 | 3,0 | 4,6 | 7,0 | 12,0 |
| RG177/U | 11,0 | 0,78 | 1,8 | 3,1 | 4,6 | 7,9 | 14,5 |

Las columnas de frecuencia indican la **atenuación a 20 °C en dB/100 m**.

**Ventajas**

- Mejor resistencia al ruido que el UTP
- Mayor ancho de banda que el UTP
- Durable
- Flexible

**Desventajas**

- Difícil instalación
- Voluminoso
- Costos

<a id="c8-8"></a>
## 8. Guías de onda

- Son conductos metálicos (generalmente rectangulares, con **aire** en el interior) que guían ondas de muy alta frecuencia, típicamente microondas.
- Impedancia de la guía, donde $f_c$ es la frecuencia de corte y $f$ la frecuencia de trabajo:

$$Z_0 = \frac{120\pi}{\sqrt{1 - \left(\dfrac{f_c}{f}\right)^2}}$$

- Existen componentes asociados: codos, uniones rotativas, acopladores direccionales, transiciones, unidades de presurización, entre otros.

<a id="c8-9"></a>
## 9. Ley de Snell

Describe la refracción de la luz al pasar de un medio a otro:

$$n_1 \sin\theta_1 = n_2 \sin\theta_2$$

Índice de refracción, con $C$ la velocidad de la luz en el vacío y $v$ la velocidad en el medio:

$$\eta = \frac{C}{v}$$

- $\theta_1$: ángulo de incidencia; $\theta_2$: ángulo de refracción.
- Cuando el ángulo de refracción llega a 90°, el ángulo de incidencia es el **ángulo crítico**. A partir de ahí hay **reflexión total**, que es el principio de la fibra óptica.

$$\theta_{critico} = \arcsin\frac{\eta_2}{\eta_1}$$

Ángulo máximo de entrada a la fibra (**cono de aceptación**), con $\eta_1$ el índice del núcleo y $\eta_2$ el del recubrimiento:

$$\phi = \arcsin\sqrt{\eta_1^2 - \eta_2^2}$$

Los rayos que entran dentro del cono de aceptación se propagan por el núcleo. Los que entran fuera de él no se propagan.

<a id="c8-10"></a>
## 10. Tipos de fibra óptica

| Tipo | Núcleo / revestimiento | Característica |
|---|---|---|
| **Multimodo de salto de índice** | núcleo ~200 µm | El pulso se ensancha más por dispersión |
| **Multimodo de gradiente de índice** | núcleo 50 a 100 µm, revestimiento 125 µm | Menor dispersión que el salto de índice |
| **Monomodo** | núcleo ~10 µm, revestimiento 125 µm | Un solo modo de propagación, mínima dispersión |

**Estructura del cable de fibra**: fibra óptica, tubo de acero liviano, Kevlar y cubierta exterior (*jacket*).

**Empalmes**

- Manuales o mecánicos
- Por fusión

<a id="c8-11"></a>
## 11. Ventanas de transmisión

La atenuación de la fibra depende de la longitud de onda, y se aprovechan las zonas de menor pérdida, llamadas **ventanas**:

| Ventana | Longitud de onda | Frecuencia aproximada |
|---|---|---|
| 1.ª | 850 nm | 60 THz |
| 2.ª | 1300 nm | 28 THz |
| 3.ª | 1550 nm | 20 THz |

La curva de atenuación resulta de la suma de varios fenómenos:

- Dispersión de Rayleigh
- Absorción ultravioleta
- Absorción infrarroja
- Picos de absorción por iones de agua

**Bandas de transmisión**

| Banda | Descripción | Rango |
|:-:|---|---|
| O | Original (segunda ventana) | 1260 a 1360 nm |
| E | Ampliada | 1360 a 1460 nm |
| S | Longitudes de onda corta | 1460 a 1530 nm |
| C | Convencional (ventana de erbio) | 1530 a 1565 nm |
| L | Longitudes de onda larga | 1565 a 1625 nm |
| U | Longitudes de onda ultralarga | 1625 a 1675 nm |

<a id="c8-12"></a>
## 12. Pérdidas por dispersión y acoplamiento

**Dispersión**: el pulso transmitido llega **ensanchado** al receptor. Ese ensanchamiento es $T_d = t_2 - t_1$ y limita el ancho de banda (medido en los puntos de −3 dB) y, por lo tanto, la velocidad.

**Pérdidas por acoplamiento** (cuando se unen dos fibras):

- Excesiva **separación** entre las fibras
- **Desplazamiento axial**
- **Desplazamiento angular**
- **Pulido incorrecto** de la fibra

En todos los casos parte del haz se pierde.

<a id="c8-13"></a>
## 13. Categorías, colores y conectores

**Categorías de fibra multimodo**

| Categoría | Ancho de banda modal mínimo [MHz·km] | 100 Mb (100BASE-FX) | 1 Gb (1000BASE-SX) | 10 Gb (10GBASE-SR) | 40 Gb | 100 Gb |
|---|:-:|:-:|:-:|:-:|:-:|:-:|
| OM1 (62,5/125) | 200 / 500 | hasta 2000 m | 275 m | 33 m | no soportado | no soportado |
| OM2 (50/125) | 500 / - | hasta 2000 m | 550 m | 82 m | no soportado | no soportado |
| OM3 (50/125, láser optimizada) | 1500 / 2000 | hasta 2000 m | 550 m | 300 m | 100 m (330 m con QSFP+ eSR4) | 100 m |
| OM4 (50/125, láser optimizada) | 3500 / 4700 | hasta 2000 m | 1000 m | 400 m | 150 m (550 m con QSFP+ eSR4) | 150 m |

**Código de colores de la cubierta** (aplicaciones no militares)

- Multimodo 50/125 (OM2): naranja
- Multimodo 50/125 optimizada láser (OM3, OM4): aqua
- Multimodo 62,5/125 (OM1): naranja
- Monomodo (OS1, OS2): amarillo
- Monomodo con mantenimiento de polarización: azul

**Tipos de conector:** SC, FC, APC, ST, LC, MU, MT-RJ y MTP/MPO (multifibra).

<a id="c8-14"></a>
## 14. Ventajas y desventajas de la fibra óptica

**Ventajas**

- Muy alta velocidad
- Largas distancias de transmisión
- Alta seguridad

**Desventajas**

- Costos elevados
- Difícil instalación
- Frágil

<a id="c8-15"></a>
## 15. LED y láser

**Esquema de transmisión:** fuente de información → circuito modulador → diodo láser → haz de láser → fotodiodo → circuito demodulador → sumidero de información.

- El **láser** tiene una **corriente umbral** a partir de la cual emite luz coherente. El LED emite de forma gradual.
- **Ancho espectral**: el del láser es más estrecho, típicamente 1 a 6 nm, frente a 25 a 40 nm del LED.

| Característica técnica | LED | Láser |
|---|---|---|
| Tipo de luz emitida | Incoherente | Coherente |
| Potencia óptima emitida | Baja | Alta |
| Ancho espectral | Grande | Pequeño |
| Direccionamiento de la luz | Menor | Mayor |
| Tiempo de crecimiento (10 % al 90 %) | 100 ns | 1 ns |
| Confiabilidad | Mayor | Menor |
| Vida útil | Aprox. $10^5$ h | Aprox. $10^5$ h |
| Circuitos estabilizadores y de enfriamiento | No | Sí |
| Ruido modal (distorsión de amplitud) | Bajo | Alto |
| Costo | Bajo | Alto |

<a id="c8-16"></a>
## 16. Mediciones en fibra óptica

Se utilizan un **medidor de potencia** y un equipo de **reflectometría** (que muestra la traza de atenuación en función de la distancia). En la traza se identifican **eventos**: curvaturas, empalmes por fusión, conectores APC y PC, y el corte final.

**Pérdidas típicas de potencia**

| Elemento | Pérdida media |
|---|:-:|
| Empalme mecánico | 0,4 dB |
| Empalme por fusión | 0,1 dB |
| Splitter 1:2 | 3,2 dB |
| Splitter 1:4 | 7,2 dB |
| Splitter 1:8 | 10,5 dB |
| Splitter 1:16 | 13,5 dB |
| Splitter 1:32 | 16,5 dB |
| Splitter 1:64 | 19,3 dB |
| Cable G.652 a 1310 nm | 0,35 dB/km |
| Cable G.652 a 1490 nm | 0,25 dB/km |

<a id="c8-17"></a>
## 17. Cables multifibra

Un cable multifibra se compone de vaina exterior, protección, vaina de polietileno, recubrimiento de sujeción y las fibras ópticas en su interior.

**Capas de un cable de fibra con protección** (de afuera hacia adentro):

1. Polietileno
2. Cinta de Mylar
3. Alambres de acero trenzado
4. Barrera de aluminio resistente al agua
5. Policarbonato
6. Tubo de cobre o aluminio
7. Petrolato
8. Fibras ópticas

<a id="c8-18"></a>
## 18. Cables submarinos

- Los enlaces intercontinentales usan **cables submarinos de fibra óptica**.
- Cada **30 a 50 km** se instalan **repetidores de amplificación óptica**, y en los extremos hay una **estación terrena**.
- El trazado debe sortear el relieve del fondo marino (por ejemplo, entre Estados Unidos y Europa: dorsal mesoatlántica a unos −2200 m y plataforma celta a unos −100 m).
- En Sudamérica hay anillos que conectan ciudades como Buenos Aires, Córdoba, Valparaíso, Lima, Fortaleza y Santos con Estados Unidos y Europa.
- Mapa interactivo de cables: www.submarinecablemap.com

---

<a id="clase-9"></a>
# Clase 9

## Índice de la Clase 9

- [1. Ventajas y desventajas de los medios inalámbricos](#c9-1)
- [2. Radiocomunicaciones y bandas de frecuencia](#c9-2)
- [3. Polarización de la señal electromagnética](#c9-3)
- [4. Antenas](#c9-4)
- [5. Propagación](#c9-5)
- [6. Propagación por onda terrestre](#c9-6)
- [7. Propagación por onda reflejada espacial o ionosférica](#c9-7)
- [8. Propagación por onda directa](#c9-8)
- [9. Cálculo de enlace radioeléctrico](#c9-9)
- [10. Ecuación del enlace por onda directa](#c9-10)
- [11. Zona de Fresnel](#c9-11)
- [12. Microondas](#c9-12)
- [13. Software de ayuda para cálculos de enlaces](#c9-13)
- [14. Satélites y características generales](#c9-14)
- [15. Órbitas satelitales](#c9-15)
- [16. Componentes del satélite y bandas de frecuencia](#c9-16)
- [17. Transpondedor](#c9-17)
- [18. Antenas satelitales](#c9-18)
- [19. Clasificación de satélites por función](#c9-19)
- [20. Satélites de órbita baja LEO](#c9-20)
- [21. Satélites de órbita media MEO](#c9-21)
- [22. Satélites de órbita geoestacionaria GEO](#c9-22)
- [23. Satélites de órbita excéntrica HEO](#c9-23)
- [24. Satélites argentinos](#c9-24)

<a id="c9-1"></a>
## 1. Ventajas y desventajas de los medios inalámbricos

**Ventajas**

- Flexibilidad
- Movilidad
- Fácil de expandir
- Costo efectivo
- Broadcast

**Desventajas**

- Temas de seguridad
- Velocidad limitada
- Interferencias

Ejemplos: Wi-Fi, Bluetooth, enlaces punto a punto, radio y satélite. **No olvidar los infrarrojos.**

<a id="c9-2"></a>
## 2. Radiocomunicaciones y bandas de frecuencia

| Nombre | ITU | Frecuencias | Longitud de onda | Servicios |
|---|:-:|---|---|---|
| Baja frecuencia (*Low Frequency*) | LF | 30 - 300 kHz | 10 - 1 km | Móvil marítimo, radionavegación, radiofaros |
| Media frecuencia (*Medium Frequency*) | MF | 300 - 3000 kHz | 1 km - 100 m | Radiodifusión |
| Alta frecuencia (*High Frequency*) | HF | 3 - 30 MHz | 100 - 10 m | Radioaficionados, comunicaciones, onda corta |
| Muy alta frecuencia (*Very High Frequency*) | VHF | 30 - 300 MHz | 10 - 1 m | TV, radio FM, radiollamadas, radioaficionados |
| Ultra alta frecuencia (*Ultra High Frequency*) | UHF | 300 - 3000 MHz | 1 m - 100 mm | Microondas, comunicaciones móviles, TV |
| Súper alta frecuencia (*Super High Frequency*) | SHF | 3 - 30 GHz | 100 - 10 mm | Microondas, satélites |
| Extra alta frecuencia (*Extremely High Frequency*) | EHF | 30 - 300 GHz | 10 - 1 mm | Satélites, radionavegación, satelital |

- Un enlace de radio consta de **transmisor**, **antena transmisora**, distancia entre antenas, **antena receptora** y **receptor**.
- El espectro también se designa con letras según el estándar IEEE (L, S, C, X, K<sub>u</sub>, K, K<sub>a</sub>, V, W, etc.), con bandas de radar y con las designaciones de la OTAN (A a O). Más allá de los GHz están el infrarrojo y la luz (lidar).

<a id="c9-3"></a>
## 3. Polarización de la señal electromagnética

- Una onda electromagnética tiene un **campo eléctrico** y un **campo magnético** perpendiculares entre sí y perpendiculares a la **dirección de propagación**.
- La **polarización** es la orientación del campo eléctrico:
  - **Lineal** (vertical u horizontal)
  - **Circular** (mano derecha o izquierda)
  - **Elíptica**

<a id="c9-4"></a>
## 4. Antenas

**Según su diagrama de radiación:**

- **Isotrópica**: irradia igual en todas direcciones (es una referencia teórica).
- **Omnidireccional**: irradia en todo el plano horizontal (forma de toroide).
- **Directiva**: concentra la energía en una dirección (lóbulo principal).

**Omnidireccionales**

- El ejemplo típico es el **dipolo**, cuyo diagrama es circular en el plano de azimut y en forma de "ocho" en el plano de elevación.
- Los campos eléctrico y magnético de la onda se asocian al **vector de Poynting**, que indica la dirección de propagación de la energía.

**Direccionales**

- **Yagi**: reflector, dipolo y directores.
- **Parabólica**: la superficie parabólica concentra los rayos en el **foco**.
- Parámetros del diagrama: **lóbulo principal**, **lóbulos secundarios** (por ejemplo, nivel de lóbulo secundario de 13 dB), ancho de haz a −3 dB ($BW_{3dB}$ de unos 20°) y relación frente/espalda **F/B** (por ejemplo, 20 dB).

<a id="c9-5"></a>
## 5. Propagación

Formas de propagación:

- **Onda terrestre** (superficial)
- **Onda directa** (línea de vista, LOS)
- **Onda reflejada espacial o ionosférica** (onda de cielo)
- **Vía satelital**

| Clasificación | Rango | Tipo de propagación |
|---|:-:|---|
| Frecuencia baja | < 2 MHz | La onda sigue la curvatura de la Tierra, pero puede bloquearse por un terreno desnivelado |
| Frecuencia media | 2 a 30 MHz | La onda puede reflejarse por las capas de la atmósfera, especialmente de la ionosfera |
| Frecuencia alta | > 30 MHz | La onda viaja en una línea directa y será bloqueada por obstrucciones |

<a id="c9-6"></a>
## 6. Propagación por onda terrestre

- La onda se desplaza siguiendo la superficie de la Tierra (**onda de superficie**).
- Junto con ella se tienen la **onda directa** y la **onda reflejada en la superficie** de la Tierra.
- Se usa en frecuencias bajas, con grandes torres y sistemas de antenas.

<a id="c9-7"></a>
## 7. Propagación por onda reflejada espacial o ionosférica

- Se basa en la **refracción/reflexión de la onda en la ionosfera**, la región de la atmósfera ionizada por la radiación solar (influye el viento solar y la actividad del Sol).
- La ionosfera comienza en la mesosfera. Las capas de la atmósfera son troposfera (hasta unos 12 km), estratosfera (hasta 50 km), mesosfera (hasta 80 km), termosfera (hasta 500 km) y exosfera.
- Capas de la ionosfera: **D, E, F1 y F2**, ubicadas aproximadamente entre 60 y 340 km de altura.
- La onda puede dar **varios saltos** entre la ionosfera y la Tierra, y así alcanzar grandes distancias.
- Si la frecuencia es demasiado alta, la onda **atraviesa** la ionosfera y no se refleja.

<a id="c9-8"></a>
## 8. Propagación por onda directa

- La **distancia de alcance visual** es la suma de las distancias al horizonte de cada antena.
- Se deduce con Pitágoras sobre el triángulo formado por el radio terrestre $R \approx 6500\ \text{km}$, la altura de la antena $h$ y la distancia al horizonte $D$:

$$D^2 + R^2 = (R + h)^2$$

$$D^2 = (R + h)^2 - R^2$$

$$D = \sqrt{R^2 + 2Rh + h^2 - R^2}$$

Como $R \gg h$:

$$D = \sqrt{2Rh} = \sqrt{2R}\,\sqrt{h}$$

Resultado, con $D$ en kilómetros y $h$ en metros:

$$D = 3{,}61\,\sqrt{h}$$

Considerando la **acción de la atmósfera** (refracción), el alcance aumenta:

$$D = 4{,}14\,\sqrt{h}$$

<a id="c9-9"></a>
## 9. Cálculo de enlace radioeléctrico

**Enunciado:** ¿cuál es la distancia máxima de un enlace de UHF si la antena receptora está a 25 m, la transmisora a 36 m, teniendo en cuenta la acción de la atmósfera y sin obstáculos en la línea de vista?

$$D_{h}\,A_1 = 4{,}14\,\sqrt{25} = 20{,}7\ \text{km}$$

$$D_{h}\,A_2 = 4{,}14\,\sqrt{36} = 24{,}84\ \text{km}$$

$$D_{max} = D_h A_1 + D_h A_2 = 20{,}7 + 24{,}84 = 45{,}54\ \text{km}$$

La distancia máxima para el enlace es de **45,54 km**.

<a id="c9-10"></a>
## 10. Ecuación del enlace por onda directa

Un enlace tiene un transmisor y un receptor con sus cables y antenas, y entre ambos la **pérdida en el espacio libre**. La señal que llega debe superar la **sensibilidad del receptor**, y la diferencia es el **margen**.

Pérdida en el espacio libre, con $d$ en km y $f$ en MHz:

$$L = 32{,}4 + 20 \log(d) + 20 \log(f)$$

**Ecuación del enlace:**

$$S_{rx} \le P_{tx} - L_{ctx} + G_{atx} - L_{enl} + G_{arx} - L_{crx} - FD$$

| Símbolo | Significado | Unidad |
|---|---|:-:|
| $S_{rx}$ | Sensibilidad del receptor | dBm |
| $P_{tx}$ | Potencia del transmisor | dBm |
| $L_{ctx}$ | Pérdida en el cable del transmisor | dB |
| $G_{atx}$ | Ganancia de la antena transmisora | dB |
| $L_{enl}$ | Pérdida del enlace (espacio libre) | dB |
| $G_{arx}$ | Ganancia de la antena receptora | dB |
| $L_{crx}$ | Pérdida en el cable del receptor | dB |
| $FD$ | Factor de desvanecimiento | dB |

<a id="c9-11"></a>
## 11. Zona de Fresnel

- Es la región elipsoidal entre las dos antenas por la que se propaga la mayor parte de la energía. Hay que mantenerla **despejada de obstáculos**.
- Se debe asegurar como mínimo el **60 %** de la primera zona de Fresnel despejada. Una obstrucción dentro de la zona agrega pérdidas (por ejemplo, 6, 16 o 20 dB según qué parte se obstruya).

Radio de la zona $n$, con $d_1$ y $d_2$ las distancias del punto a cada antena y $\lambda$ la longitud de onda:

$$r_n = \sqrt{\frac{n\, d_1\, d_2\, \lambda}{d_1 + d_2}}$$

Radio de la **primera zona**, con $D$ en km y $f$ en GHz:

$$r_1\,[\text{m}] = 8{,}66\,\sqrt{\frac{D\,[\text{km}]}{f\,[\text{GHz}]}}$$

**Ejemplo:** enlace entre la sede Córdoba y el Rectorado, con $D = 2{,}19\ \text{km}$ y $f = 5{,}8\ \text{GHz}$.

$$r_1 = 8{,}66\,\sqrt{\frac{2{,}19}{5{,}8}} \approx 5{,}32\ \text{m}$$

Como mínimo hay que tener despejado el 60 % de 5,32 m, es decir, aproximadamente **3,2 m**.

<a id="c9-12"></a>
## 12. Microondas

- Se usan **enlaces y repetidoras** en cadena, y cada tramo se llama **salto**. Requieren línea de vista.
- Longitud de salto típica según la banda:

| Intervalo de frecuencias [GHz] | Longitud de salto [km] |
|:-:|:-:|
| 1,5 a 2,5 | 60 |
| 4 a 6 | 50 |
| 7 a 8 | 45 |
| 11 a 13 | 25 a 35 |
| 15 a 20 | 10 a 20 |
| 30 | 5 |
| 40 a 60 | 2 a 0,5 |

**Ventajas**

- Altas tasas de transmisión
- Soporta largas distancias

**Desventajas**

- Requiere línea de vista
- Afectado por el clima
- Conexión por guía de ondas

<a id="c9-13"></a>
## 13. Software de ayuda para cálculos de enlaces

- Herramientas como **UISP Design Center** (https://ispdesign.ui.com/) permiten simular un enlace sobre un mapa.
- Se cargan ubicación, altura, potencia, ancho de canal y modelo de equipo de cada extremo.
- El programa muestra el perfil del terreno, la zona de Fresnel, la señal esperada y la capacidad del enlace (en el ejemplo de clase, el enlace Córdoba - Rectorado).

<a id="c9-14"></a>
## 14. Satélites y características generales

- Costo de instalación **independiente de la distancia**.
- Rápida instalación e implementación.
- Posibilidad de conexiones **punto a punto** y **multipunto**.
- Capacidad de **transporte y acceso**.
- Ancho de banda limitado, con uso de técnicas de ahorro espectral.
- Puede cubrir **amplias extensiones geográficas**.
- Puede **sortear barreras naturales**.
- Puede dar servicio en zonas **poco pobladas o de difícil acceso**.

Un satélite recibe la señal desde una estación terrestre y la retransmite hacia otras ciudades o estaciones.

<a id="c9-15"></a>
## 15. Órbitas satelitales

| Órbita | Tiempo orbital | Altitud |
|---|:-:|:-:|
| Baja (LEO) | ~90 minutos | 200 a 2000 km |
| Polar | ~100 minutos | ~1000 km |
| Intermedia (MEO / ICO) | ~6 horas | 10 000 a 14 000 km |
| Elíptica (HEO) | ~12 horas | 1000 a 70 000 km |
| Geoestacionaria (GEO) | 24 horas | 35 786 km |

En órbita geoestacionaria, **tres satélites a 120°** entre sí cubren toda la Tierra.

<a id="c9-16"></a>
## 16. Componentes del satélite y bandas de frecuencia

- **Antena receptora**: recibe señales desde las zonas de cobertura deseadas.
- **Antena transmisora**: transmite señales hacia las zonas de cobertura.
- **Transpondedor**: amplifica la señal recibida, traslada su frecuencia y la entrega para su retransmisión a la Tierra.
- **Paneles solares**: convierten la energía solar en eléctrica para toda la potencia que necesita el satélite.
- **Propulsor**: da incrementos de velocidad o frenos para corregir desviaciones de posición y orientación (usa combustible químico).

**Bandas de frecuencia**

| Banda | Frecuencia | Longitud de onda |
|:-:|:-:|:-:|
| L | 1 - 2 GHz | 30 - 15 cm |
| S | 2 - 4 GHz | 15 - 7,5 cm |
| C | 4 - 8 GHz | 7,5 - 3,75 cm |
| X | 8 - 12,4 GHz | 3,75 - 2,42 cm |
| K<sub>u</sub> | 12,4 - 18 GHz | 2,42 - 1,66 cm |
| K | 18 - 26,5 GHz | 1,66 - 1,11 cm |
| K<sub>a</sub> | 26,5 - 40 GHz | 11,1 - 7,5 mm |
| mm | 40 - 300 GHz | 7,5 - 1 mm |

<a id="c9-17"></a>
## 17. Transpondedor

Cadena de bloques: **LNA** → mezclador con **OL** → amplificador (**AMP**) → **IMUX** → **DRV** → mezclador con **OL** → **HPA** → **OMUX**.

- **LNA**: amplificador de bajo nivel de ruido.
- **OL**: oscilador.
- **HPA**: amplificador de potencia.
- **IMUX / OMUX**: multiplexor de entrada / de salida.
- **DRV**: preamplificador (*driver*).
- $f_u$: frecuencia de subida (*upload*). $f_d$: frecuencia de bajada (*download*).

**Funciones:**

- La función principal es **amplificar y cambiar la frecuencia** de la señal.
- El repetidor es **regenerativo** o **transparente**, según se procese o no la señal en banda base.
- Se divide en **sub-bandas** como canales de amplificación independiente y controlada.

<a id="c9-18"></a>
## 18. Antenas satelitales

- Estaciones terrenas de gran porte, como las de **Balcarce** (Buenos Aires) y **Bosque Alegre** (Córdoba).
- Antenas parabólicas de menor tamaño: de recepción de TV satelital, terminales satelitales portátiles y antenas de acceso instaladas en torres.

<a id="c9-19"></a>
## 19. Clasificación de satélites por función

- **Satélites de comunicación**: ayudan a transmitir y efectuar telecomunicaciones.
- **Satélites meteorológicos**: evalúan, miden y predicen condiciones climáticas de la Tierra.
- **Satélites de navegación**: permiten conocer la posición precisa y exacta de algo o alguien.
- **Satélites de reconocimiento**: llamados satélites espías, se usan en el ámbito militar o en servicios de inteligencia.
- **Satélites astronómicos**: se fabrican para observar galaxias, planetas, asteroides u otros objetos astronómicos.

<a id="c9-20"></a>
## 20. Satélites de órbita baja LEO

**LEO** (*Low Earth Orbit*)

- Orbitan entre **150 km y 2000 km**.
- A 800 km de altura se necesitan **90 minutos** para dar una vuelta completa a la Tierra.
- Para una estación terrestre permanece disponible solo unos pocos minutos.
- Para un servicio continuo se necesitan muchos satélites (**50 a 100**).
- Requieren **bajas potencias** de transmisión (menor consumo y costo).
- La recepción se puede efectuar con **antenas omnidireccionales**.
- Por lo anterior, son aptos para **comunicaciones personales móviles**.
- Los lanzamientos son de **bajo costo** debido a la altura de la órbita.
- **Bajo retardo** (delay de ~10 ms): favorece las comunicaciones de datos.

En una constelación LEO (tipo Iridium) los satélites se enlazan entre sí en **banda K** y se comunican con terminales móviles, teléfonos portátiles y vehículos en **banda L**.

<a id="c9-21"></a>
## 21. Satélites de órbita media MEO

**ICO** (*Intermediate Circular Orbit*) o **MEO** (*Medium Earth Orbit*)

- Las órbitas duran de **seis a ocho horas** (el satélite permanece visible entre una y dos horas).
- Para un servicio continuo con cobertura mundial se necesitan **diez satélites** en dos planos a 45° respecto del Ecuador.
- Requieren potencias **mayores** que los de órbita baja.
- Los lanzamientos cuestan menos que los geoestacionarios, pero más que los de órbita baja.
- El retardo (delay) es del orden de **70 ms**.
- Ejemplos: sistemas de navegación **GPS**, **GLONASS**, **BeiDou** y **Galileo**.

<a id="c9-22"></a>
## 22. Satélites de órbita geoestacionaria GEO

- **Período de rotación igual al de la Tierra** (23 h 56 m 4,5 s): parecen permanecer fijos en el espacio, con disponibilidad de 24 horas.
- Para un servicio continuo basta **un solo satélite** para unir dos puntos que puedan ser vistos por él, y **tres** para cubrir toda la Tierra.
- Requieren **altas potencias** de transmisión, antenas costosas del tipo parabólico y amplificadores de bajo ruido (LNA).
- La cantidad de satélites que pueden operar en la órbita geoestacionaria está **limitada por las interferencias** de los satélites ubicados a ambos lados.
- Los lanzamientos tienen **costos muy elevados**.
- **Retardo muy alto** (del orden de 250 ms entre estaciones terrestres).
- **Atenuación** por atmósfera y distancia de aproximadamente **200 dB**.
- En telefonía genera **ecos indeseados** y obliga a usar canceladores de eco.
- La distancia a la órbita geoestacionaria es de **35 786 km** desde el Ecuador.

<a id="c9-23"></a>
## 23. Satélites de órbita excéntrica HEO

**HEO** (*Highly Eccentric Orbit*)

- Órbitas muy excéntricas, inclinadas **63° o 116°**.
- **Perigeo**: 548 km. **Apogeo**: 39 957 km.
- Dan cobertura a **zonas de latitud alta** (por ejemplo, la ex URSS).
- Se necesitan como mínimo **3 satélites** para cubrir el área seleccionada.

<a id="c9-24"></a>
## 24. Satélites argentinos

**CONAE – INVAP**

- Satélites de Aplicaciones Científicas **SAC**: SAC-B (1996), SAC-A (1998), SAC-C (2000) y SAC-D/Aquarius (2011). Todos fuera de uso.
- Familia **SAOCOM** (Satélite Argentino de Observación con Microondas): SAOCOM 1A (2018) y 1B (2020), con observación en banda L. Está planeada la segunda constelación (serie 2).
- **SABIA-Mar**: constelación de dos satélites argentino-brasileños para información del mar (planeada para 2022).
- **ARSAT-1** (longitud 71°47'43" Oeste) y **ARSAT-2** (longitud 81°0'4" Oeste), en órbita geoestacionaria a 35 786 km.

**Satellogic**: está construyendo una constelación de **90 microsatélites** de observación de la Tierra, con capacidad de remapear semanalmente todo el planeta a alta resolución para proporcionar información geoespacial.

**Innova Space**: nació como el proyecto de un profesor y sus alumnos de la escuela técnica N.° 5 de Mar del Plata, que construyeron un **picosatélite** y lo lanzaron al espacio. Luego crearon la empresa, que ya lanzó varios picosatélites.

## 15. Cuantificación

Las muestras tomadas pueden tener infinitos valores posibles, y no se pueden representar con una cantidad finita de bits. La **cuantificación** transforma cada muestra en el **nivel cuántico** más próximo de un conjunto finito de niveles.

- La entrada es $S(t)$ y la salida del cuantificador es $C(t)$, con forma de **escalera**.
- La distancia entre dos niveles consecutivos es el **salto o paso de cuantificación**.
- Con $n$ bits por muestra se tienen $L = 2^n$ niveles.
- Ejemplo de la clase: 3 bits → 8 niveles (000, 001, 010, 011, 100, 101, 110, 111), repartidos entre el máximo nivel positivo y el máximo nivel negativo de la señal. Toda muestra que cae dentro de una zona (por ejemplo, la "zona 101") se representa con el código de esa zona.
- Al redondear se introduce un **error de cuantificación**: es irreversible, y el receptor nunca podrá recuperar el valor exacto original, solo el nivel asignado.

## 16. Cuantificación uniforme

En la **cuantificación uniforme** todos los escalones tienen **el mismo tamaño**, sin importar la amplitud de la señal.

- La curva de transferencia entrada-salida (curva A) es una escalera de pasos iguales.
- El **error de cuantificación** es la diferencia entre la señal analógica y los pulsos cuánticos. En cada muestra, como máximo vale **la mitad del escalón** ($\pm \Delta/2$).
- Cuantos más bits se usen, más pequeños son los escalones y menor es el error. Como regla práctica, **cada bit adicional mejora la relación señal/ruido de cuantificación unos 6 dB**.
- **Desventaja:** el error absoluto es el mismo para señales fuertes y débiles, por lo que las señales de **baja amplitud** quedan con una relación señal/ruido de cuantificación peor. Eso motiva la cuantificación no uniforme.

## 17. Cuantificación no uniforme

Para dar mejor tratamiento a las señales de poca amplitud (como la voz, donde predominan los valores bajos) se usan **escalones de tamaño variable**: pequeños para amplitudes bajas y grandes para amplitudes altas.

- Se implementa con un **compresor** seguido de un **cuantificador uniforme**: $S(t)$ → compresor → $S'(t)$ → cuantificador uniforme → $C(t)$.
- El compresor tiene una **ley de compresión** (curva logarítmica) que "estira" las amplitudes bajas y "comprime" las altas. Así, los saltos de entrada son más chicos donde la señal es débil ($\Delta t_2 < \Delta t_1$ en el gráfico).
- En la práctica la curva se aproxima por **segmentos rectos** (13 segmentos en el gráfico de la clase), con cada segmento dividido en pasos uniformes.
- En el receptor se aplica el proceso inverso, un **expansor**. El conjunto compresor-expansor se llama **compansor**.

## 18. Codificación

La **codificación** asigna a cada nivel cuantificado un **código binario**. Con $n$ bits por muestra, cada pulso cuantificado se convierte en una palabra de $n$ bits.

| Nivel de amplitud (V) | Código binario |
|:-:|:-:|
| 0 | 000 |
| 1 | 001 |
| 2 | 010 |
| 3 | 011 |
| 4 | 100 |
| 5 | 101 |
| 6 | 110 |
| 7 | 111 |

Ejemplo de la clase: los pulsos cuantificados **7, 6, 4, 5** se transmiten como `111 110 100 101`.

**Velocidad de la señal digital resultante:**

$$V = f_m \cdot n \quad [\text{bps}]$$

Ejemplo: telefonía, con $f_m = 8000$ muestras/s y $n = 8$ bits, da $V = 64\,000$ bps.

---

<a id="clase-10"></a>
# Clase 10

## Índice de la Clase 10

- [1. Modulación y demodulación](#c10-1)
- [2. Métodos de modulación](#c10-2)
- [3. Clasificación según moduladora y portadora](#c10-3)
- [4. Modulación por onda continua](#c10-4)
- [5. Modulación de amplitud AM y ASK](#c10-5)
- [6. Modulación de frecuencia FM y FSK](#c10-6)
- [7. Modulación de fase PM y PSK](#c10-7)
- [8. Modulación de fase diferencial DPSK](#c10-8)
- [9. Modulación multifase](#c10-9)
- [10. Modulación multifase y multinivel](#c10-10)
- [11. Modulación por pulsos](#c10-11)
- [12. Modulación de pulsos analógica](#c10-12)
- [13. Digitalización](#c10-13)
- [14. Muestreo](#c10-14)
- [15. Cuantificación](#c10-15)
- [16. Cuantificación uniforme](#c10-16)
- [17. Cuantificación no uniforme](#c10-17)
- [18. Codificación](#c10-18)
- [19. Modulación por pulsos digital](#c10-19)
- [20. Modulación por pulsos codificados PCM](#c10-20)
- [21. Modulación delta DM](#c10-21)
- [22. Modulación delta adaptativa](#c10-22)

<a id="c10-1"></a>
## 1. Modulación y demodulación

La **modulación** es el proceso por el cual una señal que contiene la **información** (la **señal moduladora**) modifica alguna característica de otra señal, llamada **portadora**, para obtener la **señal modulada**, que es la que realmente se envía por el canal.

| Señal | Símbolo | Descripción |
|---|:-:|---|
| Moduladora | $s(t)$ | Contiene la información. Es $a(t)$ si es de origen analógico y $d(t)$ si es de origen digital |
| Portadora | $p(t)$ | Señal auxiliar que "transporta" la información |
| Modulada | $m(t)$ | Resultado de combinar moduladora y portadora |

- El **modulador** recibe la portadora y la moduladora, y entrega la modulada $m(t)$.
- El **demodulador** hace el proceso inverso: recibe $m(t)$, **recupera la moduladora** y **descarta la portadora**, que ya cumplió su función de transporte.

**¿Para qué se modula?**

- **Adaptar la señal al medio.** Una antena eficiente tiene un tamaño comparable a la longitud de onda ($\lambda = c/f$). Para una señal de voz de 3 kHz, $\lambda$ sería de unos 100 km, lo que es impráctico. Al trasladar la información a una portadora de alta frecuencia, las antenas se vuelven de tamaño razonable.
- **Multiplexar por frecuencia.** Varias señales pueden compartir un mismo medio si cada una usa una portadora distinta.
- **Mejorar la inmunidad al ruido y a las interferencias**, según el método de modulación elegido.
- **Transmitir datos digitales por canales pensados para señales analógicas**, como la línea telefónica. De ahí el nombre **módem** (modulador-demodulador).

<a id="c10-2"></a>
## 2. Métodos de modulación

Los métodos se dividen según el tipo de portadora que se utiliza.

**Modulación por onda continua** (portadora senoidal)

- **Modulación de amplitud**: ASK (*Amplitude Shift Keying*).
- **Modulación de frecuencia**: FSK (*Frequency Shift Keying*), de banda angosta o de banda ancha.
- **Modulación de fase**: PSK (*Phase Shift Keying*), con PSK convencional, **DPSK** (diferencial) y la **modulación multifase y multinivel** (4PSK, 8PSK, 16PSK, 16QAM, MQAM).

**Modulación por pulsos** (portadora formada por un tren de pulsos)

- **Analógica**: PAM (amplitud de pulsos), PDM (duración o variación del ancho de los pulsos) y PPM (posición del pulso).
- **Digital**: PCM (modulación por pulsos codificados), DM (modulación delta), modulación delta adaptativa y modulación diferencial (CM o de Q niveles).

<a id="c10-3"></a>
## 3. Clasificación según moduladora y portadora

El tipo de método depende de si la información (moduladora) y la portadora son analógicas o digitales.

| | **Portadora analógica** $p(t)$ | **Portadora digital** $p(t)$ |
|---|---|---|
| **Moduladora analógica** $s(t)$ (información) | **AM, FM, PM**. $m(t)$: modulada analógica | **PAM, PDM, PPM**. $m(t)$: modulada analógica |
| **Moduladora digital** $s(t)$ (información) | **ASK, FSK, PSK**. $m(t)$: modulada analógica | **PCM, DELTA, DELTA adaptativa**. $m(t)$: modulada digital |

- $s(t)$: moduladora → información.
- $p(t)$: portadora.
- $m(t)$: modulada.

Notar que ASK, FSK y PSK transmiten información **digital** usando una portadora **analógica** (senoidal), por eso la señal modulada resultante es analógica. Solo en la modulación por pulsos con moduladora digital (PCM, delta) la señal final es digital.

<a id="c10-4"></a>
## 4. Modulación por onda continua

La portadora es una señal **senoidal** de la forma:

$$p(t) = A_p \,\sin(\omega_p t + \theta_p)$$

(en la diapositiva se escribe como $f(x) = A\,\text{sen}(n\omega + \phi)$).

| Parámetro | Significado |
|---|---|
| $f_p = \dfrac{1}{T_p}$ | Frecuencia de la portadora |
| $T_p$ | Período de la portadora |
| $A_p$ | Amplitud máxima de la portadora |
| $\omega_p = 2\pi f_p$ | Pulsación de la portadora |
| $\theta_p$ | Fase de la portadora |

Una senoide tiene **tres parámetros** que se pueden variar para "imprimirle" la información. Cada uno da lugar a una familia de modulaciones:

- Variar la **amplitud** $A_p$ → modulación de amplitud (AM / ASK).
- Variar la **frecuencia** $f_p$ → modulación de frecuencia (FM / FSK).
- Variar la **fase** $\theta_p$ → modulación de fase (PM / PSK).

<a id="c10-5"></a>
## 5. Modulación de amplitud AM y ASK

La **amplitud** de la portadora varía en función de la moduladora, mientras que la frecuencia y la fase se mantienen constantes.

**AM (moduladora analógica)**

- La **envolvente** de la señal modulada reproduce la forma de la señal moduladora $a(t)$.
- Sin modulación, la portadora tiene amplitud constante $A_p$. Al comenzar la modulación, su amplitud sube y baja siguiendo a $a(t)$.
- Forma general, con $k$ el índice de modulación:

$$m(t) = A_p\,[\,1 + k\,a(t)\,]\,\sin(\omega_p t)$$

- **Espectro:** la moduladora ocupa de $-B$ a $+B$. Al modular, ese espectro se **desplaza** alrededor de $\pm f_p$, y queda la señal modulada entre $f_p - B$ y $f_p + B$. Por lo tanto, el ancho de banda necesario es:

$$BW_{AM} = 2B$$

- Aplicación típica: **radiodifusión AM**.

**ASK (moduladora digital)**

- La amplitud de la portadora toma **dos valores**, según el bit: un nivel para el "1" y otro para el "0".
- En el caso más simple, la portadora aparece para el "1" y se **suprime** para el "0" (secuencia $d(t)$ = 1 0 1 0 1 0 1 en la diapositiva).
- Es muy sencilla de generar y detectar, pero **sensible al ruido**, porque el ruido se suma justamente sobre la amplitud, que es donde está la información.

<a id="c10-6"></a>
## 6. Modulación de frecuencia FM y FSK

La **frecuencia** de la portadora varía según la moduladora, y la **amplitud permanece constante**.

**FM (moduladora analógica)**

- La frecuencia instantánea sigue a la señal de entrada:

$$f_i(t) = f_p + k_f \, a(t)$$

- Cuando la señal moduladora es **máxima positiva**, la portadora tiene la frecuencia **más alta** (período más corto).
- Cuando la señal es **máxima negativa**, la portadora tiene la frecuencia **más baja** (período más largo).
- Como la información está en la frecuencia y no en la amplitud, es **mucho más inmune al ruido** que la AM. A cambio, ocupa **más ancho de banda**.
- Aplicación típica: **radiodifusión FM** y los transmisores de radio de alta calidad.

**FSK (moduladora digital)**

- Cada bit se representa con una **frecuencia distinta**: una para el "1" ($f_1$) y otra para el "0" ($f_2$).
- Según la separación entre ambas frecuencias, se habla de **FSK de banda angosta** o **de banda ancha**.
- Mantiene la ventaja de la FM frente al ruido, y es muy usada en módems de baja velocidad.

<a id="c10-7"></a>
## 7. Modulación de fase PM y PSK

Se varía la **fase** de la portadora respecto de la señal sin modular, y la amplitud y la frecuencia base se mantienen.

**PM (moduladora analógica)**

$$m(t) = A_p \,\sin\big(\omega_p t + k_p\, a(t)\big)$$

- La fase y la frecuencia están relacionadas: la frecuencia instantánea es la derivada de la fase. Por eso, en la señal modulada se observan desviaciones de frecuencia respecto de la **frecuencia de reposo**, que son máximas cuando la pendiente de la moduladora es máxima y nulas cuando la pendiente es cero (en los cruces por cero y los picos).

**PSK (moduladora digital)**

- Cada bit se asocia a una **fase** distinta de la portadora.
- En su forma más simple, **BPSK**, hay dos fases separadas 180°: $0$ y $\pi$ (puntos A y B de la circunferencia).
- El radio de la circunferencia representa la **amplitud normalizada** de la portadora (igual a 1), y la posición sobre ella indica la fase.
- Cada vez que cambia el bit, se produce un **cambio de fase** en la señal modulada.

<a id="c10-8"></a>
## 8. Modulación de fase diferencial DPSK

En la PSK común el receptor necesita conocer la **fase absoluta** de la portadora para decidir si un bit es 0 o 1. En la **DPSK** la información se codifica en la **diferencia** entre bits consecutivos, y se elimina esa necesidad.

**Transmisor**

1. Un **codificador diferencial de 1 bit**: la compuerta **XNOR** combina el dato actual con el dato codificado anterior, que llega por una realimentación con **retardo de 1 bit**.
2. El resultado (datos codificados) entra a un **modulador BPSK**, y sale la señal **DBPSK**.

Tabla de verdad de la XNOR:

| A | B | A XNOR B |
|:-:|:-:|:-:|
| 0 | 0 | 1 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

En la **constelación BPSK** hay dos puntos: el bit codificado 1 se transmite con fase $0$ y el bit codificado 0 con fase $\pi$.

**Ejemplo de la clase** (el retardo arranca en 0):

| Bit | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 | 14 |
|---|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| Datos | 0 | 1 | 1 | 1 | 0 | 0 | 1 | 0 | 1 | 1 | 1 | 1 | 0 | 0 |
| Realimentación (retardo) | 0 | 1 | 1 | 1 | 1 | 0 | 1 | 1 | 0 | 0 | 0 | 0 | 0 | 1 |
| Datos codificados | 1 | 1 | 1 | 1 | 0 | 1 | 1 | 0 | 0 | 0 | 0 | 0 | 1 | 0 |
| DBPSK (fase) | 0 | 0 | 0 | 0 | $\pi$ | 0 | 0 | $\pi$ | $\pi$ | $\pi$ | $\pi$ | $\pi$ | 0 | $\pi$ |

**Receptor**

1. Un **demodulador BPSK** recupera los datos codificados.
2. Un **decodificador diferencial de 1 bit** compara cada bit codificado con el anterior (retardado 1 bit) mediante la misma compuerta, y se obtienen los **datos originales**.

<a id="c10-9"></a>
## 9. Modulación multifase

En lugar de usar solo dos fases, se usan $M$ fases distintas. Cada fase representa un **grupo de bits**, entonces cada cambio de fase (cada **símbolo** o **baudio**) transporta más de un bit.

**4PSK (QPSK)**: 4 fases, 2 bits por símbolo.

| N.° de secuencia | Secuencia de bits | Fase asignada |
|:-:|:-:|:-:|
| 1 | 00 | 0° |
| 2 | 01 | 90° |
| 3 | 11 | 180° |
| 4 | 10 | 270° |

**8PSK**: 8 fases separadas 45°, 3 bits por símbolo.

| N.° de secuencia | Dígitos binarios | Fase asignada |
|:-:|:-:|:-:|
| 1 | 011 | 0° |
| 2 | 010 | 45° |
| 3 | 000 | 90° |
| 4 | 001 | 135° |
| 5 | 101 | 180° |
| 6 | 100 | 225° |
| 7 | 110 | 270° |
| 8 | 111 | 315° |

Notar que las asignaciones de bits entre fases vecinas difieren en **un solo bit**, de modo que un error de fase pequeño provoca, a lo sumo, un bit errado.

**Relación entre velocidad de símbolos y de bits.** Con $M$ estados posibles, cada símbolo transporta $\log_2 M$ bits:

$$V_{bits} = V_{baudios} \cdot \log_2 M$$

Es la misma idea de la señal multinivel de la [Clase 6](#clase-6): $C = 2B\log_2 n$. Se aumenta la velocidad de bits **sin aumentar el ancho de banda**, a costa de que las fases estén más próximas entre sí y el sistema sea más sensible al ruido.

<a id="c10-10"></a>
## 10. Modulación multifase y multinivel

Para transportar aún más bits por símbolo se combinan **dos parámetros a la vez**: la **fase** y la **amplitud**. Esto se conoce como **QAM** (*Quadrature Amplitude Modulation*).

**Ejemplo de 16 estados** (esquema de módems para línea telefónica):

- **8 fases** (cada 45°) y **2 amplitudes** por fase, es decir, $8 \times 2 = 16$ estados, que equivalen a **4 bits por símbolo** ($Q_1$ a $Q_4$).
- $Q_1$ selecciona la **amplitud** (menor o mayor) y $Q_2$, $Q_3$ y $Q_4$ seleccionan la **fase**.
- Las amplitudes relativas son **3 y 5** sobre los ejes (0°, 90°, 180°, 270°) y **$\sqrt{2}$ y $3\sqrt{2}$** sobre las diagonales (45°, 135°, 225°, 315°).

**Constelaciones de mayor orden** (módems de alta velocidad):

- Se ubican muchos puntos en el plano fase-amplitud. En el diagrama de la clase, cada punto está identificado por un código de **7 bits**, es decir, $2^7 = 128$ estados.
- Cuantos más puntos hay, más bits por símbolo se transmiten, pero **menor es la distancia entre puntos**, por lo que se necesita una mejor relación señal/ruido ([Teorema de Shannon-Hartley, Clase 6](#clase-6)).

<a id="c10-11"></a>
## 11. Modulación por pulsos

En la modulación por pulsos, la portadora no es una senoide sino un **tren de pulsos** periódicos. Se describe con tres parámetros:

| Parámetro | Significado |
|---|---|
| $T$ | Período (tiempo entre pulsos) |
| $A$ | Amplitud del pulso |
| $D$ | Duración (ancho) del pulso dentro del período |

Al igual que en la onda continua, se puede variar cada parámetro:

- Variar $A$ → **PAM**.
- Variar $D$ → **PDM**.
- Variar la posición del pulso dentro del período → **PPM**.

Si la moduladora es analógica se obtiene **modulación de pulsos analógica** (PAM, PDM, PPM). Si la moduladora es digital se obtiene la **modulación por pulsos digital** (PCM, delta, delta adaptativa).

<a id="c10-12"></a>
## 12. Modulación de pulsos analógica

La señal analógica de entrada se **muestrea** con el tren de pulsos de la portadora, y la información queda contenida en una característica del pulso:

- **PAM** (*Pulse Amplitude Modulation*): la **amplitud** de cada pulso es proporcional al valor de la señal en ese instante. Los pulsos siguen la forma de la señal analógica.
- **PDM** (*Pulse Duration Modulation*): la **duración** (ancho) de cada pulso es proporcional al valor de la señal.
- **PPM** (*Pulse Position Modulation*): la **posición** del pulso respecto de su instante nominal varía con el valor de la señal.

Aunque la señal se transmite en forma de pulsos, la **información sigue siendo analógica**, porque la amplitud, el ancho o la posición pueden tomar cualquier valor continuo. Por eso la señal modulada es analógica. La **PAM** es la primera etapa de la digitalización por PCM.

<a id="c10-13"></a>
## 13. Digitalización

Muchas señales (voz, video, mediciones) nacen como **analógicas**: en ellas "la inteligencia está en la forma de onda". Para transmitirlas o procesarlas en sistemas digitales se las convierte en una secuencia de bits mediante un **conversor A/D**.

**Etapas del conversor A/D**

| Etapa | Entrada → Salida | Qué hace |
|---|---|---|
| **Muestreador** | $x_a(t)$ → $x(n)$ | Toma valores de la señal en instantes discretos. Resultado: señal en **tiempo discreto** |
| **Cuantificador** | $x(n)$ → $x_q(n)$ | Redondea cada muestra a uno de un número finito de niveles. Resultado: señal **cuantificada** |
| **Codificador** | $x_q(n)$ → señal digital | Asigna a cada nivel un código binario. Resultado: **señal digital** |

**¿Por qué digitalizar?** Una señal digital se puede **regenerar** (no solo amplificar) en repetidores, por lo que el ruido no se acumula, como se vio con la regeneración en la [Clase 2](#clase-2). Además, es más robusta frente al ruido, se puede multiplexar, comprimir, cifrar y detectar o corregir errores con los métodos de la [Clase 7](#clase-7).

<a id="c10-14"></a>
## 14. Muestreo

El **muestreo** consiste en tomar el valor de la señal analógica a intervalos regulares $T_m$. La **frecuencia de muestreo** es $f_m = \dfrac{1}{T_m}$.

**Teorema de Nyquist (de muestreo):** para poder reconstruir la señal original sin pérdida de información, la frecuencia de muestreo debe ser, como mínimo, el **doble de la frecuencia máxima** de la señal:

$$f_{muestreo\ minima} \ge 2\, f_{max}$$

- Si se muestrea por debajo de ese valor se produce **aliasing** (solapamiento de espectros): componentes de alta frecuencia aparecen como falsas componentes de baja frecuencia y la señal no se puede reconstruir.
- Ejemplo: en telefonía, la voz se limita a unos 4 kHz, por lo que se muestrea a $2 \times 4000 = 8000$ muestras por segundo.

**Tipos de muestreo**

- **Ideal**: se toma un **impulso instantáneo** en cada instante de muestreo. Es un modelo teórico.
- **Natural**: se toma un **pulso de corta duración** cuya amplitud acompaña la forma de la señal durante ese tiempo (amplitud variable).
- **Flat top** (*sample and hold*): similar al natural, pero cada pulso mantiene un **valor simple de amplitud constante**, el de la muestra tomada, durante todo su ancho. Es el más fácil de implementar en la práctica.

<a id="c10-15"></a>
## 15. Cuantificación

Las muestras tomadas pueden tener infinitos valores posibles, y no se pueden representar con una cantidad finita de bits. La **cuantificación** transforma cada muestra en el **nivel cuántico** más próximo de un conjunto finito de niveles.

- La entrada es $S(t)$ y la salida del cuantificador es $C(t)$, con forma de **escalera**.
- La distancia entre dos niveles consecutivos es el **salto o paso de cuantificación**.
- Con $n$ bits por muestra se tienen $L = 2^n$ niveles.
- Ejemplo de la clase: 3 bits → 8 niveles (000, 001, 010, 011, 100, 101, 110, 111), repartidos entre el máximo nivel positivo y el máximo nivel negativo de la señal. Toda muestra que cae dentro de una zona (por ejemplo, la "zona 101") se representa con el código de esa zona.
- Al redondear se introduce un **error de cuantificación**: es irreversible, y el receptor nunca podrá recuperar el valor exacto original, solo el nivel asignado.

<a id="c10-16"></a>
## 16. Cuantificación uniforme

En la **cuantificación uniforme** todos los escalones tienen **el mismo tamaño**, sin importar la amplitud de la señal.

- La curva de transferencia entrada-salida (curva A) es una escalera de pasos iguales.
- El **error de cuantificación** es la diferencia entre la señal analógica y los pulsos cuánticos. En cada muestra, como máximo vale **la mitad del escalón** ($\pm \Delta/2$).
- Cuantos más bits se usen, más pequeños son los escalones y menor es el error. Como regla práctica, **cada bit adicional mejora la relación señal/ruido de cuantificación unos 6 dB**.
- **Desventaja:** el error absoluto es el mismo para señales fuertes y débiles, por lo que las señales de **baja amplitud** quedan con una relación señal/ruido de cuantificación peor. Eso motiva la cuantificación no uniforme.

<a id="c10-17"></a>
## 17. Cuantificación no uniforme

Para dar mejor tratamiento a las señales de poca amplitud (como la voz, donde predominan los valores bajos) se usan **escalones de tamaño variable**: pequeños para amplitudes bajas y grandes para amplitudes altas.

- Se implementa con un **compresor** seguido de un **cuantificador uniforme**: $S(t)$ → compresor → $S'(t)$ → cuantificador uniforme → $C(t)$.
- El compresor tiene una **ley de compresión** (curva logarítmica) que "estira" las amplitudes bajas y "comprime" las altas. Así, los saltos de entrada son más chicos donde la señal es débil ($\Delta t_2 < \Delta t_1$ en el gráfico).
- En la práctica la curva se aproxima por **segmentos rectos** (13 segmentos en el gráfico de la clase), con cada segmento dividido en pasos uniformes.
- En el receptor se aplica el proceso inverso, un **expansor**. El conjunto compresor-expansor se llama **compansor**.

<a id="c10-18"></a>
## 18. Codificación

La **codificación** asigna a cada nivel cuantificado un **código binario**. Con $n$ bits por muestra, cada pulso cuantificado se convierte en una palabra de $n$ bits.

| Nivel de amplitud (V) | Código binario |
|:-:|:-:|
| 0 | 000 |
| 1 | 001 |
| 2 | 010 |
| 3 | 011 |
| 4 | 100 |
| 5 | 101 |
| 6 | 110 |
| 7 | 111 |

Ejemplo de la clase: los pulsos cuantificados **7, 6, 4, 5** se transmiten como `111 110 100 101`.

**Velocidad de la señal digital resultante:**

$$V = f_m \cdot n \quad [\text{bps}]$$

Ejemplo: telefonía, con $f_m = 8000$ muestras/s y $n = 8$ bits, da $V = 64\,000$ bps.

<a id="c10-19"></a>
## 19. Modulación por pulsos digital

Se usa una **portadora digital** (tren de pulsos) y una **moduladora digital** o digitalizada. Es el caso de la última celda de la tabla de clasificación, y la señal modulada resultante es **digital**. Incluye:

- **Modulación por pulsos codificados** (PCM).
- **Modulación delta** (DM).
- **Modulación delta adaptativa**.

<a id="c10-20"></a>
## 20. Modulación por pulsos codificados PCM

La **PCM** (*Pulse Code Modulation*) es el método estándar de digitalización de señales analógicas. Reúne en un solo codificador las tres etapas vistas:

1. **Muestreo** (*sampling*): la señal analógica se convierte en una señal **PAM**.
2. **Cuantificación** (*quantizing*): los pulsos PAM se llevan a niveles discretos.
3. **Codificación** (*encoding*): cada nivel se convierte en un código binario, y se obtienen los **datos digitales** (por ejemplo, `11...1100`).

Los parámetros que definen una PCM son la **frecuencia de muestreo** $f_m$ (que debe cumplir Nyquist) y el **número de bits por muestra** $n$. De ellos resultan la calidad de la señal reconstruida y la velocidad de transmisión $V = f_m \cdot n$.

La PCM necesita **más ancho de banda** que la señal analógica original, pero a cambio la señal digital es mucho más robusta frente al ruido.

<a id="c10-21"></a>
## 21. Modulación delta DM

La **modulación delta** transmite, en cada instante de muestreo, **un solo bit** que indica si la señal debe **subir o bajar un escalón** de altura fija. No se transmite el valor de la muestra sino la **variación** respecto de una aproximación escalonada.

**Funcionamiento** (según el esquema de la clase)

- El **amplificador diferencial** compara la señal de entrada $e(t)$ con la señal escalonada $s(t)$, y entrega $a(t)$.
- El **generador de pulsos** $d(t)$ marca los instantes de muestreo.
- El **modulador de pulsos** emite un pulso positivo ($+A$) si $e(t) > s(t)$ o negativo ($-A$) en caso contrario. Esa es la salida $p(t)$.
- El **integrador** acumula los pulsos de salida y reconstruye la señal escalonada $s(t)$ que realimenta al comparador.

**Fases y problemas**

- **Arranque**: al comienzo, la señal escalonada parte de cero y sube escalón a escalón hasta alcanzar la señal.
- **Persecución**: luego $s(t)$ oscila alrededor de $e(t)$, subiendo y bajando un escalón por vez.
- **Sobrecarga de pendiente**: si la señal cambia más rápido de lo que el escalón puede seguir, $s(t)$ se queda atrás. Para evitarlo se debe cumplir aproximadamente:

$$\Delta \cdot f_m \ge \left|\frac{de(t)}{dt}\right|_{max}$$

- Si en cambio el escalón es grande y la señal casi no cambia, aparece el **ruido granular**: $s(t)$ oscila sin necesidad.

**Ventaja:** es muy simple y usa un solo bit por muestra.

<a id="c10-22"></a>
## 22. Modulación delta adaptativa

La **delta adaptativa** resuelve el compromiso de la delta común haciendo que el **escalón sea variable**, con una altura que se mueve entre un valor mínimo ($A_{min}$) y uno máximo ($A_{max}$).

- Cuando la señal **cambia rápido** (por ejemplo, subidas fuertes), el escalón **aumenta** hacia $A_{max}$, lo que reduce la sobrecarga de pendiente.
- Cuando la señal **varía lentamente**, el escalón **disminuye** hacia $A_{min}$, lo que reduce el ruido granular.

De este modo se obtiene una mejor aproximación de la señal original con la misma cantidad de bits por muestra (un bit), a costa de un circuito algo más complejo que decide cómo cambiar el escalón.

---

<a id="clase-11"></a>
# Clase 11

## Índice de la Clase 11

- [1. Multiplexación y concentración](#c11-1)
- [2. Técnicas de multiplexación](#c11-2)
- [3. Multiplexación por división de frecuencia FDM](#c11-3)
- [4. Jerarquía analógica de FDM](#c11-4)
- [5. Multiplexación por división de longitud de onda WDM](#c11-5)
- [6. Multiplexación por división de tiempo TDM](#c11-6)
- [7. Entramado de bits y de caracteres](#c11-7)
- [8. Esquema básico de multiplexación digital](#c11-8)
- [9. Jerarquía digital plesiócrona PDH](#c11-9)
- [10. Tramas E1 y T1](#c11-10)
- [11. Trama E2](#c11-11)
- [12. Jerarquía digital sincrónica SDH](#c11-12)
- [13. Trama STM-N](#c11-13)
- [14. Multiplexación por división de tiempo estadística STDM](#c11-14)
- [15. Sincronización y reloj](#c11-15)
- [16. Tipos de reloj y modos de operación](#c11-16)
- [17. Protocolo de precisión de tiempo PTP](#c11-17)
- [18. Ejemplo de cálculo con PTP](#c11-18)

<a id="c11-1"></a>
## 1. Multiplexación y concentración

**Multiplexar** es transmitir varios canales de información independientes por un **único canal físico**, de modo que todos compartan el mismo medio. Así se evita tender un medio por cada comunicación, lo que abarata el sistema.

- En el origen (**fuente**), el **multiplexor** (Mx) recibe los canales de entrada $C_1, C_2, \dots, C_n$ y los reúne en un **canal único**.
- En el destino (**sumidero**), el equipo del otro extremo hace la operación inversa (demultiplexación) y entrega cada canal $C_1', C_2', \dots, C_n'$ a su destinatario.

**Relación entre las capacidades.** Sea $C_c$ la capacidad del canal común y $C_i$ la capacidad de cada canal de entrada:

$$\text{Multiplexor:} \quad C_c \ge \sum_{i=1}^{n} C_i$$

$$\text{Concentrador:} \quad C_c \le \sum_{i=1}^{n} C_i$$

- En el **multiplexor**, el canal común puede transportar a todos los canales a la vez, y a cada uno se le reserva su porción.
- En el **concentrador**, el canal común es menor que la suma de las entradas, y se confía en que no todos los canales transmitan al mismo tiempo (se aprovechan los momentos en que algunos están inactivos). Es la idea que está detrás de la multiplexación estadística (ver [sección 14](#c11-14)).

Ejemplo: 30 canales de 64 kbps suman $30 \times 64 = 1920$ kbps, que entran en un canal de 2048 kbps (E1), con el resto reservado para sincronismo y señalización.

<a id="c11-2"></a>
## 2. Técnicas de multiplexación

| Técnica | Sigla | Qué se reparte entre los canales |
|---|:-:|---|
| Multiplexado por división de **frecuencia** | **FDM** (*Frequency Division Multiplexing*) | El **ancho de banda**: cada canal ocupa una banda de frecuencias propia |
| Multiplexado por división de **tiempo** | **TDM** (*Time Division Multiplexing*) | El **tiempo**: cada canal usa el medio en intervalos asignados |
| Multiplexado por división de tiempo **estadístico** | **STDM** (*Statistical Time Division Multiplexing*) | El tiempo, asignado **según la demanda** de cada canal |

Además, la diapositiva incluye la **multiplexación por división de longitud de onda** (WDM), que es la equivalente a FDM en fibra óptica.

Los sistemas de multiplexado por división de tiempo pueden utilizar técnicas **plesiócronas** o **sincrónicas** (ver las jerarquías PDH y SDH más adelante).

<a id="c11-3"></a>
## 3. Multiplexación por división de frecuencia FDM

- El **ancho de banda total** del canal ($\Delta f$) se divide en **subcanales** (Subcanal 1, 2, ..., N), cada uno con su propio ancho de banda.
- Entre un subcanal y otro se deja una **banda de protección** (banda de guarda), para que las señales vecinas no se interfieran.
- Cada señal se **modula** sobre una portadora de frecuencia distinta (ver [Clase 10](#clase-10)) y las N señales se transmiten **al mismo tiempo**, ocupando cada una su porción del espectro.

$$\Delta f \ge \sum_{i=1}^{N} \Delta f_i + \text{bandas de protección}$$

- Es la técnica clásica de la radiodifusión y de la telefonía analógica.
- Se aplica a señales **analógicas**.

<a id="c11-4"></a>
## 4. Jerarquía analógica de FDM

En telefonía analógica, cada canal de voz ocupa **4 kHz** (0-4, 4-8, 8-12, ..., 44-48 kHz). Los canales se agrupan por niveles, y cada nivel agrupa varios del nivel anterior:

| Grupo | Se forma con | Canales de voz | Ancho de banda | Banda ocupada |
|---|---|:-:|:-:|---|
| **Primario** | 12 canales de voz | 12 | 48 kHz | 60 - 108 kHz |
| **Secundario** | 5 grupos primarios | 60 | 240 kHz | 312 - 552 kHz |
| **Terciario** | 5 grupos secundarios | 300 | 1200 kHz | 312 - 1552 kHz |
| **Cuaternario** | 3 grupos terciarios | 900 | 3716 kHz | 312 - 4028 kHz |
| **Quinario** | 3 grupos cuaternarios | 2700 | 12 026 kHz | 312 - 12 338 kHz |

Nota: en la diapositiva, el grupo primario figura con la leyenda "1 (12 cm)", que parece un error de tipeo por "12 canales".

Con cada nivel se reutiliza la misma idea: la señal del nivel anterior se **traslada a otra banda de frecuencias** para que los grupos no se superpongan.

<a id="c11-5"></a>
## 5. Multiplexación por división de longitud de onda WDM

Es el equivalente de la FDM para la **fibra óptica**. Cada canal de datos se transmite por la misma fibra con una **longitud de onda distinta** ($\lambda_1, \lambda_2, \lambda_3, \dots, \lambda_n$), que equivale a decir una frecuencia distinta, ya que $f = c/\lambda$.

**Esquema de la clase**

1. Cada señal de entrada ingresa a un **transponder**, que adapta la señal a su longitud de onda asignada.
2. El **multiplexor** (Mux) combina todas las longitudes de onda en una sola fibra óptica.
3. En el extremo opuesto, el **demultiplexor** (Demux) separa las longitudes de onda.
4. Cada una pasa por su transponder y sale como el canal original.

**Variantes** (la diapositiva solo las nombra):

- **CWDM** (*Coarse WDM*): pocas longitudes de onda, muy separadas entre sí. Equipos más económicos.
- **DWDM** (*Dense WDM*): muchas longitudes de onda muy próximas entre sí, que aprovechan mucho mejor la fibra.

Las definiciones de CWDM y DWDM de arriba son ampliación de la explicación habitual. Revisalas contra tu material.

Se aprovechan las ventanas de transmisión de la fibra vistas en la [Clase 8](#clase-8) (850, 1300 y 1550 nm), en especial la banda C de 1550 nm. Permite multiplicar la capacidad de un enlace sin tender más fibras.

<a id="c11-6"></a>
## 6. Multiplexación por división de tiempo TDM

En TDM cada canal utiliza **todo el ancho de banda** del medio, pero solo durante un **intervalo de tiempo** ($\Delta t$) asignado. Los canales se turnan, uno detrás de otro, de forma periódica.

**Ejemplo de funcionamiento** (según el esquema de la clase)

- Cinco equipos terminales de datos (ETD) A, B, C, D y E envían información a un multiplexor TDM.
- El multiplexor toma un dato de cada uno y arma una **trama** `a b c d e`.
- La trama viaja por el medio de comunicación y, en el extremo receptor, otro multiplexor TDM **distribuye** cada dato a su destinatario (A, B, C, D, E).

**Técnica de conmutación en el tiempo.** Cada señal $S_1(t), S_2(t), \dots$ pasa primero por un **filtro** y luego por un **conmutador**. Un conmutador en el transmisor y otro en el receptor giran **sincronizados**, de modo que el dato que entra por el canal $k$ sale por el canal $k$ del otro lado. Si los conmutadores se desincronizan, los datos llegan a destinos equivocados. Por eso la sincronización (ver [sección 15](#c11-15)) es clave en TDM.

**Características**

- Se aplica a señales **digitales** (o analógicas ya muestreadas, como en la modulación PAM / PCM de la [Clase 10](#clase-10)).
- La capacidad del canal debe cubrir la suma de las capacidades de entrada, más los bits de sincronismo y señalización: $C_c \ge \sum C_i$.
- Si un canal no tiene datos para enviar, su intervalo **se desperdicia** (esto motiva la STDM, [sección 14](#c11-14)).

<a id="c11-7"></a>
## 7. Entramado de bits y de caracteres

La forma en que se intercalan los datos de los canales dentro de la trama define dos tipos de entramado:

| Tipo | Qué se intercala | Orden de transmisión (4 canales A, B, C, D) |
|---|---|---|
| **Entramado de bits** | Un **bit** de cada canal | A1, B1, C1, D1, A2, B2, C2, D2, ... |
| **Entramado de caracteres** | Un **carácter** (palabra de 8 bits) de cada canal | A1 A2 ... A8, B1 B2 ... B8, C1 ... C8, D1 ... D8, ... |

- En el **entramado de bits** el multiplexor necesita poco almacenamiento, porque no espera a completar un carácter. En PDH, entre los niveles superiores a E1, la multiplexación se produce bit a bit (ver [sección 9](#c11-9)).
- En el **entramado de caracteres** se agrupan los bits de cada carácter, de modo que el receptor entrega caracteres completos a cada destino.
- En ambos casos la numeración indica el orden de los dígitos: el "1.er bit transmitido" es el primero que sale hacia la línea.

<a id="c11-8"></a>
## 8. Esquema básico de multiplexación digital

La multiplexación digital se organiza en **niveles u órdenes** conectados en cascada:

- Los multiplexores de **orden 1** reciben los canales de abonado (tributarios) y entregan una señal de mayor velocidad.
- Esa señal se convierte en **una entrada** del multiplexor de **orden 2**, que a su vez reúne varias entradas en una señal de velocidad aún mayor.
- Se repite el proceso en los órdenes 3, ..., $n$, hasta llegar al **medio** de transmisión.
- En el extremo opuesto, se hace el camino inverso con multiplexores que separan cada nivel, hasta recuperar los canales originales.

Cada orden multiplica la velocidad y reduce la cantidad de medios necesarios. Las jerarquías **PDH** (plesiócrona) y **SDH** (sincrónica) son dos implementaciones de este esquema.

<a id="c11-9"></a>
## 9. Jerarquía digital plesiócrona PDH

**PDH** (*Plesiochronous Digital Hierarchy*) es la jerarquía TDM clásica. **Plesiócrono** significa "casi sincrónico": cada **tributario** viene de una red con su **propio reloj**, y al llegar al multiplexor TDM los relojes deben **sincronizarse** (de ahí los bits de justificación de la [sección 11](#c11-11)).

- En PDH las señales son **eléctricas** y los medios físicos son **cables coaxiales** y **enlaces de radio**.
- La multiplexación entre niveles se produce **bit a bit**.
- Se parte de un canal de **64 kbps** (E0), que sale de digitalizar la voz con PCM: 8000 muestras/s × 8 bits (ver [Clase 10](#clase-10)).

**Jerarquía europea (E)**

| Orden | Nombre | Velocidad | Se forma con | Bits por trama | Duración de la trama | N.° de canales |
|:-:|:-:|:-:|---|:-:|:-:|:-:|
| 0 | E0 | 64 kbps | Un canal de voz | | | 1 |
| 1 | E1 | 2,048 Mbps | 32 E0 | 256 | 125,00 µs | 30 |
| 2 | E2 | 8,448 Mbps | 4 E1 (o 128 E0) | 848 | 100,38 µs | 120 |
| 3 | E3 | 34,368 Mbps | 4 E2 (o 16 E1) | 1536 | 44,69 µs | 480 |
| 4 | E4 | 139,264 Mbps | 4 E3 (o 64 E1) | 2904 | 20,85 µs | 1920 |
| 5 | E5 | 564,992 Mbps | 4 E4 | 2688 | 4,70 µs | 7680 |

- En E1, de los 32 intervalos, **30 son canales de voz**, y los otros 2 son de sincronismo y señalización (ver [sección 10](#c11-10)).
- La velocidad de cada nivel es **algo mayor que la suma de las entradas**. Por ejemplo, $4 \times 2{,}048 = 8{,}192$ Mbps, pero E2 trabaja a 8,448 Mbps. La diferencia se usa para alineamiento de trama, control y justificación.
- Para E5, la trama de 2688 bits a 564,992 Mbps daría unos 4,76 µs, y la diapositiva indica 4,70 µs. Es una diferencia pequeña y no queda claro si es redondeo o error de la tabla.

**Otras jerarquías** (según el diagrama comparativo de la clase)

| Jerarquía | Zona | Velocidades |
|---|---|---|
| PDH (E) | Mundial | 2048, 8448, 34 368 y 139 264 kbps |
| T-Carrier | EE. UU. y Canadá | T1 1544, T1c 3152, T2 6312 y T3 44 736 kbps |
| J | Japón | J1 1544, J1c 3152, J2 6312, J3 32 064 y J4 97 728 kbps |

<a id="c11-10"></a>
## 10. Tramas E1 y T1

Ambas tramas duran **125 µs**, que es el período del muestreo de la voz (1/8000 s). En cada trama se transmite **una muestra de 8 bits por canal**.

| Característica | **E1** (Europa) | **T1** (EE. UU.) |
|---|---|---|
| Duración de la trama | 125 µs | 125 µs |
| Composición | 32 intervalos de 8 bits | 24 intervalos de 8 bits + 1 bit de entramado |
| Bits por trama | 256 | 193 |
| Velocidad | 2,048 Mb/s | 1,544 Mb/s |
| Canales de información | 30 | 24 |
| Velocidad de cada canal | 64 kb/s | 64 kb/s (56 kb/s en los canales con señalización) |

**Trama E1**

- **Intervalo 0**: alineamiento y sincronización de la trama.
- **Intervalo 16**: canal de señalización.
- **Intervalos 1 a 15 y 17 a 31**: canales de información, con 8 bits de datos (64 kb/s) cada uno.

**Trama T1**

- Un **bit de entramado** al comienzo de la trama.
- **Intervalos 1 a 5, 7 a 11 y 13 a 24**: canales de información, con 8 bits de datos (64 kb/s).
- En los **intervalos 6 y 12** (así figuran en la diapositiva) se usan solo **7 bits de información** (56 kb/s) y **1 bit de señalización**.

Verificación de las velocidades:

$$V_{E1} = \frac{256\ \text{bits}}{125\ \mu\text{s}} = 2{,}048\ \text{Mb/s} \qquad V_{T1} = \frac{24 \cdot 8 + 1}{125\ \mu\text{s}} = \frac{193\ \text{bits}}{125\ \mu\text{s}} = 1{,}544\ \text{Mb/s}$$

<a id="c11-11"></a>
## 11. Trama E2

Para multiplexar cuatro E1 en un E2 hay que resolver que **los relojes de los tributarios no son exactamente iguales**. La solución es la **justificación** (*bit stuffing*):

- Cada señal de 2 Mbps pasa por un **circuito de adaptación de bit rate**, que usa un **generador de reloj local**.
- Si una señal es **más rápida** que el reloj local, o **más lenta**, el circuito **inserta bits de justificación** ($J$) para igualar las velocidades.
- Luego, el **circuito de multiplexación** combina las señales ya adaptadas.

**Estructura de la trama E2:** 848 bits en 100,38 µs, divididos en **cuatro segmentos de 212 bits**.

| Segmento | Cabecera | Datos | Total |
|:-:|---|:-:|:-:|
| 1 | 10 bits (FAS) + 2 bits (A y N) | 200 | 212 |
| 2 | 4 bits de control ($C_1$ a $C_4$) | 208 | 212 |
| 3 | 4 bits de control ($C_1$ a $C_4$) | 208 | 212 |
| 4 | 4 bits de control ($C_1$ a $C_4$) + 4 bits de justificación ($S_1$ a $S_4$) | 204 | 212 |

- **FAS**: palabra de alineamiento de trama. En la diapositiva se muestra como `1111010000` seguida de los bits **A** y **N**.
- **$C_1$ a $C_4$**: bits de control, que le indican al receptor si hubo justificación.
- **$S_1$ a $S_4$**: bits de justificación, que son los lugares donde se pueden insertar los bits de relleno.
- Los significados de **A** y **N** no se detallan en la diapositiva (habitualmente son un bit de alarma y un bit de uso nacional). Revisalo con tu material.

<a id="c11-12"></a>
## 12. Jerarquía digital sincrónica SDH

**SDH** (*Synchronous Digital Hierarchy*) resuelve las limitaciones de PDH: toda la red trabaja **sincronizada con un reloj común**, por lo que ya no hace falta justificar bit a bit. Se transporta sobre **fibra óptica**.

**Armado de la jerarquía** (según el diagrama de la clase)

1. Los tributarios **PDH** (E1, E3, ...) se colocan en **contenedores virtuales** y forman tramas **STM-1** de 155,52 Mbps.
2. Un **multiplexor 4:1** combina cuatro STM-1 en una **STM-4** de 622,08 Mbps.
3. Otro multiplexor 4:1 combina cuatro STM-4 en una **STM-16** de 2488,32 Mbps.
4. La señal pasa por un **codificador** (*scrambler*) y por un **conversor electro-óptico**, y sale hacia la fibra (en el esquema, como OC-48c).

**Niveles de la jerarquía** ($N = 1, 4, 16, 64, 256$):

| Denominación | Velocidad exacta | N | Número de canales | Velocidad simplificada |
|---|:-:|:-:|:-:|:-:|
| STM-1 | 155,520 Mbps | 1 | 1890 | 155 Mbps |
| STM-4 | 622,080 Mbps | 4 | 7560 | 620 Mbps |
| STM-16 | 2488,320 Mbps | 16 | 30 240 | 2,5 Gbps |
| STM-64 | 9953,280 Mbps | 64 | 120 960 | 10 Gbps |
| STM-256 | 39 813,120 Mbps | 256 | 483 840 | 40 Gbps |

Cada nivel es $N$ veces la velocidad de STM-1:

$$V_{STM\text{-}N} = N \cdot 155{,}520\ \text{Mbps}$$

Nota: en la diapositiva, la columna N de STM-16 se lee como "26". Por la velocidad y la cantidad de canales (16 × 1890 = 30 240) debe ser **16**.

**Contenedores virtuales** (según la diapositiva)

| N.° | Contenedor | Velocidad de la multiplexación PDH |
|:-:|:-:|:-:|
| 1 | VC-11 | 1,544 Mbps |
| 2 | VC-12 | 2,048 Mbps |
| 3 | VC-2 | 6,048 Mbps |
| 4 | VC-3 | 34,368 y 44,736 Mbps |
| 5 | VC-4 | 139,264 Mbps |

**Topología en anillo.** Los **ADM** (*Add-Drop Multiplexer*, multiplexores de inserción y extracción) forman un **anillo** de fibra, con una **fibra de trabajo** y una **fibra de protección**. Si se corta una fibra, el tráfico pasa por la de protección, y la red sigue funcionando. Los tributarios PDH entran y salen del anillo por los ADM.

<a id="c11-13"></a>
## 13. Trama STM-N

Cada trama STM-N se divide en dos partes:

- **SOH** (*Section Overhead*, sección de encabezado): información de control, alineamiento, supervisión y gestión.
- **Payload**: carga total de la trama, que transporta los datos de los usuarios.

**Estructura:** 9 filas × $270 \times N$ bytes.

| Zona | Tamaño por fila |
|---|:-:|
| Sección de encabezado (SOH) | $9 \times N$ bytes |
| Columna adicional (junto al encabezado) | $1 \times N$ bytes |
| Capacidad neta de carga | $260 \times N$ bytes |
| **Carga total de la trama** (payload) | $261 \times N$ bytes |
| **Trama completa** | $270 \times N$ bytes |

Verificación para STM-1 (cálculo propio, que usa la trama de 125 µs):

$$V = \frac{9 \cdot 270 \cdot 8\ \text{bits}}{125\ \mu\text{s}} = \frac{19\,440\ \text{bits}}{125\ \mu\text{s}} = 155{,}520\ \text{Mbps}$$

<a id="c11-14"></a>
## 14. Multiplexación por división de tiempo estadística STDM

En la TDM común, a cada canal le corresponde un intervalo fijo en cada trama, haya o no datos para enviar. Los intervalos vacíos son **tiempos muertos**, y desperdician capacidad.

En la **STDM** el multiplexor estadístico **asigna los intervalos según la demanda**: solo se transmiten los canales que tienen datos en ese momento.

- En el esquema de la clase hay cuatro canales (A, B, C, D) con intervalos vacíos (tiempos muertos).
- Si fuera TDM común, esos intervalos viajarían vacíos. Con STDM, el multiplexor los salta y arma la secuencia de salida solo con datos (en la figura: C1, D1, A1, B1, D2, C2, A2, B2).
- Como el orden ya no es fijo, **cada bloque debe ir identificado con su canal**, para que el multiplexor del otro extremo sepa a qué destino entregarlo (en la figura, cada bloque lleva su rótulo).

**Ventajas y costos**

- Se aprovecha mejor el canal: la capacidad del canal común puede ser **menor que la suma** de las capacidades de entrada. Es el caso del **concentrador** ($C_c \le \sum C_i$) de la [sección 1](#c11-1).
- Si coinciden muchos canales con datos a la vez, el multiplexor necesita **memoria** para encolar y puede introducir **demoras**.
- Los bloques llevan información extra de identificación, que aumenta un poco la carga.

<a id="c11-15"></a>
## 15. Sincronización y reloj

**Sincronizar** es hacer que dos o más hechos, fenómenos, movimientos o mecanismos estén en **perfecta correspondencia temporal**, es decir, que ocurran en un momento predefinido de tiempo o lugar.

En una red de comunicaciones, los **elementos de la red** tienen cada uno un **reloj local**, y todos deben seguir a un **reloj patrón** (de referencia). Sin sincronización, los multiplexores TDM pierden la alineación de las tramas y se producen errores (en PDH, los relojes casi iguales se compensan con justificación, y en SDH se sincroniza toda la red).

**Alternativas de sincronización**

| Tipo | Qué se logra |
|---|---|
| **Sincronización de frecuencia** | Los relojes tienen la **misma frecuencia** ($f_A = f_B$), pero sus pulsos no tienen por qué coincidir |
| **Sincronización de fase** | Además de tener la misma frecuencia, los **pulsos coinciden** en el tiempo |
| **Sincronización de tiempo** | Además de frecuencia y fase, los relojes marcan la **misma hora** (en la figura, ambos indican 01:00:00 y 01:00:10 en los mismos instantes) |

Cada tipo incluye al anterior, y el de tiempo es el más exigente.

<a id="c11-16"></a>
## 16. Tipos de reloj y modos de operación

**Reloj**: en redes, es un **generador de frecuencias** que se utiliza para sincronizar la red.

**Tipos de reloj**

- **Maestro** (*master*): entrega la referencia de tiempo.
- **Esclavo** (*slave*): toma la referencia del maestro y ajusta su reloj local.

**Modos de operación** (la diapositiva solo los nombra; las definiciones son ampliación)

- **Enganchado** (*locked*): el reloj está sincronizado con una referencia externa.
- **Retención** (*holdover*): se perdió la referencia, y el reloj mantiene la última frecuencia conocida.
- **Libre** (*free-run*): el reloj trabaja solo, con su oscilador interno.

**Elementos del esquema de la clase**

- **PTP**: protocolo de precisión de tiempo (ver [sección 17](#c11-17)), con interfaces *Slave* y *Master*.
- **SyncE**: Ethernet sincrónico, que distribuye la frecuencia por la capa física.
- **EEC**: reloj del equipo, un oscilador que se engancha a la referencia.
- **1pps**: salida de un pulso por segundo, para sincronización de tiempo.

<a id="c11-17"></a>
## 17. Protocolo de precisión de tiempo PTP

Con PTP, un reloj **esclavo** calcula su desfase respecto de un **maestro** intercambiando mensajes con **marcas de tiempo** (*timestamps*).

**Secuencia de mensajes**

1. El maestro envía **SYNC** en el instante $t_1$ (de su reloj). El esclavo lo recibe en $t_2$ (de su reloj).
2. El maestro envía **Follow_Up**, que contiene el valor de $t_1$.
3. El esclavo envía **Delay_Req** en $t_3$ (de su reloj), y el maestro lo recibe en $t_4$ (de su reloj).
4. El maestro responde con **Delay_Resp**, que contiene $t_4$.

Con eso el esclavo conoce $t_1, t_2, t_3, t_4$.

**Planteo.** Sea $\text{Delay}$ el retardo de propagación (se asume igual en ambos sentidos) y $\text{Offset} = T_S - T_M$ el desfase del esclavo respecto del maestro:

$$t_2 = t_1 + \text{Offset} + \text{Delay} \quad \Rightarrow \quad t_2 - t_1 = \text{Offset} + \text{Delay}$$

$$t_4 = t_3 - \text{Offset} + \text{Delay} \quad \Rightarrow \quad t_4 - t_3 = \text{Delay} - \text{Offset}$$

Sumando y restando ambas ecuaciones:

$$\text{Delay} = \frac{(t_2 - t_1) + (t_4 - t_3)}{2}$$

$$\text{Offset} = \frac{(t_2 - t_1) - (t_4 - t_3)}{2}$$

Con el **Offset** el esclavo corrige su reloj.

<a id="c11-18"></a>
## 18. Ejemplo de cálculo con PTP

**Datos del ejemplo de la clase**

| Marca | Valor |
|:-:|:-:|
| $t_1$ (el maestro envía SYNC) | 100 s |
| $t_2$ (el esclavo recibe SYNC) | 82 s |
| $t_3$ (el esclavo envía Delay_Req) | 86 s |
| $t_4$ (el maestro recibe Delay_Req) | 108 s |

**Desfase (Offset)**

$$o = \frac{(t_2 - t_1) - (t_4 - t_3)}{2} = \frac{(82 - 100) - (108 - 86)}{2} = \frac{-18 - 22}{2} = \frac{-40}{2} = -20\ \text{s}$$

El resultado es negativo: el reloj del esclavo está **20 s atrasado** respecto del maestro. El esclavo ajusta su reloj sumándole 20 s.

**Retardo (Delay)** (cálculo propio, la diapositiva solo resuelve el desfase):

$$\text{Delay} = \frac{(82 - 100) + (108 - 86)}{2} = \frac{-18 + 22}{2} = 2\ \text{s}$$

Verificación: el SYNC sale a las 100 s del maestro y llega a las 82 s del esclavo, que equivalen a las 102 s del maestro. Entonces tardó 2 s, que coincide con el Delay.