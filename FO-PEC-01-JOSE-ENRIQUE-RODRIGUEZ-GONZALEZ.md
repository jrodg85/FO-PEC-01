# Master Universitario de Ingeniería en Telecomunicaciones.
# 81.533 Redes de Fibra Óptica – PEC1.
# José Enrique Rodríguez González.

## Profesores de la asignatura.

Profesor responsable:
  - Dr. Pere Tuset <peretuset@uoc.edu>
Profesores colaboradores:
  - Dr. Salvatore Spadaro <sspadaro@uoc.edu>

---

## Presentación de la actividad.

La PEC1 consta de varios ejercicios acerca de las diferentes características de la fibra óptica. El objetivo es evaluar la capacidad de determinar parámetros de un sistema óptico (tasa de bits, ancho de banda, longitud de enlace óptico, etc.) que dependan de las características de las fibras ópticas utilizadas.

---

## Competencias de la PEC1.

Las competencias que se trabajan total o parcialmente en esta PEC son las siguientes:
1. Capacidad de análisis de componentes y sus specificaciones para sistemas de comunicaciones guiadas y no guiadas.
2. Capacidad para la selección de antenas, equipos y sistemas de transmisión, propagación de ondas guiadas y no guiadas, por medios electromagnéticos, de radiofrecuencia u ópticos y la correspondiente gestión del espacio radioeléctrico y asignación de frecuencias.

---

## Objetivos.

1. Conocer los principios físicos que rigen la transmisión a través de una fibra óptica.
2. Entender las limitaciones propias del canal de transmisión óptico.
3. Identificar los distintos tipos de fibra óptica.

---

## Recursos.

Para la realización de la PEC1 el material de estudio es el propio de la asignatura. Adicionalmente puede consultarse la bibliografía recomendada.

---

## Criterios de valoración.

Puntuación: Ejercicios 100% de la nota. Hay que justificar todo lo que se haga.

## Formato y fecha de entrega.

Fecha límite de entrega: 24 de octubre de 2023. Se debe entregar la PEC antes de las 24:00 horas de esta fecha a través del buzón “Entrega de actividades” de vuestra aula.

El nombre del documento deberá ser el siguiente:  <nombre_usuario_uoc>_PEC1.<extensión>. Por ejemplo, si vuestro nombre de usuario es “agarcia” y entregáis la PEC en formato .rtf, el nombre del archivo deberá ser: agarcia_PEC1.rtf.

Los formatos permitidos son .rtf, .doc y .pdf.

Todas las figuras que haya en el documento se tienen que insertar en el texto. No hay que entregar ficheros aparte.

No se aceptan entregas que sean copias escaneadas de ejercicios resueltos a mano.

---

## Índice.

- [Enunciado del ejercicio 1.](#enunciado-del-ejercicio-1)
- [Respuesta del ejercicio 1.](#respuesta-del-ejercicio-1)
- [Enunciado del ejercicio 2.](#enunciado-del-ejercicio-2)
- [Respuesta del ejercicio 2.](#respuesta-del-ejercicio-2)
- [Enunciado del ejercicio 3.](#enunciado-del-ejercicio-3)
- [Respuesta del ejercicio 3.](#respuesta-del-ejercicio-3)
- [Enunciado del ejercicio 4.](#enunciado-del-ejercicio-4)
- [Respuesta del ejercicio 4.](#respuesta-del-ejercicio-4)
- [Enunciado del ejercicio 5.](#enunciado-del-ejercicio-5)
- [Respuesta del ejercicio 5.](#respuesta-del-ejercicio-5)

---

## Enunciado del ejercicio 1.

Se considere un sistema por fibra óptica compuesto por un transmisor óptico, una fibra y un receptor óptico. Se asuma que la potencia óptica emitida por el transmisor es de 1 mW y que la longitud del tramo de fibra es L = 25 Km.

Se plantea utilizar la segunda o la tercera ventana para la transmisión.

Determinar la potencia óptica recibida por el receptor en ambos casos.

*Nota: se utilicen los datos del coeficiente de atenuación de alguna fibra óptica comercial.*

[Volver al Índice](#índice)

---

<br>

## Respuesta del ejercicio 1.


Para resolver el presente ejercicio, calcularemos la atenuacion de la señal en la fibra optica, cuya fórmula es 

$ P_{rx} = P_{tx} \times 10^{-\alpha L/10} $

Donde cada uno de los valores son:

- $ P_{rx} $ es la  poténcia óptica recibida.

- $ P_{tx} $ es la potencia óptica transmitida.

- $\alpha$  es el coeficiente de atenuación.

- $L$ es la longitud de la fibra.

Dadas las ventanas y sus coeficientes típicos, podemos encontrar el lo siguiente en la página 19 del ***Módulo 1. Redes de fibra óptica (PID_00238491)*** lo siguiente:

*Hay tres ventanas donde la atenuación presenta valores mínimos:*
*- En la primera ventana, entre 800 y 900 nm la atenuación es de unos dB/km. Esta ventana fue la primera que se utilizó en las comunicaciones ópticas, en la década de los 70 y 80, debido al bajo coste de los transmisores y receptores para esta ventana.*
*- En segunda ventana, alrededor de los 1.310 nm, los valores de atenuación bajan a menos de 1 dB/km hasta llegar a 0,2-0,3 dB/km. Esta ventana empezó a ser utilizada a mediados de la década de los 80.*
*- La tercera ventana, entre 1.510 nm y 1.600 nm, se caracteriza por el valor de atenuación mínima. A partir de finales de la década de los 90 se empezó a utilizar esta ventana, debido al elevado coste de los transmisores y los receptores.*

Por otro lado en el siguiente enlace de [Wikipedia](https://es.wikipedia.org/wiki/OTDR), podemos encontrar lo siguiente:

***Medición de longitud óptica***

*A efecto de realizar una medida de precisión, deberá considerarse el índice de refracción de las fibras ópticas instaladas. Dicha medida deberá ejecutarse mediante OTDR, debidamente calibrado y certificado por el fabricante o distribuidor autorizado y los valores resultantes de la medida no deberán superar, para el caso de empalmes por fusión, 0,15 dB de promedio por empalme medido bidireccionalmente, y 0,5 dB por par de conector instalado en el trayecto de la fibra a probar.* ***El valor teórico contemplado para pérdida de potencia por km. es de 0,35 dB para el caso de fibras medidas en segunda ventana (1310 nm) y de 0,25 dB para el caso de fibras medidas en tercera ventana (1550 nm).***

*La medición deberá efectuarse con la mejor resolución posible, es decir, la distancia y el ancho de pulso deberán ser los menores posibles.*

Por todo lo anteriormente expuesto en las fuentes de consulta procederé a lo indicado en wikipedia ya que presenta unos valores dentreo del rango expuesto en los apuntes.

En el caso que nos acompaña, la segunda ventana, nos indica que el la longitud de onda de la segunda ventana es de 1310nm, usaremos un $\alpha$ de 0.35 dB/km. Aplicando la fórmula expuesta, tenemos el siguiente razonamiento:

$ P_{rx} = 1 \times 10^{-0.35\times 25 /10} $ mW

**<span style="color:blue"> P<sub>rx</sub> = 0,133352143  mW</span>**


En el caso que nos acompaña, la tercera ventana, nos indica que el la longitud de onda de la segunda ventana es de 1550nm, usaremos un $\alpha$ de 0.25 dB/km.

$ P_{rx} = 1 \times 10^{-0.22\times 25 /10} $ mW

**<span style="color:blue"> P<sub>rx</sub> = 0,281838293  mW</span>**



[Volver al Índice](#índice)

---

<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>

## Enunciado del ejercicio 2.

Se diseña un sistema de transmisión basado en fibra óptica para poder dar soporte a una tasa de bits de hasta B = 200 Mpbs. Se compone de un transmisor óptico tipo láser que emite
una potencia óptica PTX = -1 dBm en tercera ventana (λ<sub>p</sub> = 1550 nm) y con anchura espectral de emisión Δλ = 1 nm, una fibra óptica de tipo G.652D y un receptor óptico.

En tercera ventana la fibra presenta un coeficiente de dispersión intramodal D = 17 ps/(Km·nm) y coeficiente de atenuación de 0,25 dB/Km.

Determinar:
  1. La máxima distancia a la que puede transmitirse por dispersión.
  2. La potencia óptica recibida por el receptor asumiendo que la longitud de la fibra corresponde al valor máximo calculado en el apartado anterior.
  3. Si la sensibilidad del receptor fuese de -24 dBm, ¿podría realizarse el sistema? ¿En el caso de que no, como podría entonces realizarse el sistema?

[Volver al Índice](#índice)

---

## Respuesta del ejercicio 2.











[Volver al Índice](#índice)

---

## Enunciado del ejercicio 3.

Un sistema de transmisión por fibra óptica se compone de:
  1. Un transmisor óptico que emite una potencia de -4 dBm en λp = 1530 nm y presenta anchura espectral de emisión de 2nm y un receptor óptico. Para la fibra óptica, cuya longitud es de L = 125 Km, se contemplan dos opciones: 
    1. fibra de tipo G.652 con coeficiente de dispersión intradamodal D = 17 ps/(Km·λnm);
    2. fibra de tipo G.655 con coeficiente de dispersión intramodal D = 6 ps/(Kmnm). Se determina que la potencia óptica recibida por el receptor tiene que ser de por lo menos -26 dBm y se pretende que el sistema pueda dar soporte a una tasa de transmisión de 200 Mpbs.

Determinar la opción de fibra óptica que permite implementar el sistema.

[Volver al Índice](#índice)

---

## Respuesta del ejercicio 3.











[Volver al Índice](#índice)

---

## Enunciado del ejercicio 4.

Un transmisor óptico de tipo láser emite en tercera ventana (λ<sub>p</sub>= 1510 nm). La potencia óptica emitida por el láser (-5 dBm) se acopla con una fibra óptica de longitud L = 100 Km. Para la fibra se consideran dos opciones:
  1. Una fibra A con diámetro de 2a = 10 μm, índice de refracción del núcleo n1 = 1,45 y apertura numérica NA = 0,06. Su coeficiente de dispersión intramodal (D) es de 3 ps/(Km·nm) y el coeficiente de atenuación es de α = 0,22 dB/Km.
  2. Una fibra B con los mismos diámetro, índice de refracción del núcleo y apertura numérica que la fibra del apartado anterior. Su coeficiente de dispersión intramodal (D) es de 14 ps/(Km·nm) y el coeficiente de atenuación es de α = 0,24 dB/Km.

Deducir la máxima anchura espectral de emisión () del láser para permitir la transmisión con una tasa de bits de B = 100 Mbps.

*Nota: Se asuma que la sensibilidad del receptor es de -25 dBm.*

[Volver al Índice](#índice)

---

## Respuesta del ejercicio 4.













[Volver al Índice](#índice)

---

## Enunciado del ejercicio 5.

En un sistema de transmisión por fibra, se dispone de una fuente óptica sintonizable con
λ<sub>p</sub>=1,25 &#xb1; 0,5 μm y anchura espectral de emisión de 1 nm. La fibra óptica, de longitud L = 88 Km presenta un coeficiente de dispersión intramodal que puede expresarse como D = $\frac{λ}{c}$·$\frac{d^2λ}{dn^2}$ siendo $\frac{d^2λ}{dn^2}$ la derivada segunda de λ con respecto al índice de refracción que, en este caso, pude aproximarse con la expresión $\frac{d^2λ}{dn^2}$ = $\frac{0.01}{λ^2}$.

La fibra presenta también un diámetro del núcleo de 10 μm, índice de refracción del núcleo n1 = 1,45 y apertura numérica (NA) de 0,1.

Se pretende poder transmitir una tasa de bits hasta los 250 Mbps.

Determinar el rango de valores en que puede variar p para asegurar los requerimientos del sistema.

[Volver al Índice](#índice)

---

## Respuesta del ejercicio 5.











[Volver al Índice](#índice)

---