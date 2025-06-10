# Alquimia-de-Intenciones

## Introducción
Este proyecto explora cómo aplicar la inteligencia artificial generativa para combinar productos naturales según intenciones energéticas específicas (limpieza, relajación, protección, etc.). La propuesta está pensada para personas o emprendimientos que trabajan con sahumerios, infusiones, velas de soja y otros elementos rituales.

## Presentación del problema
Tanto vendedores como usuarios finales de productos naturales no siempre saben cómo combinarlos entre sí para potenciar su efecto energético o emocional. Esto reduce el aprovechamiento real de los productos, y dificulta la venta cruzada o la creación de kits temáticos. Se requiere una solución creativa y accesible para guiar estas combinaciones.

## Propuesta de solución
Mediante prompts diseñados con técnicas de Fast Prompting, el proyecto genera recomendaciones automáticas que combinan sahumerios, velas e infusiones según una intención deseada. También se generan imágenes con IA para visualizar esas combinaciones.

## Justificación de viabilidad
El proyecto utiliza herramientas gratuitas como ChatGPT, Dall-E y Jupyter Notebook. No requiere infraestructura compleja ni inversión adicional. Se trabaja con un catálogo real de productos ya existente.

## Objetivos
- Crear prompts efectivos para combinar productos naturales con sentido energético.
- Experimentar con técnicas de Fast Prompting para mejorar resultados.
- Mostrar la prueba de concepto en un entorno ejecutable y documentado.

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

