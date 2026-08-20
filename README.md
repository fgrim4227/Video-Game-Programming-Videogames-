```markdown
# Pong AI - Video Game Programming I

Este proyecto es una implementación avanzada del clásico juego Pong, desarrollada como parte de la asignatura de Programación de Videojuegos. 

**Créditos del Código Base:** Este repositorio toma como punto de partida el motor y la estructura original provistos por el profesor e ingeniero en el repositorio del curso: [R3mmurd/VideoGameProgrammingI](https://github.com/R3mmurd/VideoGameProgrammingI).

---

## Características Implementadas

*   **Inteligencia Artificial Predictiva:** Las paletas controladas por la IA no solo siguen la pelota, sino que calculan geométricamente el punto de impacto futuro tomando en cuenta los rebotes en el techo y el piso.
*   **Múltiples Modos de Juego:** 
*   2 Jugadores (Local)
*   1 Jugador vs IA
*   IA vs IA (Modo demostración/espectador)
*   **Detección de Colisión Continua (CCD):** Se reemplazó la detección de colisiones discreta nativa por un sistema de interpolación lineal matemática para eliminar el "efecto túnel" (tunneling) cuando la pelota alcanza altas velocidades.

---

## Requisitos del Sistema

Para garantizar la correcta ejecución del juego, necesitas cumplir con los siguientes requisitos:

*   **Python:** `3.11` o superior (Totalmente compatible con las versiones más recientes).
*   **Git:** Para clonar el repositorio en tu máquina local.

---

## Guía de Instalación y Ejecución Desde Cero

Sigue estos pasos para descargar, configurar y ejecutar el juego de forma segura utilizando un entorno virtual.

### Paso 1: Verificar o Instalar Python
Abre una terminal y verifica que tienes una versión de Python instalada:

```bash
python3 --version

```

Si no tienes Python instalado en tu sistema, sigue las instrucciones según tu plataforma:

**En Ubuntu/WSL/Debian:**

```bash
sudo apt update
sudo apt install python3 python3-venv python3-dev

```

**En Windows/macOS:** Descarga el instalador oficial de la versión más reciente desde python.org.

### Paso 2: Clonar el repositorio

Descarga el código fuente en tu máquina local:

```bash
git clone [https://github.com/fgrim4227/Video-Game-Programming-Videogames-.git](https://github.com/fgrim4227/Video-Game-Programming-Videogames-.git)
cd Video-Game-Programming-Videogames-

```

### Paso 3: Crear y activar un entorno virtual (Recomendado)

Para evitar conflictos con otras dependencias del sistema, se recomienda aislar el proyecto:

**En Linux / macOS / WSL:**

```bash
python3 -m venv venv
source venv/bin/activate

```

**En Windows (Command Prompt / PowerShell):**

```cmd
py -m venv venv
venv\Scripts\activate

```

### Paso 4: Instalar las dependencias

Con el entorno virtual activado, instala las librerías necesarias ejecutando el archivo de requerimientos:

```bash
pip install -r requirements.txt

```

*Nota: Esto instalará el motor `gale`, el cual se encargará de descargar y configurar automáticamente todas las dependencias internas necesarias.*

### Paso 5: Ejecutar el juego

Finalmente, inicia el programa principal:

```bash
python main.py

```

---

## Controles del Juego

**Navegación del Menú:**

* **Seleccionar modo:** Teclas `W`/`S` o `Flecha Arriba`/`Flecha Abajo`
* **Confirmar:** `Enter`

**Durante el Juego:**

* **Jugador 1 (Paleta Izquierda):** Teclas `W` (Subir) y `S` (Bajar)
* **Jugador 2 (Paleta Derecha):** Teclas `Flecha Arriba` y `Flecha Abajo`
* **Volver al Menú Principal:** Tecla `M`
* **Cerrar el juego:** Tecla `Esc`

```

```