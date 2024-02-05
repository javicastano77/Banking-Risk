![image](https://github.com/javicastano77/Banking-Risk/assets/156696799/bf69f672-5b26-4297-b1ea-8adb13d3dfc9)


# Analísis de perfiles de Alto Riesgo

En los últimos años hemos podido observar cómo en el mundo de los negocios cada vez más son las empresas que han decidido analizar a sus clientes, no tanto desde un punto de vista comercial, sino a través del impacto que éstos pueden generar en el seno de sus organizaciones. Esto ha generado una clasificación antagónica: **"Alto Riesgo"** vs **"Bajo Riesgo"**, algo que no solo sucede en sectores tradicionales como la banca, sino también en entornos más complejos como el mundo Cyber, Blockchain, Cloud, etc.

## 1. Descripción

Los datos del proyecto provienen de [Risk Analytics in Banking](https://www.kaggle.com/datasets/sabarostami/risk-analytics-in-banking) un dataset de Kaggle con un amplio registro de clientes de un banco.

En esta dataset original podemos encontrar un detalle amplio de esa cartera de clientes dividida en:

* **Variables sociodemorgráficas**: estado civil, propiedades, miembros familiares, ocupación, etc.
* **Variables económicas**: cantidad del prestamo, anualidad, tipo de préstamo, etc.

## 2. Objetivos

El proyecto está dividido en 3 objetivos principales:

1 - Analizar de manera detallada las características que configurarían a los perfiles de **Alto Riesgo**, y aislar así aquellas variables que tengan una influencia notoria en esta clasificación.

2 - Establecer una nueva clasificación de estos perfiles, tras el análisis realizado en el paso previo.

3- Realizar una comparativa entre la clasificación original y la nueva, comprobando el acierto y la robustez del modelo generado.

## 3. Proceso

El proceso definido para este proyecto se desglosa en estos pasos:

* i. Limpieza de los datos: chequeo de valores nulos, duplicados y dtype.
* ii. transformación de los datos: mejora de la consistencia, normalización de datos, etc.
* iii. análisis de las variables: estudio del compartamiento del target en base a las variables sociodemográficas y numéricas.
* iv. identificación de la correlación entre targets: identificar aquellos parámetros y condiciones que mayor grado de explicación tienen para la clasificación de los perfiles **Alto riesgo** y **Bajo Riesgo**.
* v. establecimiento de parámetros propios: establecer las características que definen a los perfiles
* vi. comparativa de clasificación original y modelo 1: generación de nueva variable de clasificación y testeo con tabla de contingencia y matriz de confusión su usabilidad
* vii. aplicación de cálculos tradicionales de riesgos: analísis del modelo de cálculo de riesgo de crédito estandar y aplicación a la dataset tratada
* viii. comparativa de clasificación original y modelo 2: generación de nueva variables en base a ese cálculo y testeo nuevamente

## 4. Uso

El proceso realizado se encuentra  en la carpeta de Final Process con un detalle step by step de todos los pasos seguidos durante el proyecto.

## 5. Conclusiones

Tras la realización del proyecto las principales conclusiones obtenidas serían:

1 - El scoring es un proceso complejo de aislar, dado que cada empresa y cada sector usa un criterio intenro y confidencial para establecer esa clasificicación de sus clientes.
2 - En el mundo bancario no hay una distribución similar entre los clientes de Alto riesgo y Bajo, habiendo una relación 20-80 respectivamente, dado que un banco no puede asumir una cartera tan elevada de clientes de Alto Riesgo.
3- La clasificación de los modelos es tendencioso, dado que debe clasificar de manera eficiente a los clientes de Alto Riesgo, por lo que la robustez del modelo caerá en detrimento por este principio.
