# DescargarYT
Utilidad para descargar audio video y listas de reproduccion de youtube

# 🚀 Descargador de YouTube y derivados.

Una herramienta interactiva para la terminal de Linux que automatiza la descarga de videos y listas de reproducción de YouTube y derivados con menús visuales. Diseñado para ser rápido, eficiente y evitar el uso de comandos largos de memoria.

Diseñado originalmente por **SUKIGSX**.

---

## ✨ Características

- 🎯 **Menús interactivos:** Selección visual utilizando `fzf` (navegación con flechas del teclado).
- 📦 **Detección de listas de reproducción:** Identifica automáticamente si la URL es una playlist y te permite elegir entre bajar todo o solo el video individual.
- 🎬 **Múltiples formatos:** 
  - **Video:** Máxima calidad disponible empaquetada en `.mp4`.
  - **Audio:** Extracción directa a `.mp3` de alta calidad (320kbps).
  - **Ambos:** Descarga el video y extrae el audio de forma local sin consumir doble ancho de banda.
- 📁 **Gestión inteligente de carpetas:**
  - Opción de guardar en una subcarpeta automática llamada `DescargasYT/`.
  - Opción de ingresar una ruta absoluta personalizada.
  - Creación automática de directorios si no existen.
  - Organización automática de listas de reproducción en subcarpetas numeradas.

---

## 🛠️ Requisitos del Sistema

El script utiliza herramientas nativas de Linux. Asegúrate de tener instaladas las siguientes dependencias antes de ejecutarlo:

1. **`yt-dlp`**: El motor de descarga multimedia.
2. **`fzf`**: El buscador interactivo para los menús de la terminal.
3. **`ffmpeg`**: El procesador multimedia para fusionar pistas y convertir a MP3.

### 💻 Instalación de dependencias

**En Arch Linux / Manjaro / EndeavourOS:**
```bash
sudo pacman -S yt-dlp fzf ffmpeg
```

**En Linux Mint / Ubuntu / Debian:**
```bash
sudo apt update && sudo apt install yt-dlp fzf ffmpeg
```

---

## 🚀 Instalación y Uso

1. **Clona este repositorio o descarga el script:**
   ```bash
   git clone https://github.com/sukigsx/DescargarYT.git
   cd DescargarYT
   ```

2. **Dale permisos de ejecución al archivo:**
   ```bash
   chmod +x DescargarYT.sh
   ```

3. **Ejecuta el script:**
   ```bash
   ./DescargarYT.sh
   ```

---

## 💡 Nota sobre actualizaciones

YouTube actualiza su plataforma constantemente, lo que puede romper el funcionamiento de las descargas de vez en cuando. Si el script falla al procesar una URL, actualiza el motor principal ejecutando:

```bash
sudo yt-dlp -U
```
