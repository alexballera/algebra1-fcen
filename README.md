# Repositorio de Álgebra I (FCEyN - UBA)

Este repositorio centraliza material de estudio, apuntes, guías de trabajos prácticos y soluciones para la materia **Álgebra I** de la Facultad de Ciencias Exactas y Naturales (FCEyN) de la Universidad de Buenos Aires (UBA).

El objetivo es proporcionar un acceso organizado y colaborativo a todos los recursos necesarios para cursar y aprobar la materia.

## Estructura del Repositorio

El contenido está organizado en los siguientes directorios principales:

### 📁 `sesiones/`

Es el directorio principal del material de estudio, dividido en capítulos que corresponden a cada unidad temática del programa oficial. La estructura es la siguiente:

-   **Capítulo 1:** Conjuntos, Relaciones y Funciones.
-   **Capítulo 2:** Números Naturales e Inducción.
-   **Capítulo 3:** Combinatoria.
-   **Capítulo 4:** Números Enteros (Divisibilidad, Primos, MCD).
-   **Capítulo 5:** Números Enteros (Congruencias y Ecuaciones Diofánticas).
-   **Capítulo 6:** Números Complejos.
-   **Capítulo 7:** Polinomios.

Cada capítulo contiene subdirectorios para el material teórico, las guías de trabajos prácticos, resúmenes y cuestionarios interactivos.

### 📁 `bibliografia/`

Contiene material de referencia general, como apuntes teóricos de distintas cátedras, libros recomendados y notas complementarias que sirven de apoyo durante toda la cursada.

### 📁 `hp-prime/`

Dedicado a la calculadora **HP Prime**, una herramienta clave en la materia. Incluye manuales, guías de uso rápido y ejemplos prácticos para resolver problemas específicos de álgebra.

## Cuestionarios Interactivos

Para reforzar el aprendizaje, cada unidad incluye **cuestionarios interactivos** desarrollados con HTML, CSS y JavaScript.

### Características

-   **Interfaz moderna y responsive**: Diseño limpio con Tailwind CSS.
-   **Múltiples versiones**: Genera hasta 10 variantes de cada examen con preguntas aleatorias.
-   **Retroalimentación inmediata**: Explicaciones detalladas para cada respuesta.
-   **Sistema de puntaje**: Seguimiento del progreso en tiempo real.

## Generación de Resúmenes en PDF

Los resúmenes de cada unidad se gestionan a través de archivos LaTeX para asegurar un formato de alta calidad.

### Instrucciones de Generación

1.  **Prerrequisitos:** Tener una distribución de LaTeX instalada.
2.  **Generar el PDF:** Utiliza el comando `pdflatex` desde la raíz del proyecto. Por ejemplo, para la Unidad 1:
    ```bash
    pdflatex -output-directory=sesiones/capitulo1/resumen/ sesiones/capitulo1/resumen/resumen-unidad1.tex
    ```

## Contribuciones

¡Las contribuciones son bienvenidas! Si tienes material adicional, encuentras un error o quieres proponer una mejora, no dudes en abrir un **Pull Request**.

## Licencia

Este proyecto se distribuye bajo la licencia MIT. Puedes ver los detalles en el archivo [LICENSE](LICENSE).