# 🎮 Mixamo Animation Viewer con Three.js

## 📌 Descripción del Proyecto

Este proyecto consiste en una aplicación web interactiva desarrollada con **Three.js**, que permite visualizar un modelo 3D animado utilizando múltiples animaciones provenientes de Mixamo.

El usuario puede cambiar entre diferentes movimientos del personaje mediante el teclado o botones en pantalla, con transiciones suaves entre animaciones.

---

## 🎯 Objetivos

* Integrar modelos 3D con animaciones en una página web
* Utilizar Three.js para renderizado en tiempo real
* Implementar control de animaciones mediante teclado
* Aplicar transiciones suaves entre movimientos
* Diseñar una interfaz moderna con efecto *glassmorphism*

---

## 🧰 Tecnologías utilizadas

* JavaScript (ES Modules)
* Three.js
* FBXLoader
* HTML5
* CSS3 (Glassmorphism)
* Bootstrap 5

---

## 📁 Estructura del Proyecto

```
assets/
│
├── build/              # Librerías Three.js
├── css/
│   └── main.css        # Estilos (glassmorphism)
│
├── js/
│   ├── main.js         # Escena principal
│   └── animacion.js    # Control de animaciones
│
├── jsm/                # Addons de Three.js
│
└── models/
    └── fbx/
        ├── character.fbx
        ├── Crouch To Stand.fbx
        ├── Taunt.fbx
        ├── Mma Kick.fbx
        ├── Fall flat.fbx
        └── Breakdance 1990.fbx

index.html
README.md
```

---

## ⚙️ Instalación y ejecución

### 1. Clonar o descargar el proyecto

```
git clone <url-del-repositorio>
```

---

### 2. Abrir con servidor local

Es necesario usar un servidor para evitar errores de carga:

* Usar extensión **Live Server** en VS Code
* O ejecutar un servidor local

---

### 3. Ejecutar

Abrir:

```
index.html
```

---

## 🎮 Controles

| Tecla | Acción          |
| ----- | --------------- |
| 1     | Crouch To Stand |
| 2     | Taunt           |
| 3     | MMA Kick        |
| 4     | Fall Flat       |
| 5     | Breakdance 1990 |

También puedes usar los botones en pantalla.

---

## 🎥 Funcionamiento

1. Se carga el modelo base (`character.fbx`)
2. Se cargan animaciones externas (sin skin)
3. Se crea un `AnimationMixer`
4. Cada animación se asigna a una tecla
5. Se aplican transiciones suaves (`fadeIn / fadeOut`)

---

## 🎨 Interfaz

La interfaz utiliza un diseño moderno con efecto **glassmorphism**, incluyendo:

* Navbar superior
* Panel de controles flotante
* Botones interactivos
* Footer informativo

---

## ⚠️ Problemas comunes

### ❌ Animaciones no cargan

* Verificar rutas (`./assets/models/fbx/`)
* Verificar nombres exactos de archivos

### ❌ Teclas no funcionan

* Asegurarse de que las animaciones terminaron de cargar
* Usar teclas numéricas superiores (no numpad)

### ❌ Modelo no visible

* Ajustar escala del modelo
* Ajustar posición de la cámara

---

## 🚀 Posibles mejoras

* Movimiento del personaje con teclado (WASD)
* Sistema de cámara dinámica
* Interfaz tipo videojuego
* Carga de modelos GLTF (más optimizado)
* Sistema de estados de animación

---

## 👨‍💻 Autor

**Jean Samuel Laroque**

Proyecto académico utilizando Three.js y animaciones de Mixamo.

---

## 📄 Licencia

Este proyecto es de uso educativo.
Las animaciones pertenecen a Mixamo (Adobe).
