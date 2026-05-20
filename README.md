# TravelWorld ✈️ - Vistas declarativas XML

Aplicación Android desarrollada en **Kotlin** como parte de la **Práctica 2 - Vistas declarativas XML**. La app consta de dos pantallas: una pantalla de **Onboarding** que presenta la aplicación al usuario, y una pantalla **Home** que muestra destinos de viaje con tarjetas e iconos de categorías.

![Android](https://img.shields.io/badge/Android-11.0+-green.svg)
![Kotlin](https://img.shields.io/badge/Kotlin-1.9+-purple.svg)
![MinSDK](https://img.shields.io/badge/MinSDK-API%2030%20(Android%2011.0)-blue.svg)
![ViewBinding](https://img.shields.io/badge/ViewBinding-Enabled-orange.svg)

---

## 📱 ¿Qué hace la app?

### Pantalla 1 — Onboarding
- Muestra un **fondo con ola** lila/blanca creado con un vector drawable.
- Presenta el **título** "Tu App de Viajes" y una **descripción** de la aplicación.
- Incluye una **ilustración** central de la app.
- Contiene un **botón "Next"** redondeado que navega a la pantalla Home.
- Al pulsar "Next", la pantalla de Onboarding se cierra definitivamente (el usuario no puede volver atrás con el botón de retroceso).

### Pantalla 2 — Home
- Muestra el título **"Upcoming meetups"**.
- Fila de **4 botones de categoría** con iconos de Material Icons sobre fondos de color:
  - 📷 Cámara (azul claro)
  - ❤️ Corazón (morado claro)
  - ⛰️ Montañas (rosa claro)
  - 🙂 Smiley (amarillo claro)
- **2 tarjetas de destino** desplazables con imagen, ubicación y título:
  - **City of Los Angeles** — USA, Los Angeles - 2 Weeks
  - **Beach vacation** — Maldivas - 3 weeks
- Las tarjetas son accesibles mediante **scroll** con `NestedScrollView`.

---

## 📸 Capturas de pantalla

| Onboarding | Home (parte superior) | Home (completo) |
|:----------:|:---------------------:|:---------------:|
| <img width="352" height="772" alt="image" src="https://i.ibb.co/4Z4vxNBn/Onboarding.png" /> | <img width="500" height="800" alt="image" src="https://i.ibb.co/TDgZygvV/Home-parte-superior.jpg" /> | <img width="352" height="772" alt="image" src="https://i.ibb.co/FbLndRqj/Home-completo.png" /> |

---

## 🛠️ Tecnologías y requisitos

| Concepto | Detalle |
|----------|---------|
| **Lenguaje** | Kotlin |
| **IDE** | Android Studio (Ladybug \| 2024.2.1 o superior) |
| **SDK mínimo** | API 30 (Android 11.0) |
| **SDK destino** | API 37 |
| **ViewBinding** | Activado |
| **UI Components** | ConstraintLayout, LinearLayout, NestedScrollView |
| **Material Design** | MaterialCardView, Material Button |
| **Iconos** | Vector Drawables (Material Icons) |
| **Navegación** | Intent entre Activities |

---

## ⚙️ ¿Cómo ejecutarlo?

Sigue estos pasos para probar la aplicación en tu equipo:

```bash
# 1. Clona el repositorio
git clone https://github.com/douglasvelezv/vistas-declarativas_xml.git

# 2. Abre Android Studio y selecciona "Open an Existing Project"
#    (elige la carpeta donde clonaste el repositorio)

# 3. Espera a que Gradle termine de sincronizar las dependencias

# 4. Conecta un dispositivo físico (con depuración USB activada)
#    o inicia un emulador con API 30 o superior

# 5. Pulsa el botón verde "Run" (►) y listo
```

---

## 📂 Estructura del proyecto

```
es.travelworld.traveling/
├── app/
│   └── src/
│       └── main/
│           ├── java/es/travelworld/traveling/
│           │   ├── MainActivity.kt              # Pantalla Onboarding + navegación al Home
│           │   └── HomeActivity.kt              # Pantalla Home
│           ├── res/
│           │   ├── layout/
│           │   │   ├── activity_onboarding.xml  # UI del Onboarding
│           │   │   └── activity_home.xml        # UI del Home (iconos + cards)
│           │   ├── drawable/
│           │   │   ├── background_onboarding.xml  # Fondo vectorial con ola
│           │   │   ├── ic_camera.xml              # Icono cámara
│           │   │   ├── ic_heart.xml               # Icono corazón
│           │   │   ├── ic_mountains.xml           # Icono montañas
│           │   │   ├── ic_smiley.xml              # Icono smiley
│           │   │   ├── nomads_moto.png            # Ilustración Onboarding
│           │   │   ├── image_container1.png       # Imagen Card 1 (Los Angeles)
│           │   │   └── image_container2.png       # Imagen Card 2 (Maldivas)
│           │   └── values/
│           │       ├── strings.xml                # Textos de la app
│           │       ├── colors.xml                 # Paleta de colores
│           │       └── themes.xml                 # Tema Material Components
│           └── AndroidManifest.xml                # Declaración de Activities
```

---

## Este repositorio ha sido creado siguiendo las instrucciones de la práctica:

✅ Desarrollado con Android Studio.

✅ 2 Historias de usuario implementadas: **Onboarding** y **Home**.

✅ 4 botones de categoría con iconos (Material Icons).

✅ 2 tarjetas de destino construidas con `MaterialCardView`.

✅ Navegación entre pantallas con `Intent` y `ViewBinding`.

✅ Entregado mediante GitHub (enlace del proyecto).

🔗 https://github.com/douglasvelezv/vistas-declarativas_xml

---

## 📄 Licencia

Este proyecto es solo para fines educativos. Puedes usarlo libremente como base para tus propios aprendizajes.
