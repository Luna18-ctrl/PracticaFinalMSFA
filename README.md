[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=Luna18-ctrl/PracticaFinalMSFA)

# Proyecto: Sistema renal (modelo dinámico de filtración)

## Información del estudiante
Cardenas Manzo kenia [20210773];  L20210773@tijuana.tecnm.mx
Frausto Luna Carlos Daniel [C18210366]; LC18210366@tijuana.tecnm.mx
Morales Lozoya Jesus Javier [20210806]; L20210806@tijuana.tecnm.mx
Rendon Carrillo Erik Rasheed [20210818]; L20210818@tijuana.tecnm.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente
Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura

El modelizado de sistemas fisiológicos es una herramienta importante en Ingeniería Biomédica, permite comprender el funcionamiento del cuerpo humano, así como diseñar y evaluar terapias y dispositivos médicos; se define como el proceso de formular modelos matemáticos o computacionales que representan el comportamiento y la interacción de los sistemas biológicos y fisiológicos. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional; lo anterior al proporcionar al estudiante bases sólidas para modelizar sistemas y diseñar controladores para la solución de problemas en las áreas de atención médica y del sector industrial médico. La construcción de analogías entre circuitos eléctricos y sistemas fisiológicos para la formulación de modelos matemáticos y el diseño de controladores mediante la experimentación in silico brindan herramientas de gran aplicación en el quehacer profesional del Ingeniero Biomédico.

La asignatura de Modelado de Sistemas Fisiológicos forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Utiliza las propiedades de los circuitos RLC para describir la dinámica de sistemas fisiológicos, obtener modelos matemáticos y aplicar el control clásico, esto con el objetivo de integrar los principios de la Ingeniería de Control, la Electrónica Analógica y las Ciencias de la Computación con la Anatomía y Fisiología del cuerpo humano para proporcionar descripciones cuantitativas y cualitativas de sistemas fisiológicos complejos con el objetivo de modelizar, analizar, controlar, ilustrar y predecir su dinámica tanto en el corto como en el largo plazo.

## Objetivos

1. Calcular la función de transferencia.
2. Determinar el modelo de ecuaciones integro-diferenciales.
3. Calcular el error en estado estacionario y la estabilidad en lazo abierto.
4. Emular y simular la respuesta del circuito en Simulink
5. Sintonizar las ganancias de un controlador PID para eliminar el error entre la entrada y la salida del sistema  entre un individuo sano (control) y un paciente con alteraciones (hipertensión). 
6. Obtener la respuesta en lazo abierto y en lazo cerrado con el controlador PID en el cuaderno computacional de Matlab.

## Descripción detallada del sistema

El sistema renal regula el equilibrio de líquidos y electrolitos mediante la filtración de la sangre en el glomérulo y el transporte del filtrado a lo largo del túbulo renal. Este proceso puede representarse mediante un circuito eléctrico de segundo orden que captura la dinámica entre presión, flujo y almacenamiento de volumen dentro del riñón.

En este modelo:
1. La resistencia R representa la resistencia vascular renal y la resistencia al flujo tubular.
2. La capacitancia C representa la distensibilidad del glomérulo y los túbulos renales.
3. La inductancia L representa la inercia del flujo sanguíneo renal.
4. La señal de entrada Ve(t) representa la presión arterial pulsátil que impulsa la perfusión renal.
5. El flujo f(t) es el equivalente al flujo del filtrado glomerular.

Este sistema permite estudiar la dinámica de la presión glomerular, la Tasa de Filtración Glomerular (TFG) y la respuesta del nefrón ante variaciones rápidas de presión o resistencia vascular.

La hipertensión arterial es una condición crónica caracterizada por un aumento sostenido de la presión arterial sistémica. A nivel renal, produce:
1. Vasoconstricción de la arteriola aferente y eferente, aumentando la resistencia vascular.
2. Disminución de la distensibilidad glomerular, pues los capilares renales se vuelven más rígidos.
3. Aumento de la presión hidrostática glomerular, lo cual altera la Tasa de Filtración Glomerular.
4. Mayor inercia en la respuesta del flujo sanguíneo, especialmente en estadios avanzados por remodelación vascular.

Estas alteraciones afectan directamente los parámetros R, C y L del circuito.

Palabras clave: Sistema Renal; Circuito RLC; Modelo matematico; Controlador PID; Simulaciones numericas

## Lista de archivos incluidos en el repositorio
1. Cuaderno computacional de MATLAB [.mlx].
2. Modelo de Simulink [.slx].
3. Biorender 
4. Imagen con los parámetros del controlador.
5. Imágenes de las simulaciones [.pdf y .png].
6. Evidencia del análisis matemático: función de transferencia, modelo de ecuaciones integro-diferenciales, error en estado estacionario y estabilidad en lazo abierto.
7. Ensayo grafico.

## Referencias
[1] P. A. Valle, Syllabus para Modelado de Sistemas Fisiológicos, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

[2] M. C. Khoo, Physiological Control Systems Analysis Simulation, and Estimation, 2nd ed. Piscataway, New Jersey, USA: IEEE Press, 2018, Section 4, Page 93.

[3] P. B. Persson, “Physiological Regulation of Renal Blood Flow and Glomerular Filtration Rate by the Endothelium and Smooth Muscle”, Blood Purification, vol. 15, no. 4-6, pp. 219–227, 1997.

[4]  Sgouralis y A. T. Layton, “Mathematical Modeling of Renal Hemodynamics in Physiology and Pathophysiology”, Mathematical Biosciences, vol. 264, no. 1, pp. 8–20, 2015.
[4] T. Kind, T. J. Faes, J. W. Lankhaar, A. Vonk-Noordegraaf & M. Verhaegen, "Estimation of three-and four-element Windkessel parameters using subspace model identification", IEEE Transactions on Biomedical Engineering, vol. 57, issue 7, pp. 1531-1538, Jul 2010. https://doi.org/10.1109/TBME.2010.2041351
