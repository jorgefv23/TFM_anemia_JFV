## Diagnóstico diferencial de anemias mediante parámetros hematológicos y técnicas de machine learning

Bienvenidos a este GitHub,

Mediante los códigos que aquí se pueden encontrar es posible realizar predicciones mediante parámetros de autoanalizadores hematológicos y técnicas de aprendizaje automatizado sobre carencias nutricionales productoras de anemia.

Existen tres códigos diferentes, uno para cada déficit: hierro, vitamina B12 y ácido fólico

A su vez, para permitir su reproducibilidad a usuarios sin acceso a estos parámetros, se anexa un archivo .xls de prueba con datos etiquetados según tengan déficit de hierro o no.

```{r}
library(readxl)
subset_Fe <- read_excel("subset_Fe.xlsx")
```

Si hubiesen problemas para ejecutar el código es importante comprobar se encuentran instalados los principales paquetes empleados, a destacar:

```{r}
library(purr)
library(performanceEstimation)
library(caret)
library(tidyverse)
library(Boruta)
library(glmnet)
library(ranger)
library(caretEnsemble)
library(SuperLearner)
library(adabag)
```

Espero vuestros comentarios y aportaciones 😊
