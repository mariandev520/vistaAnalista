# Vistas — Servicio de reposición Mar del Plata

Bocetos de interfaz (HTML estático, sin build) para el servicio de reposición y merchandising.

## Vistas

| Archivo | Vista | Estado |
|---|---|---|
| `index.html` | Analista de cuenta / asistente comercial | En revisión |
| _(pendiente)_ | Supervisor / comercial (panel de Marcos Ferreyra) | Por hacer |

## Deploy en Vercel

Deploy estático de archivo único, sin configuración de build.

- **Desde el dashboard:** importar el repo y desplegar. Vercel sirve `index.html` en la raíz.
- **Desde la CLI:**
  ```
  npm i -g vercel
  vercel        # preview
  vercel --prod # producción
  ```

`vercel.json` sólo define `cleanUrls` y unas cabeceras básicas de seguridad.

## Fotos

`index.html` puede leer imágenes reales desde una carpeta `fotos/` ubicada al lado del HTML
(`nombre-tienda-1.jpg`, `-2`, `-3`). Si no existen, muestra el esquema de góndola generado.
