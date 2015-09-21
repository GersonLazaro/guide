### Uso de repositorios

Primero, sigue las instrucciones para [configurar los repositorios de asignaciones][repository-setup]. Una vez creado, los repositorios deben ser inicializados con el contenido repetitivo. Esto puede ser un simple archivo README, pero podría también incluir un archivo de código, función de inicialización, función main(), etc.

#### Páginas de proyecto

Si los estudiantes necesitan proporcionar materiales de apoyo, documentación, o entradas de blog acerca de su proyecto, puedes hacer:

* Hacer commit con archivos [Markdown][markdown] directamente al repositorio
* Usar la [wiki del repositorio][wikis]
* Construir una página para el proyecto/clase en [Páginas Github][pages]

#### Testing automatizado

El [testing automatizado][automated-testing] (a menudo considerado como parte de la [integración continua][ci], or "CI") es una excelente manera de verificar rapidamente las soluciones de los estudiantes.  Su conjunto de pruebas podria incluir:

* Analisis estático
    * [Validación HTML][html-validator]
    * [JSHint][jshint]
    * [Cppcheck][cppcheck]
    * *y [muchas otras][static-analysis]*
* Pruebas unitarias
    * Las pruebas pueden ser escritas por ti o por los estudiantes
    * Ocultas para el estudiante o no

Hay muchas herramientas y servicios que pueden correr pruebas automatizadas, incluyendo:

* [Travis CI][travis]
* [Jenkins CI][jenkins]
* [Web-CAT][web-cat]
* [CodeClimate][code-climate]
* [Coveralls][coveralls]

Estas herramientas pueden ser configuradas para ejecutar las pruebas cada vez que un nuevo código es agregado por el estudiante al repositorio usando [webhooks][webhooks], aunque algunos realizan la configuración de forma automática.

### Recopilación de asignaciones

La mecánica recomensada para recoger las asignaciones depende de su se utiliza la estrategia de [fork][forks] or [sandbox][sandboxing].  En cualquier caso, la retroalimentación puede darse mediante pull request o [commits][commit-comments], o abriendo [issues][issues] en el repositorio de los estudiantes para que ellos lo "corrijan".  Esto puede ser hecho por los instructores, aunque es posible considerar la incorporación de revisión de código por pares como una manera de que los estudiantes practiquen el dar y recibir retroalimentación.  Tenga en cuenta que es posible que deba conceder a los estudiantes [acceso de solo lectura][access-permissions] a uno de los otros repositorios para permitir que vean los contenidos y dejen sus comentarios.

Una caracteristica de Github que puede ser util es utilizar los gráficos de [Red][network] y [contribuyentes][graphs], al igual que la lista de commits.  Como fue [señalado en la comunidad para docentes][community-graphs],

> Tener los resumenes analíticos de Github ha sido genial -- Solo tengo que revisar el gráfico de contribuyentes y rápidamente escanear los commits realizados.  Puedo ver quien hizo que, como y cuando en solo un par de segundos. También puedo ver el flujo de trabajo del proyecto.

Sin embargo, se advierte: no tomes los metadatos (o los gráficos generados por ellos) como un evangelio; un estudiante inteligente bien podria editar el(los) autor(es) del commit(s) o su fecha y hora despues de los hechos.

<!-- Links -->
[repository-setup]: /guide/repository_setup
[markdown]: https://guides.github.com/features/mastering-markdown/
[wikis]: https://guides.github.com/features/wikis/
[pages]: https://pages.github.com
[automated-testing]: https://en.wikipedia.org/wiki/Test_automation
[ci]: https://en.wikipedia.org/wiki/Continuous_integration
[html-validator]: http://validator.w3.org/source/
[jshint]: http://www.jshint.com/about/
[cppcheck]: http://cppcheck.sourceforge.net
[static-analysis]: https://en.wikipedia.org/wiki/List_of_tools_for_static_code_analysis
[travis]: http://docs.travis-ci.com
[jenkins]: http://jenkins-ci.org
[web-cat]: http://web-cat.org
[code-climate]: https://codeclimate.com
[coveralls]: https://coveralls.io
[webhooks]: https://developer.github.com/webhooks/
[forks]: /guide/forks
[sandboxing]: /guide/sandboxing
[commit-comments]: https://help.github.com/articles/adding-commit-comments
[issues]: https://guides.github.com/features/issues/
[access-permissions]: https://help.github.com/articles/permission-levels-for-an-organization-repository
[network]: https://github.com/blog/39-say-hello-to-the-network-graph-visualizer
[graphs]: https://help.github.com/articles/using-graphs
[community-graphs]: https://github.com/education/teachers/issues/7
