# Proyecto P00 - Gestión de Contenidos Audiovisuales  
**Universidad Politécnica Salesiana**  
*Programación Orientada a Objetos - Unidad 2*
*Estudiante Evelyn Daniela Dominguez Dominguez*

## Descripción del Proyecto
Sistema Java que modela diferentes tipos de contenido audiovisual (películas, series, documentales, cortometrajes y videos digitales) utilizando **Programación Orientada a Objetos**. Implementa:
- **Herencia** y **clases abstractas**.
- **Relaciones** (asociación, composición).
- **Polimorfismo** mediante métodos sobrescritos.

## Estructura del Proyecto
src/
├── poo/
│   ├── Main.java            # Punto de entrada
│   └── PruebaAudioVisual.java
└── uni1a/
    ├── ContenidoAudiovisual.java
    ├── Pelicula.java
    ├── SerieDeTV.java
    ├── Documental.java
    ├── Cortometraje.java    # Nueva subclase
    ├── VideoYouTube.java    # Nueva subclase
    ├── Actor.java
    ├── Temporada.java
    └── Investigador.java
    
### Problema que resuelve
Organiza y gestiona información de producciones audiovisuales con sus componentes clave (actores, temporadas, investigadores), ideal para estudios de cine o plataformas de streaming.

## Características Principales
- **Clases implementadas**:
  - Base: `ContenidoAudiovisual` (abstracta).
  - Contenido: `Pelicula`, `SerieDeTV`, `Documental`, `Cortometraje`, `VideoYouTube`.
  - Relaciones: `Actor`, `Temporada`, `Investigador`.
- **Funcionalidades**:
  - Creación y asociación de objetos.
  - Visualización estructurada de detalles.

## Instalación y Ejecución

### Requisitos
- Git (opcional)
- Eclipse/IDE compatible 

### Pasos para clonar y ejecutar
1. **Clonar repositorio**:
   ```bash
   git clone https://github.com/tu-usuario/poo_unidad1.git
   cd poo_unidad1

## Instrucciones de Uso  

  Guía de Clonación y Ejecución del Proyecto POO

## Pasos para Clonar y Ejecutar (como lo hicimos en Eclipse)

### 1. Clonar el repositorio
```bash
git clone https://github.com/CS-Programacion-Orientada-Objetos/poo_unidad1.git
cd poo_unidad1
### 2. Importar en Eclipse
Abre Eclipse y selecciona:

File > Import > Git > Projects from Git

Elige "Clone URI" y pega esta URL:

text
https://github.com/CS-Programacion-Orientada-Objetos/poo_unidad1.git
Sigue el asistente:

En Branch Selection: Marca main o master

En Local Destination: Elige tu carpeta de workspace

### 3. Configurar el proyecto
Si Eclipse no reconoce el proyecto como Java:

Haz clic derecho en el proyecto > Configure > Convert to Java Project

Verifica el JDK:

Click derecho en proyecto > Build Path > Configure Build Path

En la pestaña Libraries: Asegúrate de tener JRE System Library [JavaSE-17]

### 4. Ejecutar las pruebas
