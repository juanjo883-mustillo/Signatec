# SIGNATEC — Landing Page

Landing page estática (HTML + CSS puro, sin frameworks) para el proyecto SIGNATEC, guante traductor de Lengua de Señas Argentina.

## Estructura

```
signatec-site/
├── index.html
├── images/
│   ├── signatec_logo.jpeg
│   ├── prueba_guante.jpeg
│   ├── soldando_pistas.jpeg
│   ├── pines_esp32.jpeg
│   ├── armando_guante.jpeg
│   ├── conexiones.jpeg
│   ├── probando_todo_junto.jpeg
│   └── img_guante_casi_listo.jpeg
└── README.md
```

## Ver la página en tu computadora

No necesitás ningún servidor: abrí `index.html` con doble clic en cualquier navegador.

## Subir a GitHub

1. Creá un repositorio nuevo en GitHub (por ejemplo `signatec-landing`), **sin** agregar README ni .gitignore.
2. En tu computadora, dentro de la carpeta `signatec-site`, corré:

```bash
git init
git add .
git commit -m "Landing page de Signatec"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/signatec-landing.git
git push -u origin main
```

Reemplazá `TU-USUARIO` por tu nombre de usuario de GitHub.

## Publicar en Vercel (dominio gratis)

1. Entrá a [vercel.com](https://vercel.com) e iniciá sesión con tu cuenta de GitHub.
2. Hacé clic en **Add New → Project**.
3. Elegí el repositorio `signatec-landing` que acabás de subir.
4. Como es HTML puro, no hace falta configurar ningún **Build Command** ni **Framework Preset**: dejá todo en blanco/"Other" y el **Output Directory** apuntando a la raíz (`./`).
5. Hacé clic en **Deploy**.

En un minuto Vercel te va a dar una URL gratis del estilo `signatec-landing.vercel.app`. Cada vez que hagas `git push` a `main`, Vercel vuelve a desplegar la página automáticamente.

### Cambiar el dominio (opcional)

Desde el proyecto en Vercel → **Settings → Domains** podés:
- Cambiar el subdominio gratuito (`tu-nombre.vercel.app`).
- Conectar un dominio propio si más adelante comprás uno.

## Personalizar

- **Textos:** todo el contenido está directamente en `index.html`, en español y editable con cualquier editor de texto.
- **Colores:** están definidos como variables CSS al principio del archivo, dentro de `:root { ... }`.
- **Email de contacto:** buscá `contacto@signatec.example` en `index.html` y reemplazalo por tu email real.
- **Imágenes:** podés reemplazar cualquier archivo de `images/` manteniendo el mismo nombre, o cambiar la ruta en el `<img src="...">` correspondiente.
