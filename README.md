# Mi Dinero — versión 3 (cifrado local)

Aplicación web instalable para llevar un registro manual de finanzas personales en MXN.

## Funciones
- Registro de ingresos, gastos y traspasos.
- Filtros por tipo y mes.
- Resumen de ingresos/gastos por mes y por quincena.
- Planeación de quincena: ingreso esperado, gastos fijos, pagos de deuda y ahorro previsto.
- Registro manual de deudas/tarjetas, saldo, pago habitual y fecha límite.
- Apartados y metas de ahorro con barra de progreso.
- Exportación de respaldo JSON cifrado e importación con la contraseña.
- Exportación CSV opcional sin cifrar (contiene datos legibles).
- Cifrado local AES-256-GCM y bloqueo automático tras 5 minutos de inactividad.

## Actualizar GitHub Pages desde el celular
1. Abre el repositorio `Val-BT/mi-dinero` en GitHub.
2. En Código, elige Add file → Upload files (Agregar archivo → Cargar archivos).
3. Descomprime este ZIP en tu celular y carga los cuatro archivos de la carpeta `mi_dinero_app` a la raíz del repositorio: `index.html`, `manifest.json`, `README.md` y `service-worker.js`.
4. Asegúrate de que la opción sea confirmar directamente en la rama predeterminada y confirma los cambios.
5. Espera a que la acción `pages build and deployment` termine en verde. Después abre `https://val-bt.github.io/mi-dinero/` y recarga; si la versión vieja queda en caché, cierra las pestañas de la app y vuelve a abrirla.

## Seguridad y límites
- Los datos se cifran en el navegador antes de guardarse en el almacenamiento local. No hay servidor de datos ni sincronización automática entre celular y computadora.
- La contraseña no se almacena; si se pierde, no se pueden descifrar los datos sin una copia y contraseña válidas.
- Guarda copias de respaldo cifradas en un lugar privado y prueba la restauración periódicamente.
- El CSV NO está cifrado. No lo compartas sin revisar su contenido.
- El repositorio y el código de la aplicación son públicos. No subas respaldos, movimientos ni datos personales al repositorio.
- No registres contraseñas bancarias, NIP, CVV ni números completos de tarjetas.
- Esta es una herramienta personal inicial, no una aplicación auditada profesionalmente. Mantén el teléfono actualizado y protegido con bloqueo de pantalla.
- Los saldos de deudas y apartados son manuales: no se conectan con bancos ni representan transferencias reales.
