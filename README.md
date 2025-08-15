# Repositorio de Álgebra I (FCEyN - UBA)

Este repositorio centraliza material de estudio, apuntes, guías de trabajos prácticos y soluciones para la materia **Álgebra I** de la Facultad de Ciencias Exactas y Naturales (FCEyN) de la Universidad de Buenos Aires (UBA).

El objetivo es proporcionar un acceso organizado y colaborativo a todos los recursos necesarios para cursar y aprobar la materia.

## Estructura del Repositorio

El contenido está organizado en dos directorios principales:

### 📁 `bibliografia/`

Contiene material de referencia general, como apuntes teóricos de distintas cátedras, libros recomendados y notas complementarias que sirven de apoyo durante toda la cursada.

### 📁 `unidades/`

Este directorio está dividido en capítulos, cada uno correspondiendo a una unidad temática del programa oficial de la materia. La estructura es la siguiente:

-   **Capítulo 1:** Conjuntos, Relaciones y Funciones.
-   **Capítulo 2:** Números Naturales e Inducción.
-   **Capítulo 3:** Combinatoria.
-   **Capítulo 4:** Números Enteros (Divisibilidad, Primos, MCD).
-   **Capítulo 5:** Números Enteros (Congruencias y Ecuaciones Diofánticas).
-   **Capítulo 6:** Números Complejos.
-   **Capítulo 7:** Polinomios.

Cada capítulo está organizado en subdirectorios especializados para facilitar la navegación:

#### Estructura de cada Capítulo
```
capitulo<N>/
├── lecturas/           # Material teórico y apuntes
├── practica/           # Guías de trabajos prácticos y soluciones
├── resumen/            # Resúmenes LaTeX y archivos generados
└── plan-de-estudio-unidad<N>.md  # Plan de estudio específico
```

Dentro de cada capítulo, encontrarás material teórico organizado, guías de trabajos prácticos con sus soluciones, resúmenes en formato PDF/LaTeX y **cuestionarios interactivos** para evaluar tu comprensión.

## Cuestionarios Interactivos

Para reforzar el aprendizaje de cada unidad temática, se incluyen **cuestionarios interactivos** desarrollados con tecnologías web modernas (HTML, CSS, JavaScript).

### Características de los Cuestionarios

-   **Interfaz moderna y responsive**: Diseño limpio utilizando Tailwind CSS con tipografía Inter.
-   **Múltiples versiones**: Cada cuestionario genera hasta 10 variantes diferentes con preguntas mezcladas aleatoriamente.
-   **20 preguntas por examen**: Cada sesión incluye 20 preguntas de opción múltiple sobre el tema de la unidad.
-   **Retroalimentación inmediata**: Explicaciones detalladas para cada respuesta correcte e incorrecta.
-   **Sistema de puntaje**: Seguimiento del progreso durante el examen.
-   **Efectos visuales**: Animaciones suaves y efectos hover para una mejor experiencia de usuario.

### Convención de Nombres

Los archivos de cuestionario siguen el siguiente formato dentro del subdirectorio `lecturas/` de cada capítulo:

-   **Archivo HTML:** `lecturas/capitulo<N>-cuestionario.html`

Donde `<N>` es el número de la unidad correspondiente (ej: `lecturas/capitulo1-cuestionario.html`).

### Contenido por Unidad

-   **Capítulo 1**: Preguntas sobre Conjuntos, Relaciones y Funciones con explicaciones teóricas detalladas.
-   **Capítulos posteriores**: Se agregarán progresivamente cuestionarios específicos para cada tema.

## Uso de Herramientas Tecnológicas

Uno de los objetivos de este proyecto es aprender a utilizar eficientemente las herramientas tecnológicas como apoyo en el estudio del álgebra.

### Calculadora HP Prime

En la medida de las posibilidades y según el contenido de cada unidad, se buscará integrar el uso de la calculadora HP Prime. Para las unidades donde su aplicación sea relevante, se creará una **guía de uso rápido** con ejemplos prácticos y comandos útiles para resolver problemas específicos de la materia.

El material de referencia de la calculadora se encuentra en el directorio `hp-prime/`.

## Generación de Resúmenes en PDF

Para mantener un formato consistente y de alta calidad, los resúmenes de cada unidad se gestionan a través de archivos LaTeX.

### Convención de Nombres

Los archivos de resumen deben seguir el siguiente formato dentro del subdirectorio `resumen/` de cada capítulo:

-   **Fuente LaTeX:** `resumen/resumen-unidad<N>.tex`
-   **Salida PDF:** `resumen/resumen-unidad<N>.pdf`

Donde `<N>` es el número de la unidad correspondiente (ej: `resumen/resumen-unidad1.tex`).

### Instrucciones de Generación

1.  **Prerrequisitos:** Es necesario tener una distribución de LaTeX instalada. En sistemas Debian/Ubuntu, puedes instalarla con los siguientes comandos:
    ```bash
    sudo apt-get update
    sudo apt-get install texlive-latex-base
    sudo apt-get install texlive-latex-recommended
    ```

2.  **Generar el PDF:** Una vez creado o modificado el archivo `.tex`, utiliza el siguiente comando para compilarlo a PDF. Asegúrate de estar en el directorio raíz del proyecto.

    ```bash
    pdflatex -output-directory=unidades/capitulo<N>/resumen/ unidades/capitulo<N>/resumen/resumen-unidad<N>.tex
    ```
    Reemplaza `<N>` por el número de la unidad que deseas compilar. Por ejemplo, para la Unidad 1:
    ```bash
    pdflatex -output-directory=unidades/capitulo1/resumen/ unidades/capitulo1/resumen/resumen-unidad1.tex
    ```
    Esto generará el archivo PDF y los archivos auxiliares (`.aux`, `.log`) dentro del subdirectorio `resumen/` de la unidad correspondiente.

## Contribuciones

¡Las contribuciones son bienvenidas! Si tienes material que no está en el repositorio, encontraste un error o quieres proponer una mejora, no dudes en abrir un **Pull Request**.

## Licencia

Este proyecto se distribuye bajo la licencia MIT. Puedes ver los detalles en el archivo [LICENSE](LICENSE).
