[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=Luna18-ctrl/Practica2MSFA)

# Práctica: Sistema cardiovascular

## Información del estudiante
Frausto Luna Carlos Daniel [C18210366]; LC18210366@tijuana.tecnm.mx

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
4. Emular y simular la respuesta del circuito en Simulink/Simscape a la señal "Uniform Random Number" con la siguiente configuración: min = -0.2 V; max = 1 V; seed = 106; Sample time = 0.5.
5. Sintonizar las ganancias de un controlador PID para eliminar el error entre la entrada y la salida del sistema normotenso-hipotenso y normotenso-hipertenso.
6. Obtener la respuesta en lazo abierto y en lazo cerrado con el controlador PID en Spyder/Python con la función de transferencia.

## Descripción detallada del sistema

El modelo de Windkessel de cuatro elementos contiene dos elementos dinámicos. Por lo tanto, se necesitan dos estados para describir la dinámica. El vector de estados se conforma por las variables FL(t) denotando el flujo a través de la inercia arterial total, y la variable Pp(t) representando la presión sobre la distensibilidad arterial. Entonces, asumiendo Pa(t) como la presión arterial de entrada, y en consecuencia a Fa(t) como el flujo hacia la aorta o arteria pulmonar. Los parámetros son Z, C, R y L, que representan respectivamente la impedancia característica del lecho vascular pulmonar (aorta y arteria pulmonar), la distensibilidad aérea total, la resistencia periférica y la inertancia arterial. Este modelo tiene muchas ventajas importantes, por ejemplo:

1. Su sencillez, unos pocos elementos interconectados son suficientes para reproducir la dinámica principal del sistema cardiovascular.

2. Existe una clara analogía entre los elementos eléctricos y los componentes hidráulicos implicados en el efecto Windkessel. En consecuencia, se relacionan fácilmente con el significado hemodinámico y el acoplamiento ventrículo-arterial.

Palabras clave: Sistema cardiovascular; Circuito RLC; Modelo matematico; Controlador PI; Simulaciones numericas

## Lista de archivos incluidos en el repositorio
1. Cuaderno computacional de MATLAB [.mlx].
2. Modelo de Simulink [.slx].
3. Archivos de Spyder [.py].
4. Imagen con los parámetros del controlador.
5. Imágenes de las simulaciones [.pdf y .png].
6. Evidencia del análisis matemático: función de transferencia, modelo de ecuaciones integro-diferenciales, error en estado estacionario y estabilidad en lazo abierto.

## Referencias
[1] P. A. Valle, Syllabus para Modelado de Sistemas Fisiológicos, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

[2] M. C. Khoo, Physiological Control Systems Analysis Simulation, and Estimation, 2nd ed. Piscataway, New Jersey, USA: IEEE Press, 2018, Section 4, Page 93.

[3] N. S. Nise, Control Systems Engineering, 8th ed. Hoboken, New Jersey, USA: John Wiley & Sons, 2020.

[4] T. Kind, T. J. Faes, J. W. Lankhaar, A. Vonk-Noordegraaf & M. Verhaegen, "Estimation of three-and four-element Windkessel parameters using subspace model identification", IEEE Transactions on Biomedical Engineering, vol. 57, issue 7, pp. 1531-1538, Jul 2010. https://doi.org/10.1109/TBME.2010.2041351
