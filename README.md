<!-- badges: start -->
[![Build book](https://github.com/cienciadedatos/r4ds/workflows/Build%20book/badge.svg)](https://github.com/cienciadedatos/r4ds/actions)
<!-- badges: end -->

# R for Data Science

Última versión disponible en http://es.r4ds.hadley.nz.

Este es el repositorio (y branch) para la traducción de [R for Data Science](http://r4ds.had.co.nz).

**Para consultar el libro fuera de línea:**
* Descarga y descomprime esta carpeta: https://github.com/cienciadedatos/r4ds/archive/gh-pages.zip
* Haz clic sobre cualquiera de los archivos con extensión html
* ¡Listo! Ya puedes ver el libro localmente y sin necesidad de conexión a internet.

--- 

¿Encontraste algún error en el libro que es necesario corregir? Puedes abrir un _issue_ en https://github.com/cienciadedatos/r4ds/issues o, idealmente, hacer un _pull request_ con los cambios necesarios. 

1. Haz un fork en tu cuenta de Github.
2. Clona el repositorio a tu cuenta (e.g. `git clone git@github.com:miusuario/r4ds.git`)
3. Crea un branch propio (e.g. correcciones-andrea, puedes hacer `git checkout -b correcciones-miusuario`)
4. Cuando quieras subir tus cambios, haz _push_ a tu cuenta y luego haz un *Pull Request* indicando el branch `traducción` del repositorio `cienciadedatos/r4ds`.

Puedes generar el libro directamente desde el archivo `index.qmd`. Asegurate de tener los siguientes paquetes instalados:

```r
devtools::install_github("cienciadedatos/r4ds")
devtools::install_github("cienciadedatos/datos")
```

Además debes instalar [Quarto](https://quarto.org/docs/get-started/) y hacer un downgrade de `knitr` a la versión 1.42 (e.g., `devtools::install_version("knitr", version = "1.42")`). Si no hacer el downgrade el libro da el siguiente error en las partes que contienen `htmlwidgets`:

```r
Quitting from lines 15-16 [DT htmlwidget] (Reprex.Rmd)
Error in `add_html_caption()`:
! unused argument (xfun::grep_sub("^[^<]*<[^>]+aria-labelledby[ ]*=[ ]*\"([^\"]+)\".*$", "\\1", x))
```

Revisa el código de conducta en el siguiente enlace: https://github.com/cienciadedatos/descripcion-y-orientaciones/issues/1
