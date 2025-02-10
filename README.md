# Hola Mundo con PySide6

Este repositorio contiene una aplicación simple de "Hola Mundo" utilizando PySide6. A continuación, se presentan los pasos para instalar y ejecutar la aplicación en Windows y Linux.

## Requisitos Previos

Antes de comenzar, asegúrate de tener instalado:

- [Python 3](https://www.python.org/downloads/)
- pip (normalmente incluido con Python)

## Instalación y Configuración

### 1. Verificar la Instalación de Python y pip

Ejecuta los siguientes comandos para verificar que Python y `pip` están instalados:

```sh
python --version
pip --version
```

Si estos comandos no funcionan, intenta con:

```sh
python3 --version
pip3 --version
```

### 2. Crear y Activar un Entorno Virtual

Es recomendable usar un entorno virtual para gestionar las dependencias.

#### En Windows

```sh
python -m venv venv
venv\Scripts\activate
```

#### En Linux

```sh
python3 -m venv venv
source venv/bin/activate
```

### 3. Instalar Dependencias

Una vez activado el entorno virtual, instala las dependencias necesarias:

```sh
pip install PySide6
```

### 4. Crear el Archivo de la Aplicación

Crea un archivo `app.py` en el mismo directorio y agrega el siguiente código:

```python
import sys
from PySide6.QtWidgets import QApplication, QLabel

app = QApplication(sys.argv)
label = QLabel("¡Hola, Mundo!")
label.show()
app.exec()
```

### 5. Ejecutar la Aplicación

Ejecuta el siguiente comando según tu sistema operativo:

#### En Windows

```sh
python app.py
```

#### En Linux

```sh
python3 app.py
```

Si todo está configurado correctamente, debería aparecer una ventana con el mensaje "¡Hola, Mundo!".

## Créditos

Este proyecto fue creado como parte de una actividad de documentación con Markdown.

## Licencia

Este proyecto está bajo la licencia MIT.
