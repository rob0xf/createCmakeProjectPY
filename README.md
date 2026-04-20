# 🛠️ createCmakeProjectPY

<p align="center">
  <b>Generador automático de proyectos en C con CMake</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue">
  <img src="https://img.shields.io/badge/CMake-required-green">
  <img src="https://img.shields.io/badge/Platform-Linux%20%7C%20Windows%20%7C%20Termux-lightgrey">
</p>

---

## 📦 Requisitos

### 🐍 Python

* Python 3.8 o superior

```bash
python --version
```

---

## ⚙️ Instalación de CMake

<details>
<summary><b>🐧 Linux</b></summary>

### Debian / Ubuntu / Kali

```bash
sudo apt update && sudo apt install cmake
```

### Arch / Manjaro

```bash
sudo pacman -S cmake
```

### Fedora

```bash
sudo dnf install cmake
```

### Termux

```bash
pkg install cmake
```

</details>

---

<details>
<summary><b>🪟 Windows</b></summary>

Descargar desde el sitio oficial:

https://cmake.org/download/

✔ Durante la instalación:

* Activa **"Add CMake to system PATH"**

</details>

---

<details>
<summary><b>🍎 macOS</b></summary>

```bash
brew install cmake
```

</details>

---

## Uso

```bash
./ckpjt NombreProyecto .
```

---

## 📁 Estructura generada

```bash
NombreProyecto/
├── CMakeLists.txt
├── build/
├── include/
└── src/
    └── main.c
```

---

## 🔧 Compilación

```bash
cd NombreProyecto
cmake -S . -B build
cmake --build build
```

---

## ▶️ Ejecución

### Linux / macOS / Termux

```bash
./build/app
```

### Windows

```bash
.\build\app.exe
```

---
## ⚠️ Notas importantes

### 🪟 Windows

* Necesitas un compilador:

  * Visual Studio (MSVC)
  * MinGW
  * Ninja + Clang

Ejemplo con MinGW:

```bash
cmake -S . -B build -G "MinGW Makefiles"
cmake --build build
```
## Roadmap
* Soporte para C++
* Templates personalizados
---

## 👨‍💻 Autor r0b0xf

Proyecto diseñado para automatizar la creación de proyectos en C con CMake.
