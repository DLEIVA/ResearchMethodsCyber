# ResearchMethodsCyber
## Materials for course Research Methods in Cyberspace, Behavior, and e-Therapy

### November 19-21, 2024

### David Leiva Ureña

#### Department of Social Psychology and Quantitative Psychology, University of Barcelona

---

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work has been done under the license <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8152802.svg)](https://doi.org/10.5281/zenodo.8152802)

## About the course

Este curso se ha pensado como un taller de tipo práctico en el que se introducirá a los participantes en la Ciencia de Datos mediante el software estadístico de libre distribución R. Puesto que se trata de un lenguaje de programación y su aprendizaje puede resultar costoso, se utilizarán numerosos ejemplos que faciliten el dominio de la sintaxis básica. A lo largo de las sesiones se capacitará a los participantes a ser autónomos en aquellas técnicas básicas relacionadas con la visualización de datos, la modelización estadística así como en la elaboración de informes técnicos con herramientas de R en combinación con programas como $\LaTeX$ o *Markdown*. Dado el carácter eminentemente práctico del curso, éste debería realizarse en aula de ordenadores o bien que cada participante lleve un ordenador portátil.

### Programa del curso:

1. Correlation tests (2h)
 - Instalación y ejecución de R
 - RStudio: una IDE para R
 - Introducción al *tidyverse*

2. Linear regression models (2h)
 - Paquetes gŕaficos básicos 
 - *ggplot2* y otros paquetes

3. Mediation and moderation models (2h)
 - Ejemplos de modelos estadísticos
 - Modelización con tidymodels

4. APA guidelines for reporting research results (2h)
 - Generación de documentos con *knitr* y *RMarkdown*
 - Desarrollo de aplicaciones dinámicas con Shiny

## About the lecturer

My name is David Leiva and I am an Associate Professor in the Department of Social Psychology and Quantitative Psychology. I teach undergraduate, masters and doctoral courses in Statistics, Research Techniques, Statistical Modeling, Data Science and Applied Mathematics. My main research interests are dyadic data analysis, modeling behavior and statistical software. I have also participated in numerous works in fields such as Organizational Psychology, Neuropsychology, Psychogerontology or Biology, among others. You can find my CV in the following [link](https://github.com/DLEIVA/CV/blob/main/CV_DLU_2023.pdf).

## Previous steps

Please make sure that you have at least version 4.3 of R installed &mdash; *and preferably version 4.4* &mdash; (as depending on the packages used they require updated versions of the software). Note that R and RStudio are two different programs: it is not sufficient to have an updated version of RStudio as R is updated independently on a regular basis.

To check the version of R installed, you can run

```r
version
```

in R and read in the `version.string` section (or the `major` and `minor` sections).

If the installed version of R is < 4.3.0, you will need to upgrade the program after downloading and installing it. To download R go to the [CRAN Download page](https://cran.r-project.org/) and select the appropriate link for your operating system:

* [Windows](https://cran.r-project.org/bin/windows/)
* [MacOS X](https://cran.r-project.org/bin/macosx/)
* [Linux](https://cran.r-project.org/bin/linux/)

Throughout the sessions we will be using various R packages that you will need to have installed. Before the course starts, run the following code which will update the installed packages and install the packages needed during the course:

```r
# Update packages
update.packages(ask = FALSE, checkBuilt = TRUE)

# Some packages to be installed
pkgs <- c('haven','tidyverse','car','here','boot','effects','lmtest','DiagrammeR','interactions','compareGroups','apaTables','dslabs','ggthemes','ggrepel','ggstatsplot','patchwork')

# Install these packages
install.packages(pkgs, Ncpus = 4) # Specify Ncpus depending on the number of available CPUs
```

*It is advisable to work on these 2 resources beforehand in order to make the most of the course.*

[Installing R and RStudio](https://learnr-examples.shinyapps.io/ex-setup-r/)

[R basic programming](https://posit.cloud/learn/primers/1.2)

# Course Materials

## From Github

To download the course materials you can open RStudio and run `use_course()` as shown below:

```r
usethis::use_course("DLEIVA/ResearchMethodsCyber")
```

Once the instruction is executed you will be asked if you want to download the course materials to the `~/Desktop` directory (in this case, `~/` refers to your root directory). Press the indicated number and press the <kbd>Enter</kbd> key to show your agreement. The materials will be downloaded as a zip file and extracted automatically.

After extraction, you will be asked if you want to delete the downloaded `.zip` file. Select the option you think is appropriate.

Finally, after answering this question, Rstudio will load the course project in a new RStudio session. Once the project is open, you can close the other RStudio window (where you have executed the `use_course()` instruction).

### Direct download

If you are not using RStudio or know what you are doing, you can download the zip file directly from <https://github.com/DLEIVA/ResearchMethodsCyber.git>. Extracting files and starting in the correct directory will then be up to you.

### OTHER RESOURCES

**Basic R Courses**

https://www.codecademy.com/learn/learn-r

https://www.codecademy.com/learn/learn-statistics-with-r

https://www.codecademy.com/learn/r-for-programmers

**Recommended bibliography**

Verzani, J. (2014). Using R for Introductory Statistics (2nd ed.). Chapman and Hall/CRC. https://doi.org/10.1201/9781315373089 [Free -but older- version in this link](https://cran.r-project.org/doc/contrib/Verzani-SimpleR.pdf)

Field, A., Miles, J., & Field, Z. (2012). Discovering statistics using R. SAGE Publications.
