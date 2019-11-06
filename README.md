# Practica Big Data - Visualizacion con Tableau
Este repositorio simplemente contiene el fichero tbwx con el dashboard generado por Daniel Alvaro para la practica de Visualizacion con Tableau del Bootcamp de KeepCoding Big Data & Machine Learning

## Contexto 🌐

Para la realizacion de la practica se ha usado un dataset de Airbnb filtrado para las propiedades en Madrid (14,780 records).
[Dataset Airbnb](https://public.opendatasoft.com/explore/dataset/airbnb-listings)

## Objetivo de nuestra practica 🎯
La plataforma Airbnb distingue entre Anfitriones que son particulares y aquello que son una empresa y se deben dar de alta de manera distinta.

Al ser las condiciones de los particulares mas beneficiosas, se ha detectado un creciente fraude en empresas que se dan de alta como particulares para aprovecharse de ello.

Uno de los objetivos de nuestro analisis sera intentar identificar en que barrrios o zonas de Madrid hay anfitriones con un numero especialmente alto de propiedades en la plataforma que puedan hacernos sospechar que ese Anfitrion se corresponde realmente con una empresa (o con un multimillonario :stuck_out_tongue_winking_eye:)

### Proceso ETL 💾
Para realizar un proceso basico de limpieza y eliminacion de ruido del dataset de Airbnb se llevan a cabo los siguientes filtros desde la Fuente de Datos de Tableau: 
- **City:** Nos quedamos con los que contengan la palabra Madrid
- **Country:** Nos quedamos con los que contengan Spain
- **Country Code:** Nos quedamos con los que contengan ES
- **State:** Nos quedamos con los que contengan Spain, Madrid o España
- **Neighbourhood:** Eliminamos los campos nulos, para evitar ruido cuando tratemos con ellos, ya que este campo sera clave en las hojas y el Dashboard que generaremos.

Una vez llevado a cabo este proceso de limpieza el numero de resgistros con los que vamos a trabaar son: **8.743**

### Jerarquias 🔧

La jerarquias generadas son las siguientes:

- **Jerarquia Geografica:** Country-City-ZipCode
- **Jerarquia Propiedad:** Property Type-Room Type- Bed Type

### Grupos
Para poder trabajar mas comodamente con los datos y dar mayor claridad a las graficas se ha decido agrupar los Barrios(Neghbourhood) por Zonas: Centro, Norte, Sur, Este y Oeste 


## Aclaraciones ✏️



