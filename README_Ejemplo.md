# Predicción de Agotamiento de Stock en Productos

Este proyecto tiene como objetivo anticipar, mediante un modelo de IA, si un producto en bodega se agotará en los próximos días, utilizando variables como historial de ventas, frecuencia de reposición y estacionalidad.

---

## Componentes del sistema

- **Scripts de procesamiento**: ingesta, limpieza, transformación y validación de datos.
- **Base de datos PostgreSQL**: para la carga y consulta estructurada de los datasets.
- **Modelo de IA (scikit-learn)**: clasificación binaria para predecir agotamiento.
- **Metabase (opcional)**: dashboard de visualización de resultados.
- **Documentación**: diseño técnico completo + planificación.

---

## Tecnologías utilizadas

- Python 3  
- Pandas
- Scikit-learn  
- numpy
- PostgreSQL  
- Docker  
- Git / GitHub  
- Jira (planificación)
- dashboard web
---

## Pipeline implementado

| Etapa | Descripción |
|-------|-------------|
| 1. Diseño e instalación | Definición de la arquitectura del sistema, estructura de carpetas del proyecto, configuración del entorno (Python, librerías como Pandas, NumPy y Scikit-learn) y selección de herramientas como SQL y Power BI. |
| 2. Ingesta | Obtención de datos históricos desde archivos CSV (fuentes como Kaggle o Mockaroo), lectura mediante scripts en Python y carga inicial en memoria para su procesamiento. |
| 3. Limpieza | Depuración de los datos: eliminación de duplicados, tratamiento de valores nulos, corrección de formatos y validación de tipos de datos para asegurar calidad. |
| 4. Transformación | Generación de nuevas variables relevantes como días sin reposición, tasa de ventas, stock mínimo y variables necesarias para el entrenamiento del modelo predictivo. |
| 5. Validación | Verificación de consistencia de los datos: revisión de rangos válidos, coherencia entre variables y validación básica antes de su almacenamiento o uso en el modelo. |
| 6. Carga en PostgreSQL | Almacenamiento del dataset limpio y transformado en una base de datos SQL para facilitar consultas, persistencia y uso posterior en el sistema. |
| 7. Entrenamiento IA | Desarrollo y entrenamiento de un modelo de Machine Learning (clasificación binaria) utilizando Scikit-learn para predecir la variable `se_agotara`. |
| 8. Evaluación | Evaluación del rendimiento del modelo mediante métricas como accuracy, recall y análisis de resultados para validar su efectividad. |
| 9. Visualización | Creación de dashboards (Power BI o web) para mostrar predicciones, estado del stock, alertas de quiebre y apoyo a la toma de decisiones. |

---

## 📂 Estructura del repositorio

```
agotamiento-stock/
├── README.md
├── docs/
│   └── diseño_tecnico.pdf
├── scripts/
│   ├── ingesta.py
│   ├── limpieza.py
│   ├── transformacion.py
│   └── entrenamiento.py
├── data/
│   └── productos_ventas.csv
├── dashboards/
│   └── dashboard_metabase.png
├── docker-compose.yml
```

---

## Cómo ejecutar el sistema (entorno ya instalado)

1. Clonar el repositorio  
   `git clone https://github.com/usuario/agotamiento-stock.git`

2. Entrar a la carpeta del proyecto  
   `cd agotamiento-stock`

3. Ejecutar el pipeline manualmente por etapas  
   Ejemplo:  
   `python scripts/ingesta.py`  
   `python scripts/limpieza.py`  
   `python scripts/entrenamiento.py`

4. Visualizar los resultados y métricas desde consola o dashboard

---

## Documentación técnica

El documento de diseño técnico está disponible en:  
[`docs/diseño_tecnico.pdf`](docs/diseño_tecnico.pdf)

---

## Equipo

- Integrante 1 – Procesamiento y limpieza  
- Integrante 2 – Modelado y entrenamiento  
- Integrante 3 – Visualización y documentación
