# Saludo

> Última revisión: 2026-09-28 · Responsable: Juan

<!-- Regla de prueba: para validar el ciclo completo (detectar → interpretar →
insertar) antes de construir reglas de negocio más elaboradas. -->

## Qué hace

Cubre los mensajes que son solo un saludo o cortesía dirigidos al canal de
soporte de Gravity Support (ej. "Hola", "Buenos días", "Hi Juan", "Gracias
por la ayuda"), cuando el mensaje está relacionado con el trabajo de soporte
(Kids Empire / Foxihost) y no trae ninguna pregunta o solicitud real.

## Condiciones

- El mensaje es un saludo o cortesía dirigido al canal/soporte de trabajo.
- El mensaje está relacionado con el scope laboral (Gravity Support, Kids
  Empire, Foxihost) — no charla personal ajena al trabajo.
- El mensaje no contiene ninguna pregunta ni solicitud adicional.
- Si se conoce el nombre de quien escribe ("Name to use if you greet them"),
  el saludo debe incluirlo (ej. "Hello Marissa!"). Si no se conoce, se saluda
  sin nombre — nunca se inventa uno.
- La respuesta SIEMPRE va en inglés, sin importar en qué idioma esté el
  mensaje original (regla general del sistema, no solo de este módulo).

## Excepciones

- Si el saludo viene junto con una pregunta o solicitud (ej. "Hola, ¿cómo
  reviso una membresía?"), NO uses este módulo: la pregunta debe resolverse
  con el módulo del tema correspondiente. Si ese tema no tiene módulo o está
  en "siempre debe escalar", debe escalar igual aunque el saludo por sí solo
  fuera inofensivo.
- Charla personal o social que no tiene nada que ver con el trabajo (memes,
  comentarios fuera de tema) → no se responde (`supported: false`).

## Nivel de autonomía permitido a la IA

<!-- Opciones: puede responder sola | con aviso | siempre debe escalar -->
**Nivel:** puede responder sola

Notas: es solo cortesía, no hay información sensible, dinero ni decisiones de
negocio en juego. Sirve como regla de prueba de extremo a extremo.

## Errores comunes de quien recién empieza

- Usar este módulo para contestar la pregunta real que viene junto al saludo
  → el saludo puede ir al inicio de la respuesta, pero el contenido de
  negocio necesita su propio módulo.
- Contestar saludos o charla que no están relacionados con el trabajo → no;
  esos deben quedar sin respuesta.

## Casos reales

- **Pregunta:** "Hola equipo!" (autor: "AM Marissa Ware")
  **Respuesta correcta:** "Hello Marissa! How can I help?" (en inglés aunque el
  mensaje original haya llegado en español — regla general del sistema)
- **Pregunta:** "Goodmorning Everyone!!" (autor: "M Rishunda Colbert")
  **Respuesta correcta:** "Good morning Rishunda! How can I help?"
- **Pregunta:** "Buenos días Juan, gracias por la ayuda de ayer" (autor sin
  nombre reconocible)
  **Respuesta correcta:** "You're welcome! Let me know if you need anything
  else." (sin nombre, porque no se pudo determinar con certeza; en inglés
  aunque el mensaje haya llegado en español)
