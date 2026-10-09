# Glosario

Términos internos que la IA debe entender al leer los mensajes de Gravity Support.
El Worker incluye este archivo en cada interpretación, así que mantenlo corto y preciso.

| Término | Significado |
|---|---|
| Kids Empire | Cadena de parques de juego para niños; el cliente al que damos soporte. |
| Foxihost | Plataforma/sistema que Kids Empire usa y al que Juan da soporte de producto. |
| Gravity Support | Canal de Connecteam por el que llegan los requerimientos de las sucursales. |
| Sucursal | Una ubicación física de Kids Empire. |
| Staff | Empleado del parque; es quien escribe en el chat. Nunca hay contacto con el huésped. |
| Guest / huésped | Cliente final del parque; solo lo atiende el staff. |
| Play Card | Tarjeta de 10 dígitos que guarda flames para jugar. Se vende en el POS (brazalete de $1). |
| Flames | Moneda de juego de las máquinas de Amusement Connect. |
| Receipt ID / Transaction # | Número (solo dígitos) del comprobante de pago en Gravity. |
| Gravity | `access.thegravityapp.io`; cobra al huésped y emite el recibo. |
| Amusement Connect | `app.amusementconnect.com`; proveedor de las máquinas y de los saldos de flames. |
| Webhook | Aviso automático de Gravity a Amusement Connect para cargar los flames; si falla, el pago queda sin recarga. |
| Manual Kiosk | Pantalla de Amusement Connect para recargar una tarjeta a mano ("Reload Card" → "Credit"). |
| TODO(Juan) | Agrega aquí abreviaturas, nombres de pantallas, nombres de máquinas, etc. |

## Rangos

<!--
El nombre que muestra Connecteam trae el rango como prefijo (ej. "AM Marissa
Ware", "M Rishunda Colbert"). El backend usa ESTA tabla para reconocer el
prefijo y sacar el nombre real antes de saludar (ej. "Marissa"), así el saludo
no incluye el rango ni corta el nombre a la mitad.

Reglas de esta tabla:
- Una fila por rango, el prefijo EXACTO tal como aparece en Connecteam
  (en mayúsculas, sin punto).
- Si un prefijo no está aquí, el sistema simplemente no lo recorta y usa la
  primera palabra del nombre tal cual (más seguro que adivinar).
- No hace falta reiniciar nada: el backend lee esta tabla en vivo desde GitHub.
-->

| Prefijo | Significado |
|---|---|
| AM | Assistant Manager (confirmado en captura de Connecteam) |
| M | Manager (confirmado en captura de Connecteam) |
| PM | Rango de sucursal (TODO(Juan): confirmar nombre completo) |
| SL | Rango de sucursal (TODO(Juan): confirmar nombre completo) |
| RM | Rango de sucursal (TODO(Juan): confirmar nombre completo) |
| DM | Rango de sucursal (TODO(Juan): confirmar nombre completo) |
| CTM | Rango de sucursal (TODO(Juan): confirmar nombre completo) |
| C | Rango de sucursal (TODO(Juan): confirmar nombre completo) |
| RTM | Rango de sucursal (TODO(Juan): confirmar nombre completo) |
| * | Prefijo especial que traen algunos nombres de usuario (ej. "* paquito contreras"); se trata como rango |
