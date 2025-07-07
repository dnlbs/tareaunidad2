# 📽️ Proyecto P00 - Gestión de Contenidos Audiovisuales  
**Universidad Politécnica Salesiana**  
*Programación Orientada a Objetos - Unidad 2*
*Estudiante Evelyn Daniela Dominguez Dominguez*

---

## 📌 Descripción  
Sistema de gestión para contenidos audiovisuales (series, películas, documentales) con relaciones de composición y asociación, implementado en Java.  
**Extensión personal**: Se añadieron las subclases `VideoYouTube` y `Cortometraje` (Etapa 4).

---

## 🏗️ Estructura de Clases  

### Clases Base  
- `ContenidoAudiovisual` (clase abstracta)  
  - Atributos: `titulo`, `duracion`, `rating`  
  - Métodos: `calcularRatingPromedio()`  

### Clases de Contenido Principal  
- `SerieDeTV` (extiende `ContenidoAudiovisual`)  
  - Relación: **Composición** con `Temporada`  
  - Métodos: `agregarTemporada()`, `listarCapítulos()`  
- `Pelicula` (extiende `ContenidoAudiovisual`)  
  - Relación: **Asociación** con `Actor`  
- `Documental` (extiende `ContenidoAudiovisual`)  
  - Relación: **Asociación** con `Investigador`  

### Subclases Nuevas (Mi Implementación)  
- `VideoYouTube` (extiende `ContenidoAudiovisual`)  
  - Atributos únicos: `canal`, `likes`  
  - Métodos: `darLike()`, `generarEnlace()`  
- `Cortometraje` (extiende `ContenidoAudiovisual`)  
  - Atributos únicos: `festival`, `esAnimacion`  
  - Métodos: `esPremiado()`  

### Clases de Relación  
- `Actor` → Asociación con `Pelicula`  
- `Temporada` → Composición con `SerieDeTV`  
- `Investigador` → Asociación con `Documental`  

---

## 🔗 Relaciones Implementadas  

| Relación                | Tipo          | Descripción                                  |
|-------------------------|---------------|---------------------------------------------|
| `Actor` ↔ `Pelicula`    | Asociación    | Actores participan en múltiples películas.  |
| `Temporada` → `SerieDeTV`| Composición   | Temporadas no existen sin la serie.         |
| `Investigador` ↔ `Documental`| Asociación | Investigadores colaboran en documentales.   |

---

## 🚀 Instrucciones de Uso  

1. **Clonar el repositorio**:  
   ```bash
   git clone https://github.com/tu-usuario/proyecto-series-java.git
