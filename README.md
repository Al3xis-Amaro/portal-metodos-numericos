# Portal de Métodos Numéricos

Página web educativa (HTML + CSS + JS, sin frameworks) con las 4 secciones del proyecto:

1. **Inicio y Glosario Visual** – 8 conceptos con diagrama y ejemplo de ingeniería + comparativa "tiro al blanco".
2. **Clasificación de Errores** – mapa conceptual, tabla con fórmulas, demo de redondeo en vivo y serie de *e* (truncamiento).
3. **Caso Práctico** – *e* truncado (2.71) y redondeado (2.72) a 3 cifras: errores absoluto, relativo y porcentual + interpretación.
4. **Zona Interactiva** – calculadora de errores, simulador de precisión vs. exactitud y quiz de 5 preguntas.

## Personalizar (antes de entregar)
Abre `index.html` y busca **`EDITA AQUÍ`** (está en el `<script>` del final). Ahí se ponen:
- `integrantes`: nombres completos del equipo.
- `carrera`, `grupo`, `profesor` (opcionales; si se dejan vacíos no se muestran).
- `formUrl`: enlace del quiz en Google Forms / Kahoot / Quizizz. Si se deja vacío, el botón no aparece.

Otros:
- **Logo:** guarda la imagen del logo como `logo.png` junto a `index.html` y aparece sola en la portada.
- **Vista previa al compartir:** después de publicar, en el `<head>` cambia `og:image` y `og:url` por la dirección completa
  (ej. `https://usuario.github.io/portal-metodos-numericos/og-image.png`).

### Preguntas sugeridas para el Google Form
1. Una báscula siempre marca 2 kg de más, pero sus lecturas casi no varían. ¿Es exacta, precisa o ambas? *(Precisa, no exacta)*
2. Si Vv = 50 y Va = 49, ¿cuál es el error relativo porcentual? *(2 %)*
3. Cortar una serie infinita en n términos produce error por… *(truncamiento)*

## Estructura
```
index.html          ← toda la página
og-image.png        ← imagen para la vista previa al compartir el enlace
vendor/katex/       ← librería para mostrar fórmulas (copia local)
```

## Publicar gratis (GitHub Pages)
1. Crear un repositorio público en GitHub y subir el contenido de esta carpeta.
2. Settings → Pages → Source: *Deploy from a branch* → rama `main`, carpeta `/ (root)`.
3. En 1–2 minutos queda en `https://<usuario>.github.io/<repositorio>/`.

Alternativa sin cuenta de GitHub: arrastrar la carpeta a https://app.netlify.com/drop
