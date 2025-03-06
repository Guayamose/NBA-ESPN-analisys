# Comparador de Estadísticas de Equipos de NBA

<p align="center">
  <img src="https://img.shields.io/badge/Status-EN%20DESARROLLO-yellow" alt="Status" />
  <img src="https://img.shields.io/badge/Python-3.x-blue" alt="Python Version" />
  <img src="https://img.shields.io/badge/BeautifulSoup-4.x-blue" alt="BeautifulSoup Version" />
  <img src="https://img.shields.io/badge/Rich-Latest-blue" alt="Rich Version" />
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

Este proyecto es una herramienta en Python que permite comparar las estadísticas de dos equipos de la NBA. Se extraen datos de HTML obtenidos de la web de ESPN (estadísticas propias y de oponentes) y se realizan dos tipos de análisis:

1. **Comparación Individual:** Se contrasta cada estadística (por ejemplo, puntos, rebotes, asistencias, etc.) mostrando la diferencia absoluta y relativa entre lo que produce el equipo y lo que permite el rival.
2. **Comparación por Áreas de Juego:** Se agrupan las estadísticas en áreas (Disparo, Tiros de 3, Tiros libres, Rebotes, Juego de pases y Defensa) y se genera una diferencia relativa promedio, acompañada de una narrativa interpretativa que sugiere cómo se podrían desarrollar las interacciones durante el partido.

La salida se presenta de forma visual y estructurada utilizando la biblioteca **Rich**, lo que facilita la interpretación de las diferencias y la comprensión de la dinámica de juego sin enfocarse en predecir ganadores.

## Características

- **Comparación Individual Detallada:** Muestra cada estadística con valores numéricos, diferencia absoluta y diferencia relativa, resaltados en verde (favorable) o rojo (desfavorable).
- **Análisis por Áreas de Juego:** Agrupa las estadísticas en categorías y ofrece un análisis narrativo sobre las áreas clave de interacción (por ejemplo, disparo, rebotes, defensa).
- **Salida Visual Mejorada:** Utiliza la biblioteca Rich para generar tablas, paneles y mensajes con colores en la terminal, haciendo el output más atractivo y fácil de interpretar.
- **Procesamiento de HTML:** Extrae y organiza datos de HTML de ESPN mediante BeautifulSoup, integrando estadísticas propias y de oponentes.
- **Interfaz Interactiva:** Permite la selección de equipos con validación insensible a mayúsculas.

## Requisitos

- **Python 3.x**
- **BeautifulSoup (bs4)**
- **Rich**

Instala las dependencias con:
```bash
pip install beautifulsoup4 rich
```

# Instalación y Ejecución

## Clona el Repositorio
```bash
git clone https://github.com/tu_usuario/tu_repositorio.git
```

## Instala las Dependencias
Abre una terminal y ejecuta:
```bash
pip install beautifulsoup4 rich
```

## Configura el HTML
Asegúrate de tener definidas las variables \`html_propias\` y \`html_oponentes\` con el código HTML obtenido de las tablas de ESPN.

## Ejecuta el Programa
Navega al directorio del proyecto y ejecuta:
```bash
python main.py
```

# Uso

El programa procesa los datos de estadísticas propias y de oponentes, y luego solicita al usuario que seleccione dos equipos. Se generan dos análisis:

- **Individual:** Comparación de cada estadística (valor del equipo vs. lo que permite el rival), mostrando diferencias absolutas y relativas con resaltado en colores.
- **Por Áreas de Juego:** Agrupa las estadísticas en áreas clave y calcula la diferencia relativa promedio en cada grupo, acompañada de una breve narrativa interpretativa sobre la interacción entre equipos.

Esta información te ayudará a comprender cómo podrían interactuar los equipos durante el partido en distintas áreas (por ejemplo, circulación de balón, rebotes, eficacia en tiro, etc.), sin enfocarse en predecir el resultado del juego.

# Lógica del Programa

## Carga y Procesamiento del HTML
Se definen las variables \`html_propias\` y \`html_oponentes\` con el HTML obtenido de ESPN. Con BeautifulSoup se extraen los nombres de los equipos y las estadísticas, organizándolas en diccionarios.

## Comparación de Estadísticas
- **Individual:** Se compara cada estadística y se calcula la diferencia absoluta y relativa (porcentaje) entre lo que produce el equipo y lo que permite el rival.
- **Por Áreas de Juego:** Se agrupan las estadísticas en categorías (Disparo, Tiros de 3, Tiros libres, Rebotes, Juego de pases y Defensa) y se calcula la diferencia relativa promedio, generando un resumen narrativo.

## Salida Visual Mejorada
La biblioteca **Rich** se utiliza para mostrar tablas y paneles en la terminal, haciendo el output más atractivo y fácil de interpretar.

## Interacción con el Usuario
El usuario selecciona dos equipos de una lista y se muestran los análisis comparativos en la terminal.

# Contribuciones
Las contribuciones son bienvenidas. Si deseas mejorar o ampliar el proyecto, por favor abre un issue o envía un pull request.

# Tecnologías
- Python 3.x
- BeautifulSoup4
- Rich

# Licencia
Uso Comercial con Permiso. Consulta el archivo de licencia para más detalles.

# Autores
- Rafael Pradillo Lopez-Ortum

# Contacto
Para consultas o sugerencias, contacta a [rafapradillo78@gmail.com](mailto:rafapradillo78@gmail.com)
