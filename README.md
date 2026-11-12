# 🎨 Aeducar: calificador amplio con rúbrica completa (Extensión Stylus)

Mejora la vista de **calificación de tareas en Aeducar (Moodle)**: rúbrica entera y legible, PDF más grande y con fondo blanco. Solo cambia cómo lo ves tú; no modifica nada en Aeducar.

## 1. Instalar Stylus (extensión del navegador)

- Chrome / Edge: [Stylus en Chrome Web Store](https://chromewebstore.google.com/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne)
- Firefox: [Stylus en Firefox Add-ons](https://addons.mozilla.org/firefox/addon/styl-us/)

## 2. Instalar el estilo

### Opción A — Instalación en un clic (recomendada)

Con Stylus ya instalado, abre este enlace y pulsa **Instalar estilo**:

👉 [aeducar-calificador.user.css](https://raw.githubusercontent.com/luisjsolsona/aeducar-calificador-stylus/main/aeducar-calificador.user.css)

Se aplica automáticamente a cualquier centro (`https://<tu-centro>.aeducar.es/mod/assign/view.php`) y Stylus te avisará cuando haya actualizaciones.

### Opción B — Manual

1. Abre Aeducar e inicia sesión.
2. Entra en una tarea → **Ver todos los envíos** → **Calificar**.
3. Pulsa el icono de Stylus en la barra del navegador.
4. En **Escribir estilo para…** elige la opción de la **URL** (debe empezar por `https://<tu-centro>.aeducar.es/mod/assign/view.php`).
5. Borra lo que aparezca y pega el contenido de [`moodle-admin.css`](moodle-admin.css).
6. Pon un nombre (p. ej. *Aeducar calificador*) y pulsa **Guardar**.
7. Recarga la página del calificador.

## 3. Ajustes y trucos

- **Más o menos zoom del PDF:** cambia `zoom: 1.3` (1 = tamaño normal, 2 = doble).
- **Si las anotaciones del PDF salen desplazadas:** borra el bloque *PDF ampliado* o desactiva el estilo desde el icono de Stylus mientras anotas.
- **Ver una captura en detalle:** usa **Ctrl + rueda**.
- **PDF a todo el ancho:** usa los botones de disposición de abajo a la derecha del calificador.
- **Desactivar temporalmente:** icono de Stylus → desmarcar el estilo.

## 4. Si eres administrador de Moodle… hazlo permanente y para tod@s

Usa el contenido de [`moodle-admin.css`](moodle-admin.css) en una de estas dos ubicaciones:

- **SCSS:** Administración del sitio → Apariencia → Temas → *tema activo* → Avanzado → **SCSS en bruto**.
- **HTML adicional:** Administración del sitio → Apariencia → HTML adicional → **Dentro de HEAD**, metiendo el código entre `<style>` y `</style>`.

## Ficheros

| Fichero | Uso |
|---|---|
| `aeducar-calificador.user.css` | Estilo Stylus instalable en un clic |
| `moodle-admin.css` | CSS plano: instalación manual en Stylus o en la configuración de Moodle |

---

Luis Solsona · [github.com/luisjsolsona](https://github.com/luisjsolsona)
