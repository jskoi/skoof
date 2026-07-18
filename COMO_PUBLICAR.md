# Cómo publicar tu app en GitHub Pages

Archivos incluidos:
- `index.html` — la app
- `manifest.json` — hace que se pueda "instalar" como app
- `sw.js` — hace que funcione offline
- `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png` — íconos

## Pasos

1. Entra a https://github.com y crea una cuenta si no tienes.
2. Crea un repositorio nuevo (botón verde "New"). Ponle un nombre, por ejemplo `finanzas`. Puede ser público (tus datos igual quedan solo en tu celular, nadie los ve).
3. Sube **todos** los archivos de esta carpeta al repositorio:
   - Opción fácil: en la página del repo, click en "Add file" → "Upload files", arrastra los 6 archivos, y click en "Commit changes".
4. Ve a la pestaña **Settings** del repositorio → en el menú lateral busca **Pages**.
5. En "Source" selecciona la rama `main` y la carpeta `/ (root)`. Guarda.
6. Espera 1–2 minutos. GitHub te dará una URL como:
   `https://tuusuario.github.io/finanzas/`
7. Abre esa URL desde Chrome en tu celular.
8. Toca el menú (⋮) → **"Agregar a pantalla de inicio"** (o **"Instalar app"** si aparece directo). Listo: queda como app con ícono propio y pantalla completa.

## Notas
- Cada vez que quieras actualizar la app, solo tienes que volver a subir el `index.html` modificado al mismo repositorio (Add file → Upload files, sobrescribe).
- Tus datos (gastos, ingresos, PIN) se guardan en el navegador de tu celular (`localStorage`), no en GitHub. Nadie más los puede ver aunque el repositorio sea público.
- Si luego quieres el `.apk`, con esta URL ya puedes ir a https://www.pwabuilder.com, pegarla, y generar el paquete Android.
