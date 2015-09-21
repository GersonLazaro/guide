### Configuración

Para configurar las tareas usando el método sandboxing (conocido tambien como "caja de arena", "forks falsos" or [repositorios duplicados][help-duplicate]):

#### 1. Obtener un plan actualizado

Revisa nuestra [guia][private-repos] para crear repositorios privados para su clase. Necesitaras un repositorio privado por estudiante para cada tarea.

#### 2. Configura los repositorios

Tienes algunas opciones para organizar los repositorios de tus estudiantes. Tenemos una herramienta de linea de comandos llamada [teachers_pet][teachers-pet] que automatiza estos pasos. Puedes usar la acción [`create_repos`][create-repos-action] para crear repositorios, o seguir los pasos [manualmente][help-duplicate].

##### Proyectos individuales

Por cada estudiante:

1. Crea un repositorio en la organización con el nombre del estudiante.
1. Crea un equipo en la organización, que coincida con el nombre del repositorio.
1. Establece que el equipo tiene permisos `Push/Pull`.
1. Agrega los estudiantes al equipo.
1. Asigna al equipo acceso al repositorio correspondiente.

##### Proyectos grupales

Por cada grupo:

1. Crea un repositorio en la organización.
1. Crea un equipo en la organización.
1. Establece que el equipo tiene permisos `Push/Pull`.
1. Agrega los miembros del grupo al equipo.
1. Asigna al equipo acceso al repositorio correspondiente.

#### 3. Inicia los repositorios

Su tiene código/archivos iniciales que cada estudiante necesite, puedes crear un repositorio de inicio a nivel local, y luego realizar [push][ref-push] en cada repositorio de estudiante para esa tarea. La acción [`push_files`][push-files] en [teachers_pet][teachers-pet] automatiza esto para ti.

Para las instrucciones de la tarea, utilice una de estas dos opciones recomendadas:

* Crea un repositorio canónico con las instrucciones, en el repositorio syllabus, o en uno dedicado a la tarea. Esto da a los estudiantes una fuente general para referir a los estudiantes.  If creas un README en cada repositorio estudiantil, agrega un link a las instrucciones canónicas.
* Abre "issues" en cada repositorio estudiantil para que las completen.  El comando [`open_issue`] en [teachers_pet][teachers-pet] automatiza esto por ti.

### Recopilación de tareas

Cuando estes listo para calificar las tareas, puedes clonar los repositorios a tu maquina usando el comando [`clone_repos`][clone-repos] en [teachers_pet][teachers-pet].

<!-- Links -->
[help-duplicate]: https://help.github.com/articles/duplicating-a-repository
[private-repos]: /guide/private_repos
[create-repos-action]: https://github.com/education/teachers_pet#creating-assignments
[teachers-pet]: https://github.com/education/teachers_pet
[push-files]: https://github.com/education/teachers_pet#pushing-starter-files
[ref-push]: http://gitref.org/remotes/#push
[open-issue]: https://github.com/education/teachers_pet#opening-issues
[clone-repos]: https://github.com/education/teachers_pet#clone-repositories-for-grading
