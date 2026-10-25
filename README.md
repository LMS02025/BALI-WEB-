# BALI · Concesión Planta Desaladora para la Región de Coquimbo

Visor web interactivo de las **Bases de Licitación** (texto refundido) de la *Concesión Planta Desaladora para la Región de Coquimbo*. Es una página única (`index.html`) sin dependencias ni proceso de compilación.

## Funcionalidades

| Módulo | Descripción |
|---|---|
| **Índice** | Tabla de contenidos navegable de los 523 artículos (Cap. 1 Administrativas, Cap. 2 Técnicas, Cap. 3 Económicas y Anexos). |
| **Búsqueda** | Búsqueda de texto completo, sin distinguir tildes, con frases exactas entre comillas y salto entre coincidencias. |
| **Filtros** | Por capítulo, sección, etapa, categoría, criticidad, multas, plazos y notas propias. |
| **Notas** | Notas por artículo o sobre texto seleccionado, con etiquetas (Observación, Riesgo, Consulta, Cumplido) y exportación a `.md` / `.csv`. |
| **Panel · Resumen** | Indicadores clave, distribución por categoría, etapa y criticidad, y rankings de artículos más referenciados y con más multas. Cada elemento aplica su filtro con un clic. |
| **Panel · Mapa** | Mapa de todo el articulado: un cuadro por artículo, con tamaño según la extensión del texto y color por criticidad, etapa, multas, capítulo o notas. |
| **Panel · Relaciones** | Grafo de referencias cruzadas (a qué artículos remite y quién lo cita), con navegación e historial. |
| **Sonidos y animaciones** | Señales sonoras sintetizadas (silenciables) y transiciones. Se respeta la preferencia de "reducir movimiento" del sistema. |

## Atajos de teclado

| Tecla | Acción |
|---|---|
| `/` | Ir a la búsqueda |
| `Enter` / `Shift+Enter` | Coincidencia siguiente / anterior |
| `M` | Abrir o cerrar el Panel |
| `1` `2` `3` | Resumen / Mapa / Relaciones |
| `S` | Activar o silenciar sonidos |
| `Retroceso` | Volver al artículo anterior en Relaciones |
| `Esc` | Cerrar panel o paneles laterales |

## Publicación con GitHub Pages

1. Sube `index.html`, `README.md` y `.nojekyll` a la raíz del repositorio.
2. En **Settings → Pages**, elige *Deploy from a branch*, rama `main`, carpeta `/ (root)`.
3. El sitio queda disponible en `https://<usuario>.github.io/<repositorio>/`.

## Almacenamiento de notas

Las notas se guardan en el `localStorage` del navegador de cada usuario. No salen del equipo ni se comparten entre dispositivos. Para respaldarlas o compartirlas, usa **Mis notas → Exportar**.

## Observaciones sobre el texto fuente

Son incidencias heredadas del documento original:

- Título del artículo 1.17.2 ilegible en la fuente.
- Referencias a numerales que no existen como artículo separado (1.10.2.1.4, 1.13.2.5, 2.4.5.2, 2.4.6.5, 2.7.1.12, Anexo 1.3.4–1.3.7) redirigen al artículo superior.
- Varias multas sin monto informado ("s/d UTM").
- Referencia rota del procesador de texto en 1.14.5.1.7 ("¡Error! No se encuentra el origen de la referencia").

## Aviso

Esta herramienta sirve de apoyo para la consulta. El texto oficial y vinculante es el publicado por el mandante del proceso de licitación.
