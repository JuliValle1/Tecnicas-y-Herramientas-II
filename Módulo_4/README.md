# Módulo 4: Análisis Espacial con QGIS

## Resumen del Proyecto

En este módulo se trabajó en el procesamiento y manejo de datos alfanuméricos y geográficos a través de Sistemas de Información Geográfica (SIG) en **QGIS**, junto con la integración de consultas espaciales[cite: 18].

El objetivo central es brindar al perfil de ingeniería industrial herramientas avanzadas de ingeniería de datos y análisis territorial para optimizar la toma de decisiones logísticas y de localización[cite: 18].

## Desarrollo de la Actividad 1

La propuesta permite auditar la distribución territorial del entramado industrial en Mendoza, examinando variables críticas como el área total, la absorción de mano de obra y los niveles de impacto ambiental de los sectores y parques industriales regionales[cite: 18].

1. **Procesamiento Vectorial y Raster:** Combinación de capas puntuales (geolocalización de predios) y polígonos (límites jurisdiccionales y polígonos industriales en `.shp`), complementado con la lectura de capas raster[cite: 18].
2. **Gestión y Edición de Tablas de Atributos:** Activación de edición para digitalizar parcelas, corregir geometrías y poblar las tablas con indicadores de área, empleo generado e impacto[cite: 18].
3. **Modelado Espacial Avanzado:** Creación de diagramas de Voronoi y redes de Delaunay para diagnosticar patrones de cobertura, proximidad y articulación espacial entre los nodos industriales[cite: 18].
4. **Publicación Web Georreferenciada:** Empleo del complemento `qgis2web` para exportar la visualización en formato HTML e interactivo (OpenLayers), permitiendo alternar capas desde el navegador[cite: 18].

## 🌐 Geoportal Web

Para acceder a la visualización dinámica del mapa interactivo, ingresa mediante el siguiente enlace:

👉 [Acceder al Mapa Interactivo de Parques Industriales](nombre_de_tu_archivo.html)
## Contenido de la Actividad 2

### Resumen de la Actividad

Esta segunda etapa del módulo estuvo enfocada en el análisis ambiental y el tratamiento de imágenes satelitales en formato raster[cite: 19]. El propósito central consistió en medir y contrastar la evolución en la cobertura de nieve dentro del área del Valle de las Lágrimas entre dos momentos temporales (hace dos años en comparación con la toma actual)[cite: 19].

### Metodología y Herramientas Utilizadas

1. **Tratamiento de Capas Raster:** Carga y superposición de tomas satelitales `.tif` (provenientes del programa Copernicus) asociadas a las dos ventanas temporales de estudio[cite: 19].
2. **Reubicación y Proyección Cartográfica:** Cambio del Sistema de Referencia de Coordenadas (SRC) del proyecto, migrando de coordenadas geográficas (EPSG:4326) hacia una proyección métrica (**EPSG:32719 - WGS 84 / UTM zone 19S**)[cite: 19]. Este procedimiento es fundamental para asegurar precisión métrica y corregir distorsiones topográficas durante el cálculo de superficies[cite: 19].
3. **Vectorización de Coberturas:** Generación de capas vectoriales de tipo polígono (`Shapefiles`) para la delimitación y extracción del manto nival en cada etapa, empleando herramientas de edición y digitalización manual[cite: 19].
4. **Cálculo Superficial y Geoprocesamiento:** Aislamiento de capas geométricas y uso de la Calculadora de Campos mediante la expresión espacial (`$area / 10000`) en la tabla de atributos[cite: 19]. Esto permitió obtener la extensión exacta procesada matemáticamente en **hectáreas (ha)** para realizar el análisis comparativo[cite: 19].

## 🌐 Visor Web Interactivo

Puedes examinar la plataforma interactiva del mapa directo en el enlace a continuación: 👉 [Ver Mapa Interactivo del Valle de las Lágrimas](nombre_del_mapa.html)

## 📥 Sección de Descargas

Los paquetes comprimidos (.zip) con los proyectos están disponibles en los siguientes hipervínculos[cite: 19]:

[Descarga aquí el paquete de la Actividad 1 (.zip)](actividad1.zip)

[Descarga aquí el paquete de la Actividad 2 (.zip)](actividad2.zip)
