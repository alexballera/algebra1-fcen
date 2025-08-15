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

Dentro de cada capítulo, encontrarás los apuntes teóricos, la guía de trabajos prácticos y las soluciones correspondientes.

## Uso de Herramientas Tecnológicas

Uno de los objetivos de este proyecto es aprender a utilizar eficientemente las herramientas tecnológicas como apoyo en el estudio del álgebra.

### Calculadora HP Prime

En la medida de las posibilidades y según el contenido de cada unidad, se buscará integrar el uso de la calculadora HP Prime. Para las unidades donde su aplicación sea relevante, se creará una **guía de uso rápido** con ejemplos prácticos y comandos útiles para resolver problemas específicos de la materia.

El material de referencia de la calculadora se encuentra en el directorio `hp-prime/`.

## Generación de Resúmenes en PDF

Para mantener un formato consistente y de alta calidad, los resúmenes de cada unidad se gestionan a través de archivos LaTeX.

### Convención de Nombres

Los archivos de resumen deben seguir el siguiente formato dentro del directorio de cada capítulo:

-   **Fuente LaTeX:** `resumen-unidad<N>.tex`
-   **Salida PDF:** `resumen-unidad<N>.pdf`

Donde `<N>` es el número de la unidad correspondiente (ej: `resumen-unidad1.tex`).

### Instrucciones de Generación

1.  **Prerrequisitos:** Es necesario tener una distribución de LaTeX instalada. En sistemas Debian/Ubuntu, puedes instalarla con los siguientes comandos:
    ```bash
    sudo apt-get update
    sudo apt-get install texlive-latex-base
    sudo apt-get install texlive-latex-recommended
    ```

2.  **Generar el PDF:** Una vez creado o modificado el archivo `.tex`, utiliza el siguiente comando para compilarlo a PDF. Asegúrate de estar en el directorio raíz del proyecto.

    ```bash
    pdflatex -output-directory=unidades/capitulo<N>/ unidades/capitulo<N>/resumen-unidad<N>.tex
    ```
    Reemplaza `<N>` por el número de la unidad que deseas compilar. Por ejemplo, para la Unidad 1:
    ```bash
    pdflatex -output-directory=unidades/capitulo1/ unidades/capitulo1/resumen-unidad1.tex
    ```
    Esto generará el archivo PDF y los archivos auxiliares (`.aux`, `.log`) dentro del directorio de la unidad correspondiente.

## Contribuciones

¡Las contribuciones son bienvenidas! Si tienes material que no está en el repositorio, encontraste un error o quieres proponer una mejora, no dudes en abrir un **Pull Request**.

## Licencia

Este proyecto se distribuye bajo la licencia MIT. Puedes ver los detalles en el archivo [LICENSE](LICENSE).
