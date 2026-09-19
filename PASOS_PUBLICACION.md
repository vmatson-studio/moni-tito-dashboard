# Publicar el dashboard de Moni y Tito

## 1. Subir la demostración a GitHub Pages

1. En GitHub, crea un repositorio llamado `moni-tito-dashboard`.
2. Déjalo **público solo mientras use datos ficticios**.
3. Sube el archivo `index.html` a la raíz del repositorio.
4. Entra en **Settings → Pages**.
5. En **Build and deployment**, elige **Deploy from a branch**.
6. Selecciona la rama `main`, la carpeta `/root` y pulsa **Save**.
7. GitHub mostrará el enlace de la demostración cuando termine la publicación.

## 2. Probar las sesiones

Al abrir el enlace aparecen tres perfiles:

- Moni: propietaria y edición.
- Tito: propietario y edición.
- Vanne: administradora del proyecto.

Son sesiones locales de demostración. No usan contraseña y no protegen datos reales.

## 3. Activar acceso real sin pagar

1. Crea un proyecto en Firebase.
2. Añade una aplicación web.
3. En **Authentication → Sign-in method**, activa **Google** y **Email link**.
4. Añade el dominio de GitHub Pages en **Authorized domains**.
5. Crea una lista de usuarios autorizados con los correos de Moni, Tito y Vanne.
6. Pega la configuración web de Firebase en el bloque de autenticación del dashboard.
7. Comprueba que un correo no autorizado no pueda acceder.

No se recomienda el acceso por teléfono para esta primera prueba: necesita SMS, reCAPTCHA y puede implicar límites o costes. Google o enlace por email son más sencillos.

## 4. Conectar las respuestas

1. Crea la hoja `Boda Moni y Tito - Datos` en Google Sheets.
2. Importa el CSV de Tito en la pestaña `Invitados`.
3. Crea pestañas para `Respuestas`, `Menus`, `Transporte` y `Ninos`.
4. Publica un Apps Script como aplicación web.
5. Pega la URL terminada en `/exec` en **Ajustes → Datos y conexión**.
6. Prueba una respuesta ficticia antes de cargar datos reales.

## Regla de seguridad

No subir a un repositorio público nombres, teléfonos, correos, alergias ni respuestas reales. GitHub aloja el código; Google Sheets o Firebase guardan los datos protegidos.
