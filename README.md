# Mi Dinero — versión con cifrado local

Aplicación web estática para registrar movimientos financieros manualmente.

## Seguridad de esta versión
- Los movimientos se cifran en el navegador antes de guardarse usando AES-256-GCM.
- La clave se deriva de una contraseña mediante PBKDF2-SHA-256 (310,000 iteraciones) y una sal aleatoria.
- La contraseña no se guarda. La app se bloquea automáticamente tras 5 minutos de inactividad.
- Los respaldos JSON exportados contienen solo el sobre cifrado; necesitan la misma contraseña para restaurarse.
- Los CSV son texto legible sin cifrar y la app muestra una advertencia antes de exportarlos.
- No hay servidor ni sincronización en la nube. Para usar en otro dispositivo, hay que trasladar el respaldo cifrado y conocer la contraseña.
- Si se olvida la contraseña y no hay una sesión desbloqueada, los datos no se pueden recuperar.

## Límites importantes
Es una implementación inicial y no una auditoría de seguridad profesional. El código de la app se publica en GitHub Pages. Mientras está desbloqueada, un navegador o una versión de la app comprometidos podrían acceder a los datos en memoria. Usa bloqueo de pantalla en el dispositivo, contraseña única, copias cifradas y mantén el navegador actualizado. No guardes NIP, CVV, contraseñas bancarias ni números completos de tarjetas.

## Publicación
Sube `index.html`, `manifest.json`, `service-worker.js` y `README.md` a la raíz del repositorio de GitHub Pages, reemplazando los archivos existentes. No subas respaldos financieros al repositorio.
