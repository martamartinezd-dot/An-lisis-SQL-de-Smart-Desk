# Análisis SQL de ventas y rentabilidad para la optimización del crecimiento en Smart Desk

**Autora:** Marta Martínez Delgado

---

## Descripción del proyecto

Este repositorio contiene un conjunto de consultas SQL desarrolladas para analizar el rendimiento comercial de **Smart Desk** desde una perspectiva estratégica.  
El objetivo principal es evaluar **ventas**, **beneficio** y **eficiencia económica** con el fin de identificar patrones de rentabilidad, comparar industrias, regiones y categorías de producto, y detectar oportunidades de optimización del crecimiento.

El análisis se apoya en datos históricos de ventas, previsiones comerciales y características de las cuentas, utilizando **Snowflake** como entorno de trabajo.

---

## Tecnologías utilizadas

- SQL (Snowflake)
- Base de datos: `UCM`
- Esquema: `SMART_DESK`
- Warehouse: `PONY_WH`
- Rol: `TRAINING_ROLE`

---

## Estructura del análisis

### 1. Análisis de ventas y beneficio por categoría de producto

Se analiza la distribución de ventas, unidades vendidas y beneficio total por categoría de producto para una cuenta específica durante el año 2020.  
Este análisis permite identificar qué líneas de producto aportan mayor valor económico.

---

### 2. Comparación de rendimiento por país en regiones APAC y EMEA

Se comparan ingresos, unidades vendidas y beneficio promedio por país dentro de las regiones **APAC** y **EMEA**.  
El objetivo es detectar diferencias regionales en el comportamiento comercial y posibles oportunidades de mejora.

---

### 3. Análisis del beneficio total por industria en clientes en etapa *Commit*

Se estudia el beneficio total generado por industria considerando únicamente cuentas con oportunidades en estado *Commit* y previsiones elevadas.  
Las industrias se clasifican según su nivel de beneficio, permitiendo identificar aquellas con mayor impacto económico.

---

### 4. Evolución del pronóstico y beneficio real por categoría

Se compara el beneficio real obtenido en 2021 con el pronóstico comercial de 2022, analizando además la antigüedad de las oportunidades.  
Este apartado permite evaluar la coherencia entre previsión y resultados reales.

---

## Caso práctico: análisis estratégico por industria

### 5.2.1 Distribución de ventas, beneficio y número de cuentas por industria

Se analiza el peso de cada industria en términos de:
- Ventas totales  
- Beneficio total  
- Número de cuentas activas  

Este análisis permite entender la contribución global de cada sector al negocio.

---

### 5.2.2 Relación entre unidades vendidas y beneficio total por industria

Se estudia la relación entre el volumen de unidades vendidas y el beneficio total generado por cada industria.  
El objetivo es observar si el beneficio depende principalmente del volumen o de otros factores.

---

### 5.2.3 Análisis del beneficio medio por unidad vendida

Se calcula el **beneficio por unidad vendida** como indicador de eficiencia económica.  
Este enfoque permite comparar industrias más allá del volumen de ventas y centrarse en la rentabilidad.

---

### 5.3.1 Comparación consolidada de ventas, beneficio y eficiencia por industria

Se integran:
- Ventas totales  
- Beneficio total  
- Beneficio por unidad  

en un único análisis para identificar posibles desequilibrios entre volumen y rentabilidad.

5.3.2 Clasificación estratégica de industrias según valor económico

Las industrias se clasifican en función de:
- Beneficio total
- Beneficio por unidad

Esto permite identificar sectores de:
- Alta prioridad estratégica  
- Alta rentabilidad  
- Prioridad media o baja  

Objetivo del proyecto

El proyecto busca responder a la siguiente pregunta de negocio:

**¿Está alineada la estrategia comercial de Smart Desk con las industrias que generan mayor valor económico?**

A partir de los análisis realizados, se identifican sectores con alto volumen de ventas pero menor eficiencia, así como industrias con menor peso en ventas pero alta rentabilidad por unidad.  
Esto permite plantear recomendaciones estratégicas basadas en datos.

Notas

- Todas las consultas incluyen agregaciones a nivel de industria, categoría o país.
- Se utiliza `NULLIF` para evitar errores de división por cero en los cálculos de eficiencia.
- El repositorio está orientado a fines académicos y de análisis estratégico.
