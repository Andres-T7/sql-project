# Análisis de Mercado de Libros Digitales — SQL

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=sqlalchemy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

## Descripción
Análisis exploratorio sobre la base de datos de un competidor en el mercado de aplicaciones de libros digitales, con más de 1,000 títulos, 179 editoriales y miles de calificaciones de usuarios. El proyecto surge del contexto post-pandemia, donde el consumo de libros digitales creció significativamente, generando una oportunidad para el lanzamiento de un nuevo producto en este mercado.

## Objetivo
Extraer insights clave del catálogo y del comportamiento de los usuarios para fundamentar decisiones estratégicas en el diseño de una nueva app de libros, identificando editoriales relevantes, autores mejor valorados y patrones de participación de los usuarios.

## Archivos del proyecto
- `Proyecto_Ebooks_SQL.ipynb` — Notebook principal con el análisis completo
- `images/` — Diagrama de la estructura de los datos
- `.env.example` — Plantilla de variables de entorno requeridas

## Hallazgos principales
1. El **80% del catálogo (819 de 1,000 libros)** corresponde a publicaciones posteriores al año 2000, lo que indica una oferta alineada con intereses actuales.
2. **Penguin Books** es la editorial con mayor presencia en el catálogo con **42 libros** de más de 50 páginas, posicionándola como un socio estratégico potencial.
3. **J.K. Rowling/Mary GrandPré** obtuvo la calificación promedio más alta (**4.28/5.0**) entre autores con al menos 50 calificaciones, lo que indica un alto engagement en títulos con amplio volumen de evaluaciones.
4. Los usuarios más activos califican una gran cantidad de libros, pero generan pocas reseñas de texto, lo que representa una oportunidad para incentivar participación más cualitativa.

## Conclusiones y recomendaciones de negocio
- Priorizar en el sistema de recomendaciones de la App a autores y libros con alta calificación y volumen significativo de evaluaciones.
- Establecer alianzas estratégicas con Penguin Books dado su peso en el catálogo y su valoración por los usuarios.
- Implementar mecanismos de incentivos para fomentar la escritura de reseñas entre los usuarios más activos, mejorando la calidad de la información disponible para otros lectores.

## Descripción de los datos
El cliente suministró una base de datos que contiene información de un competidor en el mercado. El dataset integra datos de libros, editoriales y autores, además de calificaciones y reseñas de clientes, distribuidos en las siguientes tablas:

| Tabla        | Descripción                                                      |
| ------------ | ---------------------------------------------------------------- |
| `books`      | Información de cada libro: título, páginas, fecha de publicación |
| `authors`    | Identificación y nombre de autores                               |
| `publishers` | Identificación y nombre de editoriales                           |
| `ratings`    | Calificaciones numéricas por libro y usuario                     |
| `reviews`    | Reseñas de texto por libro y usuario                             |


## Requisitos
`pandas` · `sqlalchemy` · `psycopg2-binary` · `python-dotenv`
```bash
pip install -r requirements.txt
```
