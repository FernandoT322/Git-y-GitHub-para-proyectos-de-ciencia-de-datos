# Git-y-GitHub-para-proyectos-de-ciencia-de-datos
Aplicar herramientas colaborativas de software utilizadas en la industria para organizar, versionar y compartir un proyecto de ciencia de datos mediante Git y GitHub.
# Actividad práctica: Git y GitHub para proyectos de ciencia de datos

## Resultado de aprendizaje

Aplicar herramientas colaborativas de software utilizadas en la industria para organizar, versionar y compartir un proyecto de ciencia de datos mediante Git y GitHub.

## Fuente principal

La actividad se basa en la edición oficial en español de **Pro Git**, especialmente en los capítulos sobre instalación y configuración, fundamentos de Git, ramificaciones y GitHub:

- https://git-scm.com/book/es/v2
- https://git-scm.com/downloads

## Documentos incluidos

1. `tutorial_1_preparacion.docx` y `pdf/tutorial_1_preparacion.pdf`
   - Cuenta o comprobación de cuenta de GitHub.
   - Instalación y configuración de Git.
   - Creación del repositorio y clonación mediante `git clone`.
   - Primer `git add`, `git commit` y `git push`.

2. `tutorial_2_versionado.docx` y `pdf/tutorial_2_versionado.pdf`
   - Estructura mínima de un proyecto de ciencia de datos.
   - Uso de `git status` y `git diff`.
   - Preparación de cambios con `git add`.
   - Confirmaciones descriptivas mediante `git commit`.
   - Publicación con `git push`.

3. `tutorial_3_colaboracion.docx` y `pdf/tutorial_3_colaboracion.pdf`
   - Sincronización con `git pull`.
   - Creación de ramas con `git switch -c`.
   - Publicación de ramas remotas.
   - Integración mediante `git merge`.
   - Envío final a GitHub y cierre de la rama.

## Datos que debe completar el estudiante

- `[NOMBRE]`: nombre completo.
- `[ASIGNATURA]`: nombre de la asignatura.
- `[USUARIO_GITHUB]`: usuario real de GitHub.
- `[CORREO]`: correo configurado en Git.
- `[NOMBRE_REPOSITORIO]`: nombre del repositorio creado.
- `[CARPETA_DE_TRABAJO]`: ruta local utilizada para clonar.

No se deben incluir contraseñas, tokens ni claves privadas en los documentos o en el repositorio.

## Flujo general solicitado

```bash
git clone https://github.com/[USUARIO_GITHUB]/[NOMBRE_REPOSITORIO].git
cd [NOMBRE_REPOSITORIO]
git status
git add .
git commit -m "mensaje descriptivo"
git push origin main
```

Para el trabajo colaborativo se utiliza una rama:

```bash
git switch -c mejora-documentacion
git add docs/bitacora.md
git commit -m "docs: definir criterios de éxito del proyecto"
git push -u origin mejora-documentacion
git switch main
git pull origin main
git merge mejora-documentacion
git push origin main
```

## Cambios realizados en los documentos

- Se redujo la actividad a tres tutoriales integrados.
- Se incorporaron instrucciones de cuenta de GitHub o documentación de cuenta existente.
- Se incluyeron instalación, configuración, clonación, seguimiento, confirmación y publicación.
- Se incluyeron mensajes de confirmación descriptivos.
- Se incluyó un envío a GitHub después de cada tutorial.
- Se añadieron evidencias solicitadas y campos editables para los datos del estudiante.
- Cada documento contiene referencias directas a la edición oficial en español de *Pro Git*.
- Cada documento Word tiene una versión PDF equivalente.

## Qué subir a GitHub

Sube el contenido de esta carpeta al repositorio, reemplazando los campos entre corchetes por tus datos. Como mínimo, incluye:

- `README.md`
- Los tres archivos `.docx`.
- Los tres archivos `.pdf` de la carpeta `pdf/`.
- Las evidencias solicitadas por el docente, si son archivos permitidos.

## Confirmación final

Antes de entregar, ejecuta:

```bash
git status
git add .
git commit -m "docs: entregar actividad práctica de Git y GitHub"
git push origin main
```

Después, abre la URL de tu repositorio en GitHub y verifica que todos los archivos sean visibles.

## Referencias

Chacon, S., y Straub, B. *Pro Git*, 2.ª edición, versión oficial en español. https://git-scm.com/book/es/v2

Git. Página oficial de descargas. https://git-scm.com/downloads
