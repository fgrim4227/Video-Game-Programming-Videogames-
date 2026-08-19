
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

## Requisitos Críticos del Sistema (LEER ANTES DE EJECUTAR)

Para garantizar la correcta ejecución del juego y las físicas, es **estrictamente necesario** cumplir con las siguientes versiones:

*   **Python:** `3.11` o `3.12`. 
    *   >**IMPORTANTE:** No utilizar Python 3.13 o superior. Las versiones más recientes de Python presentan inestabilidad y conflictos graves de compatibilidad al compilar los bindings de C++ de la librería `Box2D`, lo que impedirá la ejecución del juego.

---

## Guía de Instalación y Ejecución Desde Cero

Sigue estos pasos para descargar, configurar y ejecutar el juego de forma segura sin afectar las librerías globales de tu sistema.

### Paso 1: Verificar la versión de Python
Abre una terminal y verifica que tienes una versión compatible instalada:

```bash
python3 --version

```

Si no tienes Python 3.11 o 3.12 instalado:

**En Ubuntu/WSL/Debian:**

```bash
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt update
sudo apt install python3.11 python3.11-venv python3.11-dev
```

**En Windows/macOS:** Descarga el instalador oficial de la versión 3.11.x desde python.org.

## Paso 2: Clonar el repositorio

Descarga el código fuente en tu máquina local:

```bash
git clone https://github.com/fgrim4227/Video-Game-Programming-Videogames-.git
cd Video-Game-Programming-Videogames-

```

## Paso 3: Crear y activar un entorno virtual (Recomendado)

Para evitar conflictos con otras dependencias del sistema, se recomienda aislar el proyecto:

**En Linux / macOS / WSL:**

```bash
python3.11 -m venv venv
source venv/bin/activate

```

**En Windows (Command Prompt / PowerShell):**

```cmd
py -3.11 -m venv venv
venv\Scripts\activate

```

## Paso 4: Instalar las dependencias

Con el entorno virtual activado, instala las librerías necesarias (incluyendo Pygame y Box2D):

```bash
pip install -r requirements.txt

```
*Esto instalara gale sobre el cual trabaja el repositorio*

## Paso 5: Ejecutar el juego

Finalmente, inicia el programa principal:

```bash
python main.py

```

### Controles del Juego

**Navegación del Menú:**

* **Seleccionar modo:** Teclas `W`/`S` o `Flecha Arriba`/`Flecha Abajo`
* **Confirmar:** `Enter`

**Durante el Juego:**

* **Jugador 1 (Paleta Izquierda):** Teclas `W` (Subir) y `S` (Bajar)
* **Jugador 2 (Paleta Derecha):** Teclas `Flecha Arriba` y `Flecha Abajo`
* **Volver al Menú Principal:** La tecla asignada a la acción "menú" (tecla `M`).
* **Cerrar el juego:** Tecla Esc

```

```