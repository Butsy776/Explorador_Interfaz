# Explorador de Archivos en Google Drive

Es un buscador interactivo desarrollado en **Python** para entornos de **Google Colab**, diseñado para la gestión, análisis, filtrado y ordenamiento eficiente de archivos y metadatos alojados en un directorio específico de Google Drive.

---

## Características Principales

* **Algoritmo QuickSort Personalizado:** Implementación propia del algoritmo de ordenamiento rápido (*QuickSort*) desde cero para ordenar los archivos por nombre, tamaño (KB) o fecha de última modificación de manera eficiente.
* **Soporte Multiformato:** Capacidad de procesar y categorizar diversos tipos de archivos comunes (`.json`, `.csv`, `.pdf`, `.txt`, `.docx`, `.xlsx`).
* **Interfaz Interactiva Nativa (`ipywidgets`):** Construido con widgets de Jupyter/Colab para ofrecer una experiencia fluida, con menús desplegables estrictos (sin edición manual de texto) y actualizaciones en tiempo real.
* **Métricas en Vivo:** Panel superior con contador dinámico de elementos encontrados tras aplicar los filtros de búsqueda.

---

## Tecnologías y Librerías Utilizadas

* **Python 3**
* **Google Colab & Google Drive API** (`google.colab.drive`)
* **`ipywidgets`** (Para los componentes de la interfaz de usuario interactiva)
* **Librerías nativas de Python:** `os`, `json`, `datetime`, `unicodedata`

---

## Estructura del Proyecto

1. **Montaje del entorno:** Conexión segura con Google Drive para acceder al directorio de trabajo (`/content/drive/My Drive/LPII_2026`).
2. **Procesamiento de datos:** Exploración del directorio, extracción de metadatos (tamaño, marcas de tiempo de modificación) y validación de extensiones permitidas.
3. **Motor de ordenamiento:** Lógica de particionamiento y recursividad de *QuickSort*.
4. **Capa visual (UX/UI):** Inyección de estilos CSS personalizados e integración de componentes de control mediante `ipywidgets`.

---

## Instrucciones de Uso

1. Abre el cuaderno en Google Colab haciendo clic en el botón superior de *Open in Colab*.
2. Asegúrate de tener la carpeta configurada en tu Google Drive bajo la ruta `LPII_2026`.
3. Ejecuta todas las celdas del cuaderno.
4. Utiliza el buscador por nombre, los menús desplegables de extensión y ordenamiento, y haz clic en **"FILTRAR"** para interactuar con tus archivos.
