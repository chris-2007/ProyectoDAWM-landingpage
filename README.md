# Proyecto: Landing Page del Museo del Cacao

**Institución:** Escuela Superior Politécnica del Litoral (ESPOL)  
**Facultad:** Facultad de Ingeniería en Electricidad y Computación (FIEC)  
**Materia:** Desarrollo de Aplicaciones Web y Móviles  
**Autores:** Christopher Flores, Ricardo Gordillo  
**Enlace Público:** [https://chris-2007.github.io/ProyectoDAWM-landingpage/](https://chris-2007.github.io/ProyectoDAWM-landingpage/)

---

## Tabla de Contenidos
1. [Análisis](#análisis)
   * [Análisis Comparativo de Plantillas](#análisis-comparativo-de-plantillas)
2. [Planificación](#planificación)
   * [Objetivos del Proyecto](#objetivos-del-proyecto)
   * [Requerimientos del Sitio Web](#requerimientos-del-sitio-web)
   * [Tabla de Organización y Arquitectura del Contenido](#tabla-de-organización-y-arquitectura-del-contenido)
3. [Diseño](#diseño)
   * [Identidad Visual y Paleta de Colores](#identidad-visual-y-paleta-de-colores)
   * [Variables a usar en CSS](#variables-a-usar-en-css)
4. [Implementación](#implementación)
   * [Modificación de la Estructura HTML](#modificación-de-la-estructura-html)
   * [Personalización del Diseño con CSS](#personalización-del-diseño-con-css)
   * [Registro de Control de Versiones con Git y GitHub](#registro-de-control-de-versiones-con-git-y-github)
5. [Despliegue](#despliegue)
   * [Entorno y Requisitos Previos de Alojamiento](#entorno-y-requisitos-previos-de-alojamiento)
   * [Procedimiento de Publicación en GitHub Pages](#procedimiento-de-publicación-en-github-pages)
6. [Bibliografía](#bibliografía)

---

## Análisis

En esta primera fase se evaluaron tres plantillas de diseño web seleccionadas del repositorio de código abierto HTML5 UP: *Story*, *Future Imperfect* y *Twenty*. El objetivo del análisis fue determinar la plantilla que mejor se adapte a los requerimientos de información, navegación e interacción identificados durante la etapa de levantamiento de datos del Museo del Cacao.

### Análisis Comparativo de Plantillas

1. **Story**
   * **Estructura:** Plantilla modular de una sola página. Utiliza bloques de contenido en formato de banners de ancho completo (divididos o de pantalla completa), combinados con galerías responsivas y elementos en cuadrícula.
   * **Navegación:** Menú flotante o lateral con desplazamiento suave (*smooth scrolling*) hacia las distintas secciones de la página.
   * **Diseño:** Estética moderna y visual. Destaca por el uso de fondos divididos (imagen y texto) y transiciones bien trabajadas, ideal para narrativas visuales.
   * **Adaptabilidad:** Completamente responsive y optimizada para dispositivos móviles y de escritorio.
   * **Facilidad de Personalización:** Moderada-Alta. Permite reorganizar o eliminar bloques editando directamente la estructura de etiquetas HTML.

2. **Future Imperfect**
   * **Estructura:** Plantilla de diseño editorial orientada a blogs o revistas digitales. Presenta un esquema de columnas múltiples con tarjetas de artículos, barra lateral (*sidebar*) y metadatos de publicaciones.
   * **Navegación:** Barra superior con menús desplegables y accesos a redes sociales o secciones de archivo.
   * **Diseño:** Minimalista y sobrio, enfocado en la legibilidad de textos largos y artículos estructurados.
   * **Adaptabilidad:** Excelente reestructuración vertical en pantallas pequeñas.
   * **Facilidad de Personalización:** Moderada. Diseñada fuertemente para blogs, por lo que requiere modificaciones sustanciales en CSS/HTML para adaptarse a un formato de landing page de un museo.

3. **Twenty**
   * **Estructura:** Plantilla landing page corporativa e institucional completa. Incluye una cabecera de alto impacto (*Hero Section*), secciones alternas de texto e imagen, cuadrículas de características/servicios, barras de llamada a la acción (CTA) y un pie de página (*footer*) estructurado.
   * **Navegación:** Barra de navegación superior fija (*sticky header*) con soporte para menús desplegables (*dropdowns*) y botones de acción rápida.
   * **Diseño:** Profesional, cálido y equilibrado. Combina bloques oscuros y claros con iconos vectoriales, encajando con un enfoque cultural y patrimonial.
   * **Adaptabilidad:** Totalmente adaptativa, con menú hamburguesa optimizado para smartphones.
   * **Facilidad de Personalización:** Muy Alta. Su código se encuentra claramente organizado por etiquetas explicativas (`#banner`, `#main`, `#cta`), lo que facilita la inserción de las secciones requeridas.

#### Tabla Comparativa

| Criterio | Story | Future Imperfect | Twenty |
| :--- | :--- | :--- | :--- |
| **Enfoque Principal** | Portafolios y narrativas visuales one-page. | Blogs y revistas de contenido editorial. | Landing pages corporativas, institucionales y turísticas. |
| **Estructura** | Bloques horizontales de ancho completo. | Múltiples columnas con tarjetas de blog y sidebar. | Cabecera Hero, cuadrículas de salas/servicios, banners CTA y footer. |
| **Navegación** | Desplazamiento suave (*smooth scroll*). | Menús superiores clásicos y barra de búsqueda. | Barra superior fija (*sticky*) con menú desplegable e iconos. |
| **Diseño** | Moderno, versátil y visual. | Editorial y enfocado en la lectura. | Profesional, cálido, estructurado e institucional. |
| **Facilidad de Personalización** | Alta (para páginas de una sola sección). | Moderada (requiere reestructurar la lógica de blog). | Muy Alta (se acopla de manera nativa a la estructura del sitio). |

Con todo esto hemos decidido que la mejor opción es **Twenty**.

---

## Planificación

En la fase de planificación definimos la visión estratégica del proyecto, los objetivos a alcanzar, los requerimientos del sistema y la organización de los contenidos.

### Objetivos del Proyecto

* **Objetivo General:** Diseñar e implementar una landing page atractiva, intuitiva y responsiva para el Museo del Cacao que promueva el valor patrimonial e histórico del cacao ecuatoriano y facilite la reserva e información para visitantes locales e internacionales.
* **Objetivos Específicos:**
  * Estructurar el contenido informativo basándose en los hallazgos del levantamiento de datos realizado a los visitantes.
  * Implementar un diseño adaptativo utilizando la plantilla Twenty de HTML5 UP.
  * Proveer canales directos de contacto, horarios y reserva de actividades educativas/guiadas.

### Requerimientos del Sitio Web

* **Requerimientos Funcionales:**
  * Menú de navegación fijo (*sticky*) con enlaces directos a las secciones.
  * Formulario de contacto y reserva de visitas guiadas.
  * Botones de llamada a la acción (CTA) para la compra de boletos e información rápida.
  * Mapa de ubicación interactivo.
* **Requerimientos No Funcionales:**
  * **Diseño Responsive:** Adaptación fluida a dispositivos móviles, tablets y computadoras de escritorio.
  * **Usabilidad:** Navegación clara con un tiempo de lectura óptimo.
  * **Compatibilidad:** Correcta visualización en navegadores modernos (Chrome, Firefox, Safari, Edge).

### Tabla de Organización y Arquitectura del Contenido

| Nombre de la Sección | Propósito de la Sección | Datos e Información que se Presentarán |
| :--- | :--- | :--- |
| **1. Cabecera / Hero Section (Inicio)** | Captar el interés inmediato del visitante y presentar la propuesta de valor del museo. | • Título principal sobre el patrimonio e historia del cacao en Ecuador.<br>• Subtítulo sobre el origen del cacao fino de aroma.<br>• Botones de acción (CTA): "Planifica tu visita" y "Compra tus entradas".<br>• Imagen de fondo de la Casa Guzmán Aspiazu. |
| **2. Conoce el Museo (Quiénes Somos)** | Presentar el valor patrimonial, histórico y cultural de la institución. | • Historia de la restauración de la sede histórica (Casa Guzmán Aspiazu).<br>• Relevancia cultural del cacao en la identidad de Guayaquil y Ecuador.<br>• Contexto de la época de los "Gran Cacao" y su impacto socioeconómico. |
| **3. El Recorrido y Experiencias (Salas)** | Exponer la oferta expositiva y los atractivos visuales del recorrido. | • Recorrido cronológico desde el origen prehispánico (cultura Mayo Chinchipe, 5000 años de historia).<br>• Muestra de maquetas, herramientas de cosecha tradicionales y figuras a escala real de los cacahueros.<br>• Explicación del proceso: "De la semilla a la barra de chocolate". |
| **4. Propuesta Educativa y Talleres** | Difundir las actividades dirigidas a estudiantes, familias y visitantes en general. | • Programas y convenios para escuelas y universidades.<br>• Talleres cortos de cata de chocolate y chocolatería artesanal.<br>• Información didáctica sobre el cacao nacional fino de aroma frente a variedades como el CCN51. |
| **5. Experiencias y Testimonios** | Validar la calidad del servicio a través de la opinión de visitantes previos. | • Indicadores de satisfacción global (altas tasas de recomendación y valoración positiva de la visita).<br>• Comentarios reales de visitantes sobre la atención del personal y la calidad del recorrido.<br>• Enlaces a contenido en redes sociales (videos informativos en TikTok/Instagram). |
| **6. Información Práctica y Logística (FAQ)** | Resolver dudas frecuentes operativas y prevenir inconvenientes reportados. | • Horarios de atención y tarifas de entrada.<br>• Recomendaciones de accesibilidad (tercera edad y personas con movilidad reducida).<br>• Información sobre estacionamiento cercano, tienda de recuerdos y cafetería. |
| **7. Contacto y Boletería (Footer)** | Facilitar canales directos de comunicación y reserva. | • Formulario de contacto para visitas guiadas grupales.<br>• Mapa de ubicación interactivo.<br>• Enlaces a redes sociales y datos institucionales. |

---

## Diseño

En esta etapa se establecen las directrices de diseño visual, la identidad de marca web, el sistema de variables CSS, la tipografía y la distribución de componentes (*layout*) para la landing page e interfaz global del sitio web del Museo del Cacao.

### Identidad Visual y Paleta de Colores

La paleta cromática se diseñó con un enfoque temático e histórico, inspirada en los tonos orgánicos del fruto del cacao, el chocolate artesanal, las haciendas cacaoteras tradicionales y la arquitectura patrimonial de la Casa Guzmán Aspiazu. Se implementó un sistema de variables CSS (`:root`) para garantizar consistencia visual y facilidad de mantenimiento.

### Variables a usar en CSS

```css
:root {
    /* --- Identidad Principal (Cacao & Oro) --- */
    --color-banner: #3D2314;           /* Marrón cacao profundo, elegante y de alto impacto */
    --color-boton: #C89D34;            /* Dorado / Oro cacao para llamadas a la acción (CTA) */
    --color-fondo: #FDFBF7;            /* Tono crema cálido/marfil, suave para la vista */
    --color-boton-borde: #3D2314;      /* Marrón oscuro para bordes de botones secundarios */
    --color-texto: #4A4238;            /* Sepia oscuro/tierra para óptima legibilidad */
    --color-enlace: #8C4A27;           /* Terracota / Marrón rojizo para enlaces */
    --color-enfoque: #C89D34;          /* Dorado para estados :focus e interacciones */

    /* --- Bordes, Sombras y Capas --- */
    --color-borde: rgba(74, 42, 27, 0.18);        /* Borde marrón tenue */
    --color-borde-tenue: rgba(74, 42, 27, 0.08);  /* Borde secundario sutil */
    --color-sombra: rgba(61, 35, 20, 0.1);         /* Sombra cálida y suave */
    --color-banner-overlay: rgba(30, 15, 8, 0.55); /* Capa de contraste sobre imágenes */

    /* --- Fondos de Secciones Estructuradas --- */
    --color-cta: #4A2E1B;              /* Marrón cacao mediano para barra de acción */
    --color-footer: #2A180E;           /* Marrón cacao extra oscuro para pie de página */
    --color-tabla-encabezado: #5C3D2E;  /* Tono cacao para encabezados de tablas */    

    /* --- Navegación (Header y Menú) --- */
    --color-nav: #24140B;              /* Marrón muy oscuro institucional */
    --color-nav-borde: rgba(200, 157, 52, 0.2); /* Destello dorado en divisores */
    --color-nav-boton: rgba(253, 251, 247, 0.85); /* Enlaces del menú principal */

    /* --- Redes Sociales (Ajustadas a Tonos Sobrios) --- */
    --color-twitter: #558098;
    --color-twitter-hover: #6894AC;
    --color-facebook: #4A6B94;
    --color-facebook-hover: #5B7DA8;
    --color-google-plus: #C0554E;
    --color-google-plus-hover: #D1665F;
    --color-github: #8C6D58;
    --color-github-hover: #9E7E69;
    --color-dribbble: #B85B88;
    --color-dribbble-hover: #C96C99;

    /* --- Estados Generales y Utilidades --- */
    --color-blanco: #ffffff;
    --color-hover: rgba(200, 157, 52, 0.12);      /* Overlay al pasar el cursor (dorado tenue) */
    --color-hover-claro: rgba(255, 255, 255, 0.15);
    --color-transparente: transparent;
}
```

---

## Implementación

La fase de implementación describe el proceso de construcción del sitio web mediante la modificación semántica del HTML de la plantilla seleccionada (Twenty), la personalización de estilos CSS para reflejar la identidad del evento y el control de versiones a través de Git y GitHub.

### Modificación de la Estructura HTML

El proceso de adaptación del archivo HTML consistió en depurar el código base de la plantilla para alinearlo con las necesidades reales:

1. **Eliminación de contenido demostrativo:** Se removieron las secciones de prueba (*lorem ipsum*), imágenes predeterminadas y enlaces ficticios de la plantilla que no correspondan al evento.
2. **Estructuración semántica:** Se mantuvo y reforzó el uso de etiquetas HTML5 semánticas (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`) para asegurar una correcta jerarquía de contenido y accesibilidad web.
3. **Incorporación de información real:**
   * **Navegación fija (`<header>`/`<nav>`):** Se configuraron los hipervínculos del menú principal para conectar de manera fluida con las 7 secciones planificadas.
   * **Sección principal:** Se adaptaron los títulos y subtítulos principales con la propuesta de valor del museo, acompañados de botones de acción para reservaciones y recorrido visual.
   * **Cuerpo principal (`<main>`):** Se integraron los textos e imágenes recopilados sobre la historia del cacao, la cultura Mayo Chinchipe, la Casa Guzmán Aspiazu, las maquetas de cacahueros y los talleres de cata.
   * **Módulo de testimonios:** Se incluyó una sección adaptada para destacar la satisfacción de los visitantes a partir de los datos analizados.
   * **Formulario y pie de página (`<footer>`):** Se implementaron los campos de captura de datos de contacto (nombre, correo, tipo de visitante) y enlaces a redes sociales oficiales.

### Personalización del Diseño con CSS

La adaptación visual se llevó a cabo mediante la modificación de las hojas de estilos para aplicar las reglas de la marca del Museo del Cacao:

1. **Aplicación de la paleta de colores:** Se redefinieron las variables globales del CSS para aplicar los tonos tierra y marrón cacao en encabezados y contenedores clave, y el tono dorado en botones de acción e indicadores visuales.
2. **Configuración tipográfica:** Se optimizaron las fuentes tipográficas ajustando los tamaños de fuente, interlineados y pesos para garantizar la legibilidad.
3. **Optimización responsive:** Se revisaron y ajustaron las reglas de *media queries* para asegurar que las tarjetas de las salas, tablas de horarios y formularios se reordenen dinámicamente en teléfonos móviles y tablets.

### Registro de Control de Versiones con Git y GitHub

El desarrollo del sitio se registró mediante el control de versiones Git, manteniendo un flujo de trabajo estructurado basado en commits frecuentes y descriptivos que reflejen el avance cronológico del proyecto:

1. **Inicialización:** Descarga de la plantilla base e inicialización del repositorio local de Git con la rama principal (`main`).
2. **Estructuración HTML:** Registro de cambios enfocado en la depuración del contenido demostrativo y la inclusión de la estructura semántica de las 7 secciones.
3. **Integración de Contenidos:** Commit dedicado a la adición de los textos reales, imágenes optimizadas y datos del formulario de levantamiento de información.
4. **Personalización CSS:** Registro de la aplicación de la hoja de estilos personalizada con la paleta de colores, fuentes tipográficas y diseño responsivo.
5. **Revisión y Ajustes:** Commits de corrección para ajustar el comportamiento del menú de navegación en smartphones y corregir estilos en el formulario de contacto.
6. **Publicación y Documentación:** Actualización del archivo `README.md` del repositorio con las instrucciones de compilación, estructura del proyecto y enlaces de previsualización.

---

## Despliegue

La fase de despliegue detalla el procedimiento técnico llevado a cabo para trasladar el sitio web desde el entorno de desarrollo local hacia un servidor web público y accesible en línea mediante la plataforma GitHub Pages.

### Entorno y Requisitos Previos de Alojamiento

Al tratarse de un sitio web estático desarrollado con HTML5, CSS3 y JavaScript puro, no requiere de bases de datos relacionales complejas ni de servidores con entornos de ejecución de backend (como Node.js, PHP o Python). Esto permite utilizar servicios de alojamiento estático optimizados y gratuitos, siendo GitHub Pages la opción ideal por su integración nativa con el control de versiones.

### Procedimiento de Publicación en GitHub Pages

El despliegue se ejecutó siguiendo una secuencia estructurada de pasos operativos:

1. **Preparación del Repositorio Remoto:** Se creó un repositorio público en la plataforma GitHub y se aseguró que la estructura de archivos en la raíz del repositorio incluyera de manera obligatoria el archivo principal de entrada con el nombre exacto de `index.html`, acompañado de las carpetas de recursos.
2. **Subida de Archivos (*Push*):** Se sincronizó el repositorio local con el repositorio remoto ejecutando los comandos de control de versiones correspondientes:
   ```bash
   git add .
   git commit -m "Despliegue inicial de la landing page del Museo del Cacao"
   git push origin main
   ```
3. **Configuración del Servicio de Hosting:**
   * Dentro de la interfaz del repositorio en GitHub, se ingresó a la sección de **Settings** (Configuración) y posteriormente al menú lateral **Pages**.
   * En el apartado de **Build and deployment**, se configuró la fuente de despliegue (*Source*) seleccionando la rama principal (`main`) y especificando el directorio raíz (`/ (root)`).
   * Se guardaron los cambios para activar el compilador estático automatizado de GitHub.
4. **Verificación y Enlace Público:**
   * Tras un breve proceso de compilación de 1 a 2 minutos, la plataforma generó la URL pública oficial del proyecto:  
     👉 [https://chris-2007.github.io/ProyectoDAWM-landingpage/](https://chris-2007.github.io/ProyectoDAWM-landingpage/)
   * Se realizaron pruebas de navegación en vivo para comprobar la correcta carga de la paleta de colores personalizada, las fuentes tipográficas, la visualización de las 7 secciones del museo y la fluidez del menú desplegable en dispositivos móviles.

---

## Bibliografía

* HTML5 UP. (s.f.). *Story by HTML5 UP*. Recuperado de https://html5up.net/story
* HTML5 UP. (s.f.). *Future Imperfect by HTML5 UP*. Recuperado de https://html5up.net/future-imperfect
* HTML5 UP. (s.f.). *Twenty by HTML5 UP*. Recuperado de https://html5up.net/twenty
* Museo del Cacao Guayaquil. (2026). *Formulario de levantamiento de información y experiencia de visitantes* [Conjunto de datos no publicado]. Proyecto de desarrollo web.
* Mozilla Developer Network (MDN). (2024). *CSS Custom Properties (Variables) and Responsive Web Design*. MDN Web Docs. Recuperado de https://developer.mozilla.org/es/docs/Web/CSS
* World Wide Web Consortium [W3C]. (2023). *HTML5 Semantic Elements and Accessibility Guidelines*. W3C Standards. Recuperado de https://www.w3.org/standards/webdesign/htmlcss