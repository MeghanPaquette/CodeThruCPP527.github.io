---
title: "Improving Visualizations with Esquisse"
author: "Meghan Paquette"
date: "10/8/2020"
output: 
  html_document:
    df_print: paged
    theme: darkly
    highlight: haddock
---

```{r setup, include = FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

### Finding a Topic

Completing a Code Through previosly in CPP526 was a little easier given even very basic packages could be used. For this course, I wanted to find a package I haven't really used yet that also brings in my interest in data visualization.  I first started looking at packages to demonstrate, and I came across *esquisse*. This package allows the user to ‘drag-and-drop’ information as an add-in for generating plots in R. That’s right – esquisse is a package that lets you create plots without having to code them. As coding is something I am still learning, this intrigued me. 

<br>

### Loading the Package and Data

For the code-through, I am loading two data sets, just as an example. Esquisse looks at the type of data such as numerica or factor. 

```{r}
library(ggplot2)
library(esquisse)
```

```{r}
dat <- USArrests
head(dat, 3) 
```
```{r}
dat2 <- mpg
head(dat2, 3)
```
<br>

### Using the Package

Now, from here, when this code chuck below runs, a pop-up will appear which is where you can ‘drag-and-drop’ information. 
<br>

This part below would be in an r code chunk, but for the sake of knitting to html, it is listed as a stand alone in bold. 
<br>

{r}**esquisse::esquisser()**

<br>

##### STEP 1: Select what dataset you want to use. I imported two datasets above, so you can see.
<br>
![](StartPage.jpeg)

<br>

##### STEP 2: Select variable and convert any variables as desired/needed. 
<br>
![](DataSelect.jpeg)
