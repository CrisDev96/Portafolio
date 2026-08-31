# Portafolio Web — IA, Automatización y Desarrollo Web

Sitio web comercial orientado a la adquisición de clientes independientes para servicios de IA, automatización, desarrollo web y marketing digital.

## Estructura

```
index.html              ← HTML + CSS + JS + i18n (sin credenciales)
config.js               ← Credenciales EmailJS (NO se sube al repositorio)
config.example.js       ← Plantilla de referencia para config.js
assets/
  profile_pic.png
  CariAI.png
  RidePro.png
  MedicalSoft.png
  Cafecito.png
  acoustic_design.png
```

## Configuración

### EmailJS (formulario de contacto)

El formulario usa [EmailJS](https://www.emailjs.com/) para enviar emails sin backend.

1. Copiar `config.example.js` como `config.js`
2. Reemplazar los valores con tus credenciales de EmailJS
3. `config.js` está en `.gitignore` y no se sube al repositorio

```js
// config.js (NO commitear este archivo)
window.__CONFIG = {
    emailJSService: 'service_z48r34f',
    emailJSTemplate: 'template_58efp5t',
    emailJSPublicKey: 'Ll5hNgU46qYa3BAI9'
};
```

### Variables del template EmailJS

El template debe usar estas variables:

| Variable | Descripción |
|---|---|
| `{{nombre}}` | Nombre del contacto |
| `{{empresa}}` | Empresa (opcional) |
| `{{email}}` | Email del contacto |
| `{{whatsapp}}` | WhatsApp (opcional) |
| `{{necesidad}}` | Servicio requerido |
| `{{descripcion}}` | Descripción del proyecto |

## Idiomas

Soporte ES/EN con toggle en el header. Las traducciones están en el objeto `translations` dentro del `<script>` de `index.html`.

## Despliegue

Archivo estático único. Funciona en cualquier hosting estático (GitHub Pages, Netlify, Vercel, etc.).

## Contacto

- **Email:** pedrazahoyoscristiandavid@gmail.com
- **WhatsApp:** +57 300 562 4810
- **LinkedIn:** [Cristian Pedraza](https://www.linkedin.com/in/cristian)
- **GitHub:** [CrisDev96](https://github.com/CrisDev96)
