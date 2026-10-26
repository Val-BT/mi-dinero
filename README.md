# Mi Dinero — versión inicial

Esta es una app web instalable (PWA) para registrar manualmente ingresos, gastos y traspasos, filtrar movimientos y exportar/restaurar respaldos.

## Importante sobre privacidad
- Los movimientos se guardan en `localStorage` del navegador de ese dispositivo.
- No hay cuenta de usuario, servidor, sincronización ni conexión bancaria.
- Exportar el JSON crea una copia con tus datos: guárdala en un lugar privado.
- Si borras los datos del navegador, puedes perder los movimientos.
- No guardes NIP, CVV, contraseñas ni números completos de tarjetas.
- Esta versión inicial no tiene bloqueo con contraseña ni cifrado propio.

## Para probarla
Abre `index.html` en un navegador moderno. El registro funciona, pero la instalación PWA y el modo offline requieren servir la app desde HTTPS o desde `localhost`.

## Para instalarla en Android
1. Publica los archivos en un hosting estático HTTPS de confianza (por ejemplo, un proveedor que permita despliegue estático gratuito).
2. Abre la dirección en Chrome en tu Samsung.
3. Abre el menú de Chrome y elige “Instalar aplicación” o “Añadir a pantalla de inicio” (el texto puede variar).
4. Antes de registrar gastos reales, exporta un respaldo de prueba y comprueba que puedes importarlo.

## Archivos
- `index.html`: interfaz y lógica de la app.
- `manifest.json`: configuración de instalación.
- `service-worker.js`: caché básica para funcionamiento offline tras la primera carga.
