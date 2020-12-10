

---
title: "Turismo en España"
subtitle: "Origen, Motivos, Gasto"
author: "Hugo , Pavlina y Anna"
date: "2020"
output: ioslides_presentation

---


```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = FALSE)
```

# Presentación del tema 



## ¿ Por qué hemos elegido ese tema?
-Hemos elegido el tema del turismo porque es un factor clave para el desarrollo socioeconomico y cultural de un país <div class="red2">

> - La fuente de datos utilizada es **INE.es**
> - Los datos estarán subidos en **Github** 


## Slide con una imagen y texto 

- Un poco de texto y abajo una imagen

```{r, echo = FALSE, eval = TRUE, out.width = "76%", fig.align = "center"}
knitr::include_graphics(here::here("/imagenes", "spain_turismo.jpg") ) 
```

- Otro bullet con texto.


---- 


```{r echo = FALSE, out.width = "73%", fig.align = "center" , caption = "<https://xkcd.com>"}
knitr::include_graphics(here::here("/imagenes","getty_images.jpg"))
```

# Apartado para los gráficos


## Slide con indentation {.smaller}

- Gráficos elaborados

    - Gráfico 1

    - Gráfico 2


- Explicación de los gráficos

```{r echo = FALSE, out.width = "73%", fig.align = "center" , caption = "<https://xkcd.com>"}
knitr::include_graphics(here::here("/imagenes","motivos.jpeg"))
```





## Otra slide "normal" con `##` {.smaller}

-  Un enlace: para más información sobre `ioslides`, ve [aquí](https://rmarkdown.rstudio.com/ioslides_presentation_format.html)




# **R-base  vs. [tidyverse](https://www.tidyverse.org/)**  

#### Esto es un poco forzar las cosas, pero ... funciona
   
   
---

  - "Programs must be written for people to read, and only incidentally for machines to execute"  --- Hal Abelson

<br>

  - "If I had one thing to tell biologists learning bioinformatics, it would be write **code for humans**, write **data for computers**" --- Vince Buffalo
  
  <br>
  
  - "An important aspect of writing data for computers is to **make your data TIDY**" --- Jenny Bryan

---
    
- Lo siguiente es un chunk, en realidad no, porque le faltan las llaves `{}`, pero si verá de forma especial

```r
data %>% filter(X1 > 400) %>% group_by(X2) %>% summarise(media = mean(X3))
```
  
--- 

Esto sí son chunks. Se ejecutarán los 2. El primero no se verá (`echo = FALSE`) 

```{r, echo = FALSE}
library(ggplot2)
```

```{r, echo = TRUE}


```


## Bibliografía. {.smaller}

En realidad son algunos links por si os ayudan a hacer vuestras `ioslides`


- En el libro [R Markdown: The Definitive Guide](https://bookdown.org/yihui/rmarkdown/) hay un capítulo dedicado a las `ioslides`, concretamente [aquí](https://rmarkdown.rstudio.com/ioslides_presentation_format.html). El repo con el código fuente del libro está [aquí](https://github.com/rstudio/rmarkdown-book) y el del capítulo 4 sobre presentaciones [aquí](https://github.com/rstudio/rmarkdown-book/blob/master/04-presentations.Rmd)

- [Presentation with ioslides](https://garrettgman.github.io/rmarkdown/ioslides_presentation_format.html)

- [Tutorial sobre Rmd](https://codingclubuc3m.rbind.io/post/2019-09-24/) con una pequeña sección sobre `ioslides`.

- Un [ejemplo de *ioslides*](https://choux130.github.io/slide_thesis_ioslides/#1). El código está [aquí](https://github.com/choux130/slide_thesis_ioslides). 

<br><br>

Dos links más que igual os resultan complicados:  

- <https://www.rdocumentation.org/packages/rmarkdown/versions/1.10/topics/ioslides_presentation>  
  
- <https://stackoverflow.com/questions/50258283/how-to-enable-syntax-highlighting-in-code-chunks-within-r-markdown-ioslides-pres>  
  
  



# Gracias por su atención !!
