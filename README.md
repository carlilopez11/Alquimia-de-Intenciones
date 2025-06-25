# Alquimia-de-Intenciones

## Introducción
Este proyecto surge de la necesidad de conectar el uso consciente de productos naturales con herramientas tecnológicas accesibles. Muchas personas que utilizan elementos como sahumerios, velas de soja e infusiones para fines espirituales o emocionales, no siempre saben cómo combinarlos de forma coherente según una intención específica. 

*Alquimia de Intenciones* busca ofrecer una solución que permita, mediante prompts diseñados con técnicas de Fast Prompting, obtener recomendaciones automáticas y explicadas. Esta herramienta no solo mejora la experiencia del usuario final, sino que también resulta útil para emprendedores del rubro que desean ofrecer kits energéticos personalizados.


## Presentación del problema
En los espacios de venta y consumo de productos naturales con fines energéticos, tanto emprendedores como usuarios suelen enfrentarse a la dificultad de combinar adecuadamente sahumerios, infusiones y velas. Esta falta de orientación puede hacer que los productos pierdan efectividad simbólica, y genera incertidumbre al momento de armar un ritual o elegir un kit.

Esto representa una barrera tanto para la experiencia del cliente como para las posibilidades comerciales de quienes ofrecen estos productos. La problemática tiene impacto en lo emocional, en lo simbólico y en lo práctico. Por eso, desarrollar una herramienta que sugiera combinaciones intencionadas y explicadas puede representar un avance significativo.


## Propuesta de solución
La solución propuesta consiste en diseñar una herramienta que genere automáticamente combinaciones de productos naturales según la intención energética del usuario, a través de la inteligencia artificial.

Para lograrlo, se desarrolló un sistema basado en prompts que utiliza:

- **Modelos de texto a texto** (OpenAI ChatGPT `gpt-3.5-turbo`): para crear combinaciones compuestas por un sahumerio, una infusión y una vela de soja, explicando el motivo de cada elección.
- **Modelos de texto a imagen** (DALL·E): para generar visualizaciones estéticas que representen esas combinaciones como kits energéticos.

Los prompts fueron diseñados utilizando técnicas de Fast Prompting para maximizar la claridad y utilidad de las respuestas, reduciendo la cantidad de consultas necesarias. Todo el flujo fue implementado y documentado en un Jupyter Notebook como prueba de concepto (POC).


## Justificación de viabilidad
Este proyecto es viable técnica y operativamente por las siguientes razones:

- Utiliza herramientas accesibles y en su mayoría gratuitas: Jupyter Notebook, PlaygroundAI, NightCafe, y la API de OpenAI.
- Requiere únicamente una clave personal para acceder a los modelos de texto a texto, sin necesidad de una infraestructura externa compleja.
- El notebook puede ejecutarse localmente o desde Google Colab con mínimas configuraciones.
- El sistema es modular y escalable: se pueden añadir nuevas intenciones o productos sin alterar la estructura general del flujo.
- La lógica implementada es comprensible y replicable por otros emprendedores, haciendo del proyecto una solución práctica y potencialmente comercializable.

Además, la generación visual no requiere API paga si se utilizan plataformas alternativas, permitiendo mantener el costo del proyecto bajo control.


## Objetivos
- Diseñar una herramienta que sugiera combinaciones de productos naturales según una intención energética o emocional.
- Utilizar inteligencia artificial para automatizar recomendaciones explicadas y coherentes.
- Aplicar técnicas de Fast Prompting para mejorar la calidad de los resultados y reducir el número de consultas necesarias.
- Integrar generación de texto (ChatGPT) e imagen (DALL·E) para enriquecer la presentación de los kits sugeridos.
- Implementar el flujo en un Jupyter Notebook funcional, documentado y replicable.


## Metodología

El proyecto se desarrolló siguiendo una metodología iterativa y modular, centrada en la creación, prueba y ajuste de prompts diseñados para combinar productos naturales con fines energéticos o emocionales específicos.

### 🔹 Etapas del proceso:

1. **Definición del problema y contexto**
   - Se identificó la dificultad habitual de combinar sahumerios, infusiones y velas en función de intenciones como relajación, protección o limpieza energética.
   - Se relevó el catálogo real de productos disponibles para partir de ejemplos concretos.

2. **Diseño de prompts base**
   - Se redactaron prompts iniciales para cubrir intenciones frecuentes (relajación, protección, amor propio, etc.).
   - Cada prompt fue pensado para generar una combinación específica de tres productos (un sahumerio, una vela y una infusión) con explicación justificada.

3. **Aplicación de técnicas de Fast Prompting**
   - Se experimentó con diferentes formulaciones para mejorar claridad, estructura y precisión del output.
   - Se incorporaron ejemplos (few-shot prompting), instrucciones detalladas, y lenguaje contextualizado.

4. **Implementación en Jupyter Notebook**
   - Se organizaron los prompts y resultados dentro de una notebook interactiva, con celdas que permiten modificar la intención y ver el resultado dinámicamente.
   - Se simularon outputs de ChatGPT y se documentaron los resultados esperados.

5. **Visualización con IA**
   - Se seleccionaron algunas combinaciones generadas y se utilizaron como base para generar imágenes con DALL·E.
   - Las imágenes buscan representar visualmente los kits, aportando valor estético y comunicacional.

6. **Documentación y publicación**
   - Todo el proyecto fue documentado y subido a GitHub, incluyendo el archivo `README.md`, la notebook `combinaciones_IA.ipynb` y las imágenes asociadas.
   - Se eligió GitHub como plataforma por su formato accesible, versionado automático y cumplimiento con las pautas del curso.

### 🔹 Justificación de la metodología

Este enfoque permite un desarrollo ágil y realista, combinando pruebas prácticas con documentación clara. La separación por etapas facilita el escalado del proyecto (se pueden sumar más intenciones o productos), y la integración de texto e imagen brinda un resultado rico en contenido para usuarios reales o fines comerciales.


## Herramientas y tecnologías

| Herramienta                | Uso                                                                 | Justificación                                                                                          |
|----------------------------|----------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| **ChatGPT (texto a texto)**| Generación de combinaciones de productos según intención             | Permite obtener resultados personalizados en lenguaje natural. Ideal para generar rituales y recetas. |
| **DALL·E**                 | Generación de imágenes desde descripciones textuales                 | Visualiza los kits sugeridos. Agrega valor estético para redes sociales o catálogos.                 |
| **Jupyter Notebook**       | Desarrollo y documentación del proceso de prompting                  | Permite integrar texto, código e imágenes en un solo entorno interactivo.                            |
| **GitHub**                 | Publicación del proyecto y control de versiones                      | Facilita la entrega profesional y el acceso público al proyecto, como exige la consigna.              |

---

### Técnicas de Prompting utilizadas

#### 1. **Few-shot prompting**
- **Descripción**: Se incluyen uno o más ejemplos dentro del prompt para que el modelo entienda el formato esperado.
- **Ejemplo aplicado**:
  > “Por ejemplo: Para ‘relajación’ puede usarse lavanda y manzanilla. Ahora generá un combo para ‘protección energética’...”
- **Justificación**: Aumenta la precisión y coherencia de los resultados. Sirve como guía para el modelo.

#### 2. **Instrucciones claras y estructuradas**
- **Descripción**: El prompt especifica qué se espera (estructura de respuesta, número de elementos, tipo de productos, etc.).
- **Ejemplo aplicado**:
  > “Incluí un sahumerio, una infusión y una vela de soja. Explicá por qué elegís cada uno.”
- **Justificación**: Ayuda a obtener respuestas organizadas y completas, sin información irrelevante.

#### 3. **Contextualización por intención**
- **Descripción**: Se indica el propósito del combo para que la IA entienda mejor el sentido del pedido.
- **Ejemplo aplicado**:
  > “Generá un combo de productos para armonizar una habitación luego de una discusión fuerte.”
- **Justificación**: Mejora la adecuación de las sugerencias a necesidades emocionales o energéticas reales.

#### 4. **Iteración y refinamiento**
- **Descripción**: Se prueban diferentes formulaciones de prompt para evaluar cuál genera mejores resultados.
- **Justificación**: Optimiza el uso de tokens/consultas y permite encontrar la versión más efectiva del prompt para cada intención.


## Implementación
La implementación se encuentra en el archivo `https://github.com/carlilopez11/Alquimia-de-Intenciones/blob/80f6eedf3d04126f465ce7236e98e53ebdc9889d/Alquimia%20de%20Intenciones.ipynb`, donde se simulan consultas de usuario y se generan respuestas automáticas, junto a imágenes representativas.

