# Planificador de requerimientos – Subdirección de Infraestructura, SLEP Petorca

Esta página es solo la **pantalla de inicio de sesión**. El programa y todos los datos
(establecimientos, requerimientos, contratos, equipo) viven en Firebase y solo se descargan
después de entrar con un correo autorizado. Por eso este repositorio puede ser público sin exponer información.

- `index.html`: inicio de sesión y conexión con Firebase (proyecto `planificador-infra-petorca`).
  La configuración de Firebase no es secreta; la protección la dan las reglas.
- `firestore.rules`: reglas de seguridad (copia de las publicadas en Firebase).

## Roles
| Rol | Puede |
|---|---|
| admin | Todo, más agregar o quitar personas («Accesos»), cargar respaldos y actualizar el programa |
| editor | Editar todo (contrapartes) |
| cuadrilla | Ver y actualizar requerimientos (marcar hechos, cierre con fotos) |
| lector | Solo ver |

## Respaldo
«Respaldo» → «Descargar respaldo». Guardar el archivo una vez al mes en SharePoint (Infraestructura).

## Actualizar el programa
Se carga un archivo `programa_planificador_*.json` con «Respaldo» → «Cargar». No hace falta tocar GitHub.
