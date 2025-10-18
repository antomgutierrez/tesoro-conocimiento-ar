# 🧭 El Tesoro del Conocimiento - AR UCU

Un juego de búsqueda del tesoro en Realidad Aumentada ambientado en el Edificio Sacré Coeur de la Universidad Católica del Uruguay.

## 🎯 Descripción del Juego

Los jugadores deben encontrar el "Tesoro del Conocimiento" perdido en el Edificio Sacré Coeur. Este tesoro representa la sabiduría acumulada desde 1925, cuando las monjas del Sagrado Corazón fundaron la institución educativa.

### 🗺️ Ruta del Juego (Secuencial)

1. **🏛️ Recepción** - Punto de inicio con la historia del edificio
2. **🎓 Aula Magna** - Pista sobre la importancia del aprendizaje
3. **🍽️ Cantina** - Pista sobre la comunidad estudiantil
4. **🌳 Patio** - Pista sobre el espacio de encuentro al aire libre
5. **📚 Biblioteca** - Tesoro final del conocimiento

## 🚀 Cómo Jugar

1. **Accede al juego**: Abre `index.html` en tu navegador móvil
2. **Permite el acceso a la cámara** cuando se solicite
3. **Imprime los marcadores** desde la carpeta `markers/`
4. **Coloca los marcadores** en las ubicaciones correspondientes del edificio
5. **Escanea cada marcador** en orden secuencial
6. **¡Encuentra el tesoro!** en la biblioteca

## 📱 Requisitos Técnicos

- **Navegador**: Chrome, Firefox, Safari (versiones recientes)
- **Dispositivo**: Móvil o tablet con cámara
- **Conexión**: Internet para cargar las librerías AR.js y A-Frame
- **Marcadores**: Archivos impresos en papel (tamaño recomendado: 10x10 cm)

## 🛠️ Instalación y Configuración

### Para Desarrollo Local

1. **Clona el repositorio**:
   ```bash
   git clone [URL_DEL_REPOSITORIO]
   cd AR
   ```

2. **Genera los marcadores AR**:
   - Ve a [AR.js Pattern Generator](https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html)
   - Genera 4 patrones únicos
   - Descarga los archivos `.patt` y reemplaza los archivos en `markers/`

3. **Abre el juego**:
   - Abre `index.html` en un servidor local o directamente en el navegador
   - Para mejor rendimiento, usa un servidor local:
     ```bash
     python -m http.server 8000
     # Luego ve a http://localhost:8000
     ```

### Para GitHub Pages

1. **Sube el proyecto** a un repositorio de GitHub
2. **Habilita GitHub Pages** en la configuración del repositorio
3. **Selecciona la rama main** como fuente
4. **Accede al juego** desde la URL generada

## 🎨 Características del Juego

### ✨ Elementos Visuales
- **Modelos 3D**: Libros, pergaminos, elementos universitarios
- **Textos flotantes**: Pistas históricas y narrativas
- **Animaciones**: Partículas doradas, rotaciones, efectos de pulso
- **Colores temáticos**: Verde (Recepción), Azul (Aula Magna), Naranja (Cantina), Púrpura (Biblioteca)

### 🔊 Audio
- **Sonidos de descubrimiento**: Melodías al encontrar cada pista
- **Sonido del tesoro**: Secuencia musical al completar el juego
- **Efectos ambientales**: Sonidos sutiles para mejorar la experiencia

### 📊 Sistema de Progreso
- **Contador visual**: Muestra pistas encontradas (X/4)
- **Mensajes de retroalimentación**: Confirmación al encontrar cada marcador
- **Información contextual**: Detalles sobre cada ubicación
- **Animación final**: Celebración al encontrar el tesoro

## 🏗️ Estructura del Proyecto

```
AR/
├── index.html              # Archivo principal del juego
├── markers/                # Archivos de patrones AR
│   ├── pattern-RECEPCION.patt
│   ├── pattern-AULA_MAGNA.patt
│   ├── pattern-CANTINA.patt
│   ├── pattern-PATIO.patt
│   └── pattern-BIBLIOTECA.patt
├── README.md              # Este archivo
└── preguntas.md           # Respuestas del proyecto
```

## 🎓 Contexto Histórico

### Edificio Sacré Coeur
- **Ubicación**: 8 de Octubre 2738, Montevideo
- **Estilo**: Neoclásico
- **Construcción**: 1925
- **Arquitecto**: Elzeario Boix
- **Historia**: Originalmente Colegio Sagrado Corazón de Jesús, dirigido por las monjas del Sagrado Corazón
- **Actualidad**: Universidad Católica del Uruguay (fundada en 1985)

## 🔧 Tecnologías Utilizadas

- **AR.js**: Librería de Realidad Aumentada para web
- **A-Frame**: Framework de WebVR/WebAR
- **HTML5**: Estructura del juego
- **CSS3**: Estilos y animaciones
- **JavaScript**: Lógica del juego y eventos
- **Web Audio API**: Efectos de sonido

## 📝 Notas de Desarrollo

### Marcadores AR
Los archivos `.patt` actuales son placeholders. Para el funcionamiento completo:

1. **Genera patrones reales** usando el generador de AR.js
2. **Imprime en papel blanco** con buena calidad
3. **Coloca en ubicaciones fijas** del edificio
4. **Asegura buena iluminación** para el escaneo

### Optimizaciones
- **Carga asíncrona** de librerías externas
- **Compresión de assets** para mejor rendimiento
- **Responsive design** para diferentes dispositivos
- **Fallbacks** para navegadores sin soporte AR

## 🎯 Objetivos Educativos

- **Historia local**: Conocimiento del Edificio Sacré Coeur
- **Tecnología AR**: Comprensión de realidad aumentada basada en marcadores
- **Programación web**: Integración de librerías JavaScript
- **Diseño de experiencia**: Creación de narrativas interactivas

## 🐛 Solución de Problemas

### La cámara no funciona
- Verifica permisos del navegador
- Asegúrate de usar HTTPS (requerido para cámara)
- Prueba en diferentes navegadores

### Los marcadores no se detectan
- Verifica que los archivos `.patt` sean correctos
- Asegura buena iluminación
- Mantén el marcador estable y centrado
- Verifica que el marcador esté impreso correctamente

### El juego no carga
- Verifica conexión a internet
- Revisa la consola del navegador para errores
- Asegúrate de que todas las librerías se carguen correctamente

## 📞 Contacto

Para dudas o problemas con el proyecto, contacta al equipo de desarrollo.

---

**¡Disfruta explorando el Tesoro del Conocimiento en la Universidad Católica!** 🎓✨
