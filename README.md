# Comparador de Estadísticas de Equipos de NBA



<p align="center">
  <img src="https://img.shields.io/badge/Status-EN%20DESARROLLO-yellow" alt="Status" />
  <img src="https://img.shields.io/badge/Python-3.x-blue" alt="Python Version" />
  <img src="https://img.shields.io/badge/BeautifulSoup-4.x-blue" alt="BeautifulSoup Version" />
  <img src="https://img.shields.io/badge/Licencia-Uso%20Comercial%20con%20Permiso-red" alt="Licencia Propietaria" />
</p>

## Índice
- [Descripción del Proyecto](#descripción-del-proyecto)
- [Características](#características)
- [Requisitos](#requisitos)
- [Instalación y Ejecución](#instalación-y-ejecución)
- [Uso](#uso)
- [Lógica del Programa](#lógica-del-programa)
- [Contribuciones](#contribuciones)
- [Tecnologías](#tecnologías)
- [Licencia](#licencia)
- [Autores](#autores)
- [Contacto](#contacto)

## Descripción del Proyecto

Este proyecto es una herramienta en Python que permite comparar las estadísticas de dos equipos de la NBA. Utilizando datos extraídos directamente de la web de ESPN, el programa contrasta:

- **Estadísticas Propias:** Métricas propias del equipo (puntos, rebotes, asistencias, etc.).
- **Estadísticas de Oponentes:** Datos sobre lo que los rivales suelen conseguir contra el equipo.

La salida muestra cada estadística con su nombre completo y resalta las diferencias mediante colores:
- **Verde:** Diferencia positiva (favorable, por ejemplo, si el equipo anota más de lo que el rival permite).
- **Rojo:** Diferencia negativa (desfavorable, por ejemplo, si el rival permite menos puntos de los que el equipo suele anotar).

## Características

- **Comparación Detallada:** Contrasta estadísticas propias y de oponentes.
- **Visualización en Colores:** Resalta diferencias positivas y negativas.
- **Integración Sencilla:** Extrae datos a partir del HTML de ESPN.
- **Flexible:** Permite ajustar las variables para comparar distintos equipos.

## Requisitos

- **Python 3.x**
- **BeautifulSoup (bs4)**  
  Instálalo con:
  ```bash
  pip install beautifulsoup4


# Instalación y Ejecución

## Clona el Repositorio:
```bash
git clone https://github.com/tu_usuario/tu_repositorio.git
```

## Instala las Dependencias:
Abre una terminal y ejecuta:
```bash
pip install beautifulsoup4
```

## Configura el HTML (Opcional):
Si obtienes datos de ESPN u otra fuente, puedes pegarlos en el archivo principal para procesarlos.

## Ejecuta el Programa:
Navega al directorio del proyecto y ejecuta:
```bash
python main.py
```

# Uso

El programa procesa el HTML de las tablas, extrae las estadísticas y muestra una comparación en la terminal (o en una interfaz, según la implementación). Los resultados se resaltarán en:

- **Verde:** Cuando la diferencia sea favorable.
- **Rojo:** Cuando la diferencia sea desfavorable.

# Lógica del Programa

El objetivo principal del programa es comparar las estadísticas de dos equipos (o de un equipo contra sus oponentes) utilizando datos extraídos de las tablas HTML de ESPN. A continuación se describe la lógica general:

## Carga del HTML:
Se definen dos variables (por ejemplo, `html_propias` y `html_oponentes`) donde se debe pegar el código HTML obtenido de las tablas de ESPN.

## Procesamiento con BeautifulSoup:
Se utiliza la librería `BeautifulSoup` para parsear el HTML y extraer la información. El programa recorre los elementos de la tabla (usualmente `<tr>` para filas y `<td>` para celdas) para obtener las estadísticas y sus valores.

## Extracción y Organización de Datos:
Los datos se organizan en estructuras de datos como diccionarios o listas, donde cada estadística (por ejemplo, puntos, rebotes, asistencias) se asocia con su valor numérico.

## Comparación de Estadísticas:
Se comparan las estadísticas extraídas de la tabla de estadísticas propias con las de la tabla de estadísticas de oponentes:
- Si la diferencia es favorable (por ejemplo, si el equipo anota más de lo que el rival permite), se resalta en **verde**.
- Si la diferencia es desfavorable (por ejemplo, si el rival permite menos puntos de los que el equipo anota), se resalta en **rojo**.

## Salida de Resultados:
El programa muestra en la terminal una lista o tabla con cada estadística y la diferencia calculada, utilizando códigos ANSI (u otra librería) para resaltar en **verde** o **rojo** según corresponda.

## Extensibilidad:
Se pueden agregar funcionalidades adicionales, como exportar resultados a un archivo o integrarlo en una interfaz gráfica.
```

