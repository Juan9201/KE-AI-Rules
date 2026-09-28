# Glosario

Términos internos que la IA debe entender al leer los mensajes de Gravity Support.
El Worker incluye este archivo en cada interpretación, así que mantenlo corto y preciso.

| Término | Significado |
|---|---|
| Kids Empire | Cadena de parques de juego para niños; el cliente al que damos soporte. |
| Foxihost | Plataforma/sistema que Kids Empire usa y al que Juan da soporte de producto. |
| Gravity Support | Canal de Connecteam por el que llegan los requerimientos de las sucursales. |
| Sucursal | Una ubicación física de Kids Empire. |
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
