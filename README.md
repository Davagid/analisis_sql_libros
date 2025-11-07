# Análisis SQL de Libros — Proyecto Final 

## Descripción
Análisis de datos realizado sobre una base de datos de libros, autores, editoriales y reseñas, con el objetivo de **extraer información relevante mediante consultas SQL** y proporcionar **insights estratégicos** para el desarrollo de una aplicación dirigida a lectores.
El estudio incluye la conexión segura a la base de datos, ejecución de consultas SQL con Python, análisis exploratorio y generación de conclusiones basadas en tendencias editoriales y de comportamiento de usuarios.

## Objetivos
- Analizar la distribución de publicaciones por año y el impacto de las publicaciones posteriores al año 2000.  
- Calcular el número de reseñas y calificaciones promedio por libro.  
- Identificar las editoriales más activas y los autores mejor valorados.  
- Determinar patrones de comportamiento de los usuarios más participativos.  
- Proporcionar conclusiones útiles para orientar decisiones editoriales o de producto.

## Tecnologías y librerías
- **Python** (pandas, sqlalchemy, python-dotenv, psycopg2-binary).  
- **Jupyter Notebook** (análisis reproducible y documentación visual).  
- **SQL** (consultas ejecutadas sobre base de datos PostgreSQL con conexión SSL).

## Conclusiones
- La mayoría de los libros del catálogo fueron publicados **después del año 2000**, reflejando una orientación hacia literatura moderna.  
- **Penguin Books** es la editorial con mayor número de títulos extensos (>50 páginas).  
- **J.K. Rowling** destaca como la autora mejor calificada (promedio 4.41/5).  
- Un pequeño grupo de usuarios concentra la mayoría de reseñas, representando una oportunidad para estrategias de fidelización o gamificación.  
- El análisis demuestra el valor de combinar **Python + SQL** para obtener información estratégica a partir de bases de datos relacionales.

## Instrucciones de uso
1. Clonar el repositorio:
   ```bash
   git clone https://github.com/tu_usuario/analisis_sql_libros.git
   cd analisis_sql_libros
2. Instalar las dependencias:
    Se recomienda crear un entorno virtual antes de la instalación:
    python -m venv venv
    source venv/bin/activate  # En macOS o Linux
    venv\Scripts\activate     # En Windows

    pip install -r requirements.txt

3. Configurar variables de entorno:
    Crear un archivo .env en la raíz del proyecto. 
    Este archivo almacena las credenciales necesarias para la conexión segura a la base de datos:

    DB_USER=tu_usuario
    DB_PASSWORD=tu_contraseña
    DB_HOST=tu_host
    DB_PORT=tu_puerto
    DB_NAME=tu_base_de_datos

4. Descargar el certificado de conexión segura:

    Descargar el certificado público CA.pem desde el siguiente enlace oficial de Yandex Cloud:

    🔗 https://storage.yandexcloud.net/cloud-certs/CA.pem

    Guárdalo en la siguiente ruta dentro del proyecto:
    data/raw/CA.pem

5. Abrir el notebook principal:

    notebooks/analisis_sql_libros.ipynb

6. Ejecutar las celdas para reproducir el análisis, las consultas SQL y visualizar los resultados.

> Nota: las versiones y dependencias exactas sen encuentran en: `requirements.txt`.