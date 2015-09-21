Los estudiantes completan sus tareas usando forks (nota: esta configuración significa que **los estudiantes podrán ver el trabajo de sus compañeros**):

### 1. Crea los repositorios

**[Crea un repositorio][create-repo] por tarea**. Incluye cualquier archivo que tus estudiantes necesiten para empezar.

Si prefieres que tus tareas o el trabajo de tus estudiantes no sea publicamente visible, [solicita repositorios privados][private-repos] para utilizar en tu clase. Necesitas un repositorio privado por tarea.

### 2. Asigna a los estudiantes acceso de solo lectura

**Si tu repositorio es público puedes omitir este paso.**

Si los materiales de tu curso están en repositorios privados, los estudiantes necesitan acceso de solo lectura a ellos. Crea un equipo `estudiantes` con "acceso de lectura" y asigna el acceso al equipo a todos los repositorios que necesiten. Posteriormente, agrega cada estudiante al equipo, usando [`add_to_team`][add-to-team-action] en la herramienta [teachers_pet][teachers-pet] o [manualmente][help-add-to-team].

[Lee mas sobre el control de acceso][help-access-control].

### 3. Realizando las tareas

Tus estudiantes deben seguir los siguientes pasos para cada tarea:

1. Para empezar, [crea un **fork** del repositorio][forking].
1. [**Clona**][ref-clone] el repositorio a tu computador.
1. Modifica los archivos y crea un [**commit**][ref-commit] con los cambios realizados para completar la solución.
1. Realiza un [**Push**][ref-push] para sincronizar los cambios con github.
1. [Crea un **pull request**][pull-request] en el repositorio original.

Considera hacer una copia de estos pasos contextualizandolos en tu proyecto en tu syllabus o descripción de tareas – Toma el [markdown][raw].

### 4. Revisando las tareas

Una vez creado, puede hacer la revisión de código con retroalimentación linea a linea directamente dentro del pull request. Si permites que tus estudiantes presentes correcciones, pueden realizar las correcciones en sus respectivos forks, que se reflejaran en el pull request.

Dado que no deseamos tener ninguna solución en el repositorio de tareas original, debes dejar el pull request sin combinar (unmerged). Cuando termines de retroalimentar, puedes cerrar el pull request y dejar un  :+1: (`:+1:`) en un comentario final.

<!-- Links -->
[create-repo]: https://help.github.com/articles/create-a-repo
[private-repos]: /guide/private_repos
[add-to-team-action]: https://github.com/education/teachers_pet/#giving-others-access
[teachers-pet]: https://github.com/education/teachers_pet
[help-add-to-team]: https://help.github.com/articles/adding-organization-members-to-a-team
[help-access-control]: https://help.github.com/articles/what-are-the-different-access-permissions#organization-accounts
[forking]: https://guides.github.com/activities/forking/
[ref-clone]: http://gitref.org/creating/#clone
[ref-commit]: http://gitref.org/basic/#commit
[ref-push]: http://gitref.org/remotes/#push
[pull-request]: https://help.github.com/articles/creating-a-pull-request
[raw]: https://raw.githubusercontent.com/education/guide/master/docs/forks.md
