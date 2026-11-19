# Cómo publicar tu web en GitHub Pages

1. En GitHub crea un repositorio nuevo, por ejemplo `freelance` (público).
2. Pulsa **Add file → Upload files** y sube `index.html`. Confirma con **Commit changes**.
3. Ve a **Settings → Pages**. En *Source* elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`. Guarda.
4. En 1–2 minutos estará en: `https://roabuigues82-eng.github.io/freelance/`

## Usar tu dominio rominabuigues.es (opcional)
1. En **Settings → Pages → Custom domain** escribe `rominabuigues.es` y guarda.
2. En el panel de tu proveedor de dominio crea estos registros DNS:
   - 4 registros **A** para `@`: 185.199.108.153 · 185.199.109.153 · 185.199.110.153 · 185.199.111.153
   - 1 registro **CNAME** para `www` → `roabuigues82-eng.github.io`
3. Cuando GitHub lo verifique, marca **Enforce HTTPS**.

## Formulario de contacto
Ahora mismo, al pulsar "Enviar mensaje" se abre el correo del visitante con el mensaje ya escrito para ti.
Para recibir los mensajes sin que el visitante use su correo:
1. Crea una cuenta gratis en https://formspree.io y un formulario nuevo con tu email.
2. Copia la URL que te da (tipo `https://formspree.io/f/abcd1234`).
3. En `index.html`, busca `formEndpoint: ""` (al final del archivo) y pega la URL entre las comillas.

## Pendiente
- Busca `[TU PERFIL]` en `index.html` y cambia el enlace `https://linkedin.com/` por tu perfil de LinkedIn.
