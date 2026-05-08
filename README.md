# Proyecto-Análisis---ACV

**Curso:** BE3006 · Análisis de Datos Biomédicos · UVG · Ciclo 1, 2026
**Equipo:** Oscar Antonio Ramírez Duarte (23062) · Paulina María Martínez Flores (23143) · Fátima Angie Nicolle Camposeco Hernández (23122)

**Pregunta clínica.** ¿Qué características cuantitativas de la lesión por accidente cerebrovascular (volumen, localización, lateralidad) pueden estimarse de manera reproducible a partir de imágenes médicas?

La caracterización cuantitativa de la lesión es un insumo clínico directo: el volumen y la ubicación de la lesión correlacionan con la severidad neurológica (NIHSS), el pronóstico funcional y, según la literatura revisada en Fase 1, son predictores indirectos de reingreso.

**Decisión que el modelo informa.** Soporte al neurólogo en la lectura inicial de un T1w post-ACV: el modelo NO decide diagnóstico ni tratamiento — entrega volumen estimado y lateralidad de la lesión para que el clínico priorice qué imagen revisar primero y contraste contra el cuadro clínico (NIHSS, déficit motor, lateralidad esperada). En la Fase 1 nuestra pregunta era reingreso a 30 días post-alta; pivoteamos a esta pregunta porque ATLAS no contiene desenlaces longitudinales de reingreso, pero sí permite responder una pregunta vecina relevante para el mismo *patient journey* del ACV.
 
**Dataset.** ATLAS R2.0 — *Anatomical Tracings of Lesions After Stroke* (NITRC, ~955 sujetos, ~9.7 GB de NIfTI). Liew et al. (2022), *Sci Data* 9:320. T1w preprocesado en MNI-152 + máscaras manuales de lesión, deidentificado, bajo Data Use Agreement. Cohorte multi-sitio con sesgo geográfico hacia EE.UU./Europa/Asia (sin sitios latinoamericanos).

