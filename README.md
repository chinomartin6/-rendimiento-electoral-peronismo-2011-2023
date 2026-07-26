# Rendimiento Electoral del Peronismo en Elecciones Generales — Argentina 2011-2023

Proyecto final del curso **Introducción al Análisis de Datos** (Universidad de Buenos Aires).
Análisis de datos electorales públicos aplicado a un problema de ciencia política.

## Descripción

Este proyecto analiza el rendimiento electoral de las coaliciones vinculadas al Partido Peronista en cada provincia de Argentina, a lo largo de las elecciones generales presidenciales del período 2011-2023. Combina extracción, limpieza y control de calidad de datos electorales públicos con análisis comparado por provincia.

## Pregunta de investigación

**¿Cuál ha sido el rendimiento electoral de las distintas coaliciones formadas por el Partido Peronista en cada una de las provincias de la República Argentina en las elecciones generales del período 2011-2023?**

## Decisiones metodológicas

- **Se analizaron únicamente elecciones generales**, excluyendo las PASO. La decisión responde a que el objetivo es medir la intención de voto "firme" del electorado al momento de definir representación, y no el efecto de "termómetro electoral" que suelen tener las PASO dentro de cada espacio político.
- **Recorte temporal:** las cuatro elecciones generales presidenciales del período — 2011, 2015, 2019 y 2023.
- **Métrica principal:** proporción de votos obtenidos por el espacio peronista sobre el total del padrón electoral (electores habilitados) de cada provincia, promediada a lo largo de los años disponibles.

## Objetivos

- Extraer, limpiar y controlar la calidad de datos electorales públicos hasta obtener un dataset confiable y analizable por provincia y año.
- Comparar el desempeño electoral del espacio peronista a lo largo del territorio, identificando el distrito con mayor y menor respaldo relativo en el período.

## Principales hallazgos

- **Mayor respaldo relativo:** Formosa (45,5%), Chubut (40,5%) y Tucumán (39,1%) — provincias del norte argentino y la Patagonia con estructuras políticas provinciales tradicionalmente asociadas al peronismo.
- **Menor respaldo relativo:** Córdoba (16,3%, con datos completos para los 4 años) y San Luis (20,2%). Santiago del Estero registra el valor más bajo (12,9%), aunque con datos disponibles para solo 2 de los 4 años, por lo que se interpreta con mayor cautela.
- El detalle completo por provincia, la metodología y las limitaciones del análisis están documentados en el informe técnico (`informe_final.pdf`).

> **Nota sobre el proceso:** una versión previa de este análisis contenía un error de código que hacía que el resultado final reflejara solo la elección de 2015 en lugar del promedio de las 4 elecciones, además de un error en la limpieza del campo de votos que inflaba los porcentajes hasta 10 veces. Ambos se detectaron mediante control de calidad de datos y se corrigieron antes de este resultado — el proceso completo está documentado en el notebook y en el informe técnico.

## Herramientas

`Python` · `Pandas` · `NumPy` · `Matplotlib` · control de calidad y limpieza de datos

## Estructura del repositorio

```
├── notebooks/
│   └── rendimiento_electoral_peronismo_2011_2023.ipynb
├── data/
│   └── datos_electorales_err.xlsx
├── informe_final.pdf
└── README.md
```

## Autor

**Nicolás Martín** — [LinkedIn](https://linkedin.com/in/nicolás-m-65295a108)
