# Semana Empresarial 2026 – ExpoEmprende | UNIMINUTO

Sitio web responsive de inscripción para la Escuela de Ciencias Empresariales.

## Contenido
- `index.html`: página principal.
- `assets/uniminuto-logo.png`: logo suministrado.
- `assets/semana-empresarial.png`: pieza gráfica de divulgación.
- `backend/google_apps_script.gs`: backend opcional para guardar inscripciones en Google Sheets.

## Uso rápido
Abre `index.html` en un navegador. El formulario funciona en **modo demostración** y guarda registros en el navegador mediante `localStorage`.

## Activar inscripciones reales en Google Sheets
1. Crea una hoja de cálculo en Google Sheets.
2. Copia su ID (la parte de la URL entre `/d/` y `/edit`).
3. En Google Sheets ve a **Extensiones > Apps Script**.
4. Copia el contenido de `backend/google_apps_script.gs`.
5. Reemplaza `PEGA_AQUI_EL_ID_DE_TU_GOOGLE_SHEET`.
6. Implementa el script como **Aplicación web** y copia la URL terminada en `/exec`.
7. En `index.html`, busca:
   `const REGISTRATION_ENDPOINT = "";`
8. Pega la URL entre comillas.
9. Publica la carpeta en tu hosting institucional, GitHub Pages, Netlify, Vercel o servicio equivalente.

> Nota: las políticas institucionales pueden limitar el acceso público de Apps Script. Ajusta permisos según lineamientos de UNIMINUTO.
