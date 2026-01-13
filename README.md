# 🎃 Noche de Halloween - Truco o Trato

![Java](https://img.shields.io/badge/Java-21-orange)
![JavaFX](https://img.shields.io/badge/JavaFX-SDK-blue)
![Build](https://img.shields.io/badge/Build-Maven-green)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey)

Aplicación de escritorio desarrollada en **JavaFX** que simula el clásico juego de "Truco o Trato" mediante una ruleta interactiva. Este proyecto no solo demuestra el desarrollo de la interfaz gráfica, sino también el **ciclo completo de despliegue y distribución** de software en Java.

## 📋 Características

* **Interfaz Gráfica:** Desarrollada con JavaFX y FXML, utilizando CSS personalizado para la temática de terror.
* **Lógica de Juego:** Ruleta animada con resultados aleatorios.
* **Despliegue Profesional:**
    * Generación de **Fat JAR** con todas las dependencias incluidas.
    * Empaquetado en **.exe** nativo de Windows (sin consola).
    * **Instalador completo** con asistente, licencia y accesos directos.

## 🛠️ Tecnologías Utilizadas

* **Lenguaje:** Java 21 (JDK 21).
* **Framework UI:** JavaFX.
* **Gestión de Dependencias:** Maven.
* **Empaquetado JAR:** `maven-shade-plugin`.
* **Wrapper Ejecutable:** Launch4j (Conversión de JAR a EXE).
* **Instalador:** Inno Setup Compiler.

## 🚀 Instalación y Uso

### Descargar el Juego
Puedes descargar el instalador directamente desde la sección de [Releases](#) (si lo subes) o compilarlo tú mismo.

1. Ejecuta el archivo `InstaladorHalloween.exe`.
2. Acepta los términos de la licencia "terrorífica".
3. Sigue los pasos del asistente de instalación.
4. Busca el icono de la calabaza 🎃 en tu escritorio y ¡juega!

## ⚙️ Proceso de Construcción (Build Process)

Este proyecto sigue un flujo de trabajo específico para su distribución:

### 1. Generación del JAR (Maven)
Se utiliza el **Maven Shade Plugin** para crear un ejecutable único que contiene todas las librerías necesarias.
```bash
mvn clean package
Resultado: target/TrucoOTrato-1.0-SNAPSHOT.jar

2. Creación del Ejecutable (Launch4j)
El JAR se envuelve en un contenedor .exe para Windows.

Configuración: Modo GUI (sin consola).

JRE: Configurado para requerir Java 21 (64-bit).

Icono: Personalizado (favicon.ico).

3. Creación del Instalador (Inno Setup)
Se genera el paquete de distribución final InstaladorHalloween.exe que incluye:

El ejecutable del juego.

Imágenes y recursos.

Acuerdo de licencia de usuario final (EULA).

Creación automática de accesos directos y desinstalador en el Panel de Control.

📷 Capturas de Pantalla
(Puedes subir tus imágenes a una carpeta "img" en tu repo y descomentar estas líneas)

✒️ Autor
Virgilio Jesús Domínguez González

Centro: MEDAC

Módulo: Desarrollo de Interfaces

🎃 ¿Truco o Trato?
