# Instrucciones para agentes de IA (Claude, ChatGPT/Codex u otros)

Este repositorio contiene el perfil del Dr. Eduardo Portas Ruiz para su página de investigador
del CICA, Facultad de Comunicación, Universidad Anáhuac México:
https://investigadores-cica.pages.dev/eduardo-portas

Cada cambio guardado en `main` aparece en la página publicada en unos minutos.

## Qué puedes tocar
- `perfil.yml` y, si el investigador te da una foto, una imagen en la raíz del repositorio
  (referénciala en `foto:` por su nombre de archivo).
- No crees otros archivos ni cambies `AGENTS.md`, `CLAUDE.md` o `README.md`, salvo que él lo pida expresamente.

## Cómo editar `perfil.yml`
- Es YAML. Conserva la sangría de dos espacios y los comentarios existentes.
- Pon entre comillas dobles cualquier texto que contenga dos puntos (`:`).
- Campos vacíos se escriben `""` (o `[]` en listas); no los borres.
- Publicaciones: agrega cada obra nueva al inicio de la lista con
  `anio`, `tipo` (libro | articulo | capitulo | editorial | otro), `titulo`,
  `autores`, `fuente`, `enlace`. Solo una obra puede llevar `destacada: true` (con `resumen`).
- Prefiere el enlace DOI (`https://doi.org/...`). No inventes DOI, páginas, años ni coautores:
  si falta un dato, pregúntalo o déjalo vacío.
- La semblanza (`bio`) admite párrafos separados por una línea en blanco y *cursivas* con asteriscos.
- Al terminar, cambia `actualizado` a la fecha de hoy (`"AAAA-MM-DD"`).

## Privacidad
- El repositorio es público y el historial también. No agregues teléfonos personales,
  domicilios particulares ni otros datos que el investigador no haya pedido publicar.

## Antes de guardar
- Verifica que el YAML se pueda leer, por ejemplo:
  `python3 -c "import yaml; yaml.safe_load(open('perfil.yml'))"`
- Muestra al investigador un resumen de lo que cambiaste y pide su visto bueno.
- Mensaje de commit: `Actualiza perfil: <qué cambió>`.
