# Dimensionado del sistema
## 1 Generalidades
* 1.1 El objeto de este apartado es evaluar el dimensionado del generador fotovoltaico llevado a cabo por el instalador, con independencia de los métodos que el instalador utilice para esta tarea.
* 1.2 Para ello se le pedirá que indique la eficiencia energética esperada para la instalación.





## 2 Definiciones

* 2.1 Ángulo de inclinación $\beta$ .
  Ángulo que forma la superficie de los módulos con el plano horizontal (figura 1). Su valor es
  0° para módulos horizontales y 90° para verticales.
* 2.2 Ángulo de azimut $\alpha$ .
  Ángulo entre la proyección sobre el plano horizontal de la normal a la superficie del módulo y
  el meridiano del lugar (figura 2). Valores típicos son 0° para módulos orientados al sur, –90°
  para módulos orientados al este y +90° para módulos orientados al oeste.

![image-20220114164302648](Dimensionado%20del%20sistema.assets/image-20220114164302648.png)



* 2.3 $G_{dm}(0)$.
  Valor medio mensual o anual de la irradiación diaria sobre superficie horizontal en $kWh/(m^2\cdot día)$.

* 2.4 $G_{dm}(\alpha_{opt},\beta_{opt})$.
  Valor medio mensual o anual de la irradiación diaria sobre el plano del generador orientado de
  forma óptima $(\alpha_{opt}\beta_{opt})$, en $kWh/(m^2\cdot día)$. Se considera orientación óptima aquella que hace que
  la energía colectada sea máxima en un período.

* 2.5 $G_{dm}(\alpha,\beta)$.
  Valor medio mensual de la irradiación diaria sobre el plano del generador en $kWh/(m^2\cdot día)$ y
  en el que se hayan descontado las pérdidas por sombreado.

* 2.6 Factor de irradiación (FI).
  Porcentaje de radiación incidente para un generador de orientación e inclinación $(\alpha,\beta)$ respecto
  a la correspondiente para una orientación e inclinación óptimas $(\alpha=0,\beta_{opt})$ . Las pérdidas de
  radiación respecto a la orientación e inclinación óptimas vienen dadas por (1 – FI).

* 2.7 Factor de sombreado (FS).
  Porcentaje de radiación incidente sobre el generador respecto al caso de ausencia total de
  sombras. Las pérdidas por sombreado vienen dadas por (1 – FS).

* 2.8 Rendimiento energético de la instalación o “performance ratio”, PR.
  Eficiencia de la instalación en condiciones reales de trabajo para el período de diseño, de
  acuerdo con la ecuación:

  

  $PR=\frac{E_D \cdot G_{CEM}}{G_{dm}(\alpha, \beta) \cdot P_{mp}}$

  * $G_{CEM}= 1 kW/m^2$
  * $P_{mp}$ : Potencia pico del generador (kWp)
  * $E_D$ : Consumo expresado en kWh/día.

  

  Este factor considera las pérdidas en la eficiencia energética debido a:

  * La temperatura.
  * El cableado.
  * Las pérdidas por dispersión de parámetros y suciedad.
  * Las pérdidas por errores en el seguimiento del punto de máxima potencia.
  * La eficiencia energética, 0 rb , de otros elementos en operación como el regulador,batería, etc.
  * La eficiencia energética del inversor, 0 inv .
  * Otros.
    

Valores típicos son, en sistemas con inversor, $PR\approx0,7$ y, con inversor y batería, $PR\approx0,6$. A
efectos de cálculo y por simplicidad, se utilizarán en sistemas con inversor PR = 0,7 y con
inversor y batería PR = 0,6. Si se utilizase otro valor de PR, deberá justificarse el valor elegido
desglosando los diferentes factores de pérdidas utilizados para su estimación.

En caso de acoplo directo de cargas al generador (por ejemplo, una bomba), se hará un cálculo
justificativo de las pérdidas por desacoplo del punto de máxima potencia.



## 3 Procedimiento

### 3.1 Período de diseño

Se establecerá un período de diseño para calcular el dimensionado del generador en función de
las necesidades de consumo y la radiación. Se indicará cuál es el período para el que se realiza
el diseño y los motivos de la elección. Algunos ejemplos son:

* – En escenarios de consumo constante a lo largo del año, el criterio de “mes peor”
  corresponde con el de menor radiación.
* – En instalaciones de bombeo, dependiendo de la localidad y disponibilidad de agua, el
  “mes peor” corresponde a veces con el verano.
* – Para maximizar la producción anual, el período de diseño es todo el año.

### 3.2 Orientación e inclinación óptimas. Pérdidas por orientación e inclinación

Se determinará la orientación e inclinación óptimas$(\alpha=0,\beta_{opt})$ para el período de diseño
elegido. En la tabla III se presentan períodos de diseño habituales y la correspondiente
inclinación ( $\beta$ ) del generador que hace que la colección de energía sea máxima.

![image-20220114171248849](Dimensionado%20del%20sistema.assets/image-20220114171248849.png)



El diseñador buscará, en la medida de lo posible, orientar el generador de forma que la energía
captada sea máxima en el período de diseño ( " = 0°, $ opt ). Sin embargo, no será siempre posible
orientar e inclinar el generador de forma óptima, ya que pueden influir otros factores como son
la acumulación de suciedad en los módulos, la resistencia al viento, las sombras, etc. Para
calcular el factor de irradiación para la orientación e inclinación elegidas se utilizará la expresión
aproximada:



$FI=1-[1.2\cdot10^{-4}(\beta-\beta_{opt})^2]+3.5\cdot10^{-5}\alpha^2 \rightarrow 15^o<\beta<90^o$

$FI=1-[1.2\cdot10^{-4}(\beta-\beta_{opt})^2] \rightarrow \beta\leq15^o$

[Nota: $\alpha,\beta$ se expresan en grados]





### 3.3 Irradiación sobre el generador

Deberán presentarse los siguientes datos:

* $G_{dm}(0)$

Obtenida a partir de alguna de las siguientes fuentes:

1. – Instituto Nacional de Meteorología
2. – Organismo autonómico oficial



* $G_{dm}(\alpha,\beta)$

Calculado a partir de la expresión:

$G_{dm}(\alpha,\beta)= G_{dm}(0)\cdot FI\cdot FS$
donde:

$K=\frac{G_{dm}(\alpha=0,\beta_{opt})}{G_{dm}(0)}$

Este parámetro puede obtenerse de la tabla III para el período de diseño elegido.





### 3.4 Dimensionado del generador

El dimensionado mínimo del generador, en primera instancia, se realizará de acuerdo con los
datos anteriores, según la expresión:

$ P_{mp}=\frac{E_D \cdot G_{CEM}}{G_{dm}(\alpha, \beta) \cdot PR}$



$G_{CEM} = 1 kW/m^2$
$E_D$ : Consumo expresado en kWh/día.

Para el cálculo, se utilizarán los valores de PR especificados en el punto 2.8 de este anexo.

### 3.5 Diseño del sistema

El instalador podrá elegir el tamaño del generador y del acumulador en función de las
necesidades de autonomía del sistema, de la probabilidad de pérdida de carga requerida y
cualquier otro factor que quiera considerar, respetando los límites estipulados en el PCT:

* – La potencia nominal del generador será, como máximo, un 20 % superior al valor
  P mp, min para el caso general (ver 4.2.4 de este PTC).
* – La autonomía mínima del sistema será de tres días.
* – Como caso general, la capacidad nominal de la batería no excederá en 25 veces la
  corriente de cortocircuito en CEM del generador fotovoltaico.



La autonomía del sistema se calculará mediante la expresión:



$A=\frac{C_{20}PD_{max}}{L_D}\eta_{inv} \eta_b$

Donde:

* A = Autonomía del sistema en días
* $C_{20}$ = Capacidad del acumulador en Ah (*)
* $PD_{max}$ = Profundidad de descarga máxima
* $\eta_{inv}$= Rendimiento energético del inversor
* $\eta_{rb}$ = Rendimiento energético del acumulador + regulador
* $L_D$ = Consumo diario medio de la carga en Ah





## Cálculo

![image-20220118012834130](Dimensionado%20del%20sistema.assets/image-20220118012834130.png)



Se buscan los valores optimos para el VAN y el Pyback en el entorno de las Potencia pico del generador obtenida



![image-20220118013316814](Dimensionado%20del%20sistema.assets/image-20220118013316814.png)

![image-20220118013346539](Dimensionado%20del%20sistema.assets/image-20220118013346539.png)





![image-20220115134605073](Dimensionado%20del%20sistema.assets/image-20220115134605073.png)



![image-20220115135659927](Dimensionado%20del%20sistema.assets/image-20220115135659927.png)









![image-20220114194908536](Dimensionado%20del%20sistema.assets/image-20220114194908536.png)









![image-20220114202428719](Dimensionado%20del%20sistema.assets/image-20220114202428719.png)









Ref.: 

* [IDAE PCT-A-REV - febrero 2009](https://www.idae.es/sites/default/files/documentos_5654_FV_Pliego_aisladas_de_red_09_d5e0a327.pdf)