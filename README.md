# Proyecto: Predicción de Precios de Casas 🏠

## Introducción

La predicción de precios de bienes inmuebles es un área clave en la intersección de los negocios y la ciencia de datos. En este proyecto, abordarás el desafío de estimar el precio de las casas. Trabajaras con un conjunto de datos real, que contiene información detallada sobre propiedades en Madrid, como su tamaño, ubicación, número de habitaciones, tipo de propiedad, y más. El objetivo principal del proyecto es predecir el precio de una casa, 

## Contexto del Problema

El mercado inmobiliario es dinámico y está influenciado por múltiples variables, como la ubicación, las características de la propiedad y las condiciones económicas. Un modelo predictivo preciso puede ser una herramienta poderosa para agentes inmobiliarios, compradores y vendedores. Este proyecto te sumergirá en la complejidad de estos factores y te enseñará cómo transformarlos en conocimiento útil para la toma de decisiones.

## Pasos para el Desarrollo 

1. **Carga y Exploración del Dataset**

   - Seleccion de datos solo de madrid
   - extraccion de datos en columnas con diccionarios dentro.
   - borrado de duplicados
   - columnas seleccionadas para el analisis:
   - price ,propertyType, operation, size, exterior, rooms,
     bathrooms, municipality, status, newDevelopment, priceByArea,
     floor, district, neighborhood, hasLift, hasParkingSpace,
     typology, subTypology

2. **Preprocesamiento de Datos**

   - Test de imputacion de nulos con knn y imputer, mismo resultado nos quedamos con knn.

   - Imputacion de todas las categoricas con nulos con categoria "Unknown".

   - Enconding con target.

   - imputar numericos outliers con mediana
     
   - Despues de testear RobustScaler, MinMaxScaler, Normalizer, StandardScaler, nos quedamos con Normalizer

3. **Construcción del Modelo**

   - Test con DecisionTreeRegressor, RandomForestRegressor, GradientBoostingRegressor, XGBRegressor.

4. **Visualización de Resultados**

   - Mejor resultado RandomForestRegressor.

