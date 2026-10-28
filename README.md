# Mi Dinero — versión 6 consolidada

App web progresiva estática para registro personal de movimientos.

## Publicar en GitHub Pages
1. Descarga y descomprime este ZIP.
2. Sube los archivos que están dentro de `mi_dinero_app` a la raíz del repositorio (reemplazando `index.html`, `manifest.json` y `service-worker.js`).
3. Conserva el repositorio público solo si aceptas que el código sea público. Los datos no se incluyen en el repositorio: se cifran en el almacenamiento local del navegador.
4. Espera a que GitHub Pages termine de publicar y abre la URL HTTPS.

## Funciones
- Cifrado local AES-256-GCM con contraseña y PBKDF2; bloqueo automático tras 5 minutos de inactividad.
- Resumen mensual de ingresos y gastos.
- Cuentas/tarjetas creadas por la usuaria, saldos iniciales y saldos derivados de movimientos.
- Registro de ingresos, gastos y transferencias entre cuentas.
- Apartados Stori personalizados con movimientos fechados.
- Categorías de ingresos y gastos personalizables.
- Reportes por categoría y comparación de hasta seis meses.
- Exportación de respaldo cifrado e importación; CSV opcional sin cifrar.
- Vales de despensa creados con saldo inicial de $0.00. Cuentas predefinidas empiezan en $0.00.

## Límites importantes
- No se conecta a bancos, no verifica saldos reales ni sincroniza automáticamente entre dispositivos.
- Los datos permanecen en ese navegador/dispositivo; borrar almacenamiento del navegador puede perderlos. Exporta respaldos cifrados con regularidad y guarda la contraseña aparte.
- La exportación CSV no está cifrada.
- Esta app no ha sido auditada por un especialista en seguridad; prueba con datos ficticios antes de usar información financiera real.
- Las cuentas de crédito se muestran separadas del dinero disponible. Registra compras en tarjeta como gastos asociados a la tarjeta y pagos de tarjeta como transferencias desde una cuenta hacia la tarjeta.
