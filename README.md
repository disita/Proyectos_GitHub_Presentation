# Proyectos_GitHub_Presentation

![](http://www.quickmeme.com/img/75/7509f68823389e4af3777ca6d3744c632cc32ab3547bc56e319126aa29ab149a.jpg)

[Fuente: quickmeme](http://www.quickmeme.com/p/3vs3uz)

Este repositorio se creó para la elaboración de la presentación del paper _Excuse me, do you have a moment to talk about version control?_ (Brayan, 2017) de la clase de **Desarrollo de Proyectos I** de la Maestría en Ciencia de Datos (MCD) de la Universidad de Guadalajara.

Su motivo principal es documentar el procedimiento y servir como guía de apoyo para aquellos que deseen hacer una presentación desde `python`.

## ¿Cómo hacer presentación en `python`?

Hay muchas maneras y vías sobre cómo desarrollar una presentación utilizando `python`. Sin embargo, decidimos utilizar la librería de `{RISE}` por su facilidad de uso.

## Usando `{RISE}`

La librería `{RISE}` (nombre que proviene del acrónimo: Reveal.js - Jupyter/IPython Slideshow Extension) en Python es una herramienta que permite crear presentaciones interactivas utilizando Jupyter Notebook. Algunas de las principales ventajas y desventajas de uso son las siguientes:

**Ventajas:**

* Interactividad: RISE permite crear presentaciones interactivas en Jupyter Notebook, lo que significa que puedes ejecutar código en tiempo real durante la presentación. Esto es muy útil para demostrar conceptos, visualizar datos y realizar análisis en vivo.
* Integración con Jupyter: Como `{RISE}` se integra directamente con `Jupyter Notebook`, puedes aprovechar todas las características y capacidades de Jupyter, incluyendo soporte para múltiples lenguajes de programación como Python, R, Julia, entre otros.
* Personalización: `{RISE}` ofrece una amplia gama de opciones de personalización para adaptar la apariencia de tus presentaciones a tus necesidades. Puedes cambiar temas, ajustar el diseño y agregar elementos visuales personalizados.
* Exportación y compartición sencilla: Puedes exportar tus presentaciones `{RISE}` a diversos formatos, como HTML, PDF o diapositivas estáticas, lo que facilita su distribución y uso por parte de otros.
* Comunidad activa: `{RISE}` es una herramienta popular y cuenta con una comunidad activa de usuarios y desarrolladores, lo que significa que puedes encontrar documentación, tutoriales y soporte en línea fácilmente.

**Desventajas:**

* Requiere `Jupyter Notebook`: Para utilizar `{RISE}`, necesitas tener instalado Jupyter Notebook, lo que podría requerir una curva de aprendizaje adicional si no estás familiarizado con esta plataforma.
* Dependiente del navegador: RISE depende de un navegador web para la presentación. Esto puede limitar la portabilidad si necesitas presentar en un entorno sin acceso a un navegador.
* Curva de aprendizaje: Si bien `{RISE}` es relativamente fácil de usar, puede llevar tiempo acostumbrarse a su flujo de trabajo si eres nuevo en `Jupyter Notebook` y no tienes experiencia previa en la creación de presentaciones interactivas.
* Limitaciones en la exportación: Aunque `{RISE}` permite la exportación a varios formatos, la calidad y la apariencia de las diapositivas pueden variar en función del formato elegido y de la complejidad de la presentación.

De esta manera, `{RISE}` se vuelve una herramienta poderosa para crear presentaciones interactivas en `Jupyter Notebook`, pero su utilidad dependerá de tus necesidades y de tu familiaridad con la plataforma. Puede ser una excelente opción si deseas combinar análisis de datos y presentaciones en un entorno interactivo y colaborativo.

## Pasos a seguir

Basados en diferentes tutoriales, (como [este](https://mljar.com/blog/jupyter-notebook-presentation/) u este [otro](https://www.edlitera.com/blog/posts/rise-presentations-jupyter), se deben seguir tres pasos básicamente:

1. Instalar la librería de `{RISE}`. Para poder instalar la librería se puede lograr usando **pip** (`pip install rise`), o bien desde **Conda** (`conda install -c conda-forge rise`).
2. Elaborar la presentación en `jupyter Notebook`. Una vez que fue instalada la librería, se deberá crear la presentación en `jupyter Notebook`. Las presentaciones pueden tener código o bien ser puro Markdown. Una vez que se guardó el *notebook*, se deberá crear la presentación en el menú `View ➡️ Cell Toolbar ➡️ Slideshow`. Esto nos permitirá decirle a `jupyter` que nuestro _notebook_ es una presentación. Sin embargo, además de seguir este paso, se deberá declar que tipo de **diapositiva** (*slide*) será convertida cada celda del código (es recomendable dejar todo en `Slide`:
   * `Slide` - la celda será una nueva diapositiva;
   * `Sub-Slide` - la celda se mostrará como parte de la diapositiva anterior; para acceder a ella se deberá utilizar la flecha hacia abajo del teclado;
   * `Fragment` - la celda aparecerá en la diapositiva actual y se agregará al contenido anterior. Estará disponible en navegación con flecha hacia abajo y flecha hacia la derecha;
   * `Skip` - el contenido no se mostrará en la presentación;
   * `Notes` - notas para diapositiva, el contenido de la celda no se muestra en la presentación.
3. Convertir nuestro archivo `.ipynb` en uno tipo `.html`. Para poder hacer esto existen varias modalidades, las más comunes:
   * Mostrar todo el contenido: `jupyter nbconvert --to slides presentation.ipynb`
   * No mostrar el código: `jupyter nbconvert --to slides --no-input presentation.ipynb`

## Voila!

¡Ahora toca aprender **GitHub**!

![](https://res.cloudinary.com/practicaldev/image/fetch/s--NUSRQ-3J--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://i.redd.it/5iphhycu0io11.png)

## Referencias

* Bryan, J. (2017, 28 de agosto). _Excuse me, do you have a moment to talk about version control?_ [Conferencia en línea]. RStudio and the Department of Statistics, University of British Columbia.
* [RISE](https://rise.readthedocs.io/en/stable/)
* https://mljar.com/blog/jupyter-notebook-presentation/
* https://www.edlitera.com/blog/posts/rise-presentations-jupyter


