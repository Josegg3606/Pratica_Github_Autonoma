1. ¿Qué ventaja tiene registrar las dependencias del proyecto en requirements.txt en lugar de compartir la carpeta .venv?
R=Compatibilidad de sistemas operativo,contiene ejecutables binarios, rutas absolutas en el disco duro y enlaces simbolicos espeficos en el sistema operativo
¿Por qué el repositorio que tienes ahora en tu computadora no es el
mismo concepto que el fork creado en GitHub?
*Repositorio Local (tu computadora):Es tu *taller de trabajo*. Aquí editas, ejecutas y guardas los cambios de tu código sin necesidad de internet.
*Fork en GitHub (en la nube): Es tu *copia remota personal*. Sirve como respaldo en la web y como puente para subir tus cambios y compartirlos mediante un *Pull Request*.

 ## Preguntas y Respuestas ##
 79. Identificación del comando: Consultando los mensajes de orientación que muestra git status, la ayuda integrada de Git (git --help) o la documentación oficial.

80. Preparar vs. crear commit: Preparar (git add) selecciona los cambios y los pone en una zona intermedia (Staging Area); crear el commit (git commit) guarda esa foto de los cambios de forma permanente en el historial del repositorio.

81. Comprobar la rama activa: Ejecutando git branch (la rama actual estará marcada con un asterisco * y resaltada) o con el comando git status.

82. Determinar archivos modificados: Con el comando git status, el cual lista en color rojo todos los archivos que fueron modificados antes de prepararse.

83. Observar cambios exactos: Usando el comando git diff (o haciendo clic sobre el archivo en la sección de control de fuente de Visual Studio Code para ver la comparativa).

84. Reconstrucción de .venv: Porque la carpeta .venv es pesada y específica para la computadora y sistema operativo de quien la creó. No debe subirse a GitHub, por lo que cada desarrollador la genera localmente al descargar el proyecto.

85. Relación entre requirements.txt y .gitignore: Como .venv se excluye en .gitignore para no saturar el repositorio con archivos innecesarios, requirements.txt actúa como una lista ligera con las dependencias necesarias para que cualquiera pueda volver a construir la carpeta .venv.

86. Colaborar desde una rama: Para proteger el código estable de la rama principal (main), trabajar en paralelo sin afectar a otros colaboradores y permitir la revisión del código mediante Pull Requests antes de integrarlo.

87. Sin nuevo Pull Request: Porque el PR está vinculado a la rama, no a un commit específico; al subir correcciones con git push a esa misma rama, el Pull Request existente se actualiza automáticamente.

88. Actualizar el repositorio local: Porque el merge se realiza directamente en el servidor de GitHub; tu computadora no recibe esos cambios en su rama main local hasta que los descargues usando git pull.