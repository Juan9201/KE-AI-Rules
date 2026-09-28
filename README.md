# Base de conocimiento — Soporte Kids Empire / Foxihost

Esta es la **fuente de verdad** del asistente de soporte. El Cloudflare Worker lee
este repo en vivo cada vez que interpreta un mensaje de Gravity Support. Si algo no
está escrito aquí, la IA responde literalmente `Allow me take a look`.

## Estructura

```
docs/
  business-logic/     ← un archivo .md por tema (lo que la IA puede usar)
    _TEMPLATE.md      ← plantilla; la IA la ignora
    membresias.md     ← ejemplo a medio llenar
  glosario.md         ← términos internos; se incluye en cada interpretación
  fts/CHANGELOG.md    ← registro humano de cambios importantes
```

## Cómo agregar o editar una regla

1. Usa `rule-editor.html` (hace commit directo a este repo a través del Worker), o
   edita el archivo en GitHub.
2. Sigue las secciones de `_TEMPLATE.md`. Las más importantes:
   - **Nivel de autonomía permitido a la IA** — `puede responder sola`, `con aviso`
     o `siempre debe escalar`. El Worker lo aplica del lado del servidor: aunque el
     modelo quiera responder, un módulo en `siempre debe escalar` produce
     `Allow me take a look`.
   - **Errores comunes de quien recién empieza** — tu criterio de experto.
3. Nombres de archivo: minúsculas, sin acentos ni espacios (`reembolsos.md`).

## Reglas de oro

- Escribe solo lo que estás seguro de que es correcto hoy.
- Temas con dinero, seguridad de máquinas o datos personales: `siempre debe escalar`.
- Nada de contraseñas, tokens ni datos de clientes en este repo.
