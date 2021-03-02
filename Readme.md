# El uso de Git y Github para trabajos colavorativos
![Git](https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2017/12/gitHub.png)
## **Participantes**
1. Hemil A. Del Orbe Medrano
 2. Enmanuel Herrera
 3. Moises Santiago

 # Temas

**El Uso de Git y GitHub para trabajos colaborativos.**

<p style ="text-aling: justify"> Git es una excelente herramienta para desarrollar de forma individual y colaborativa.</p>

Supongamos que estás trabajando en un proyecto y quieres agregar una nueva funcionalidad. La forma correcta es creando una branch o rama con el nombre de la nueva funcionalidad donde agregaremos nuestros cambios.

Por defecto cuando creamos un repositorio tiene una rama llamada master. (Como buena practica nada se desarrolla en master).Utilizamos ramas para experimentar y hacer cambios.
Branching o ramificación es la manera de trabajar en diferentes versiones de un repositorio a la vez.<br>



**Comandos:<br>**

- git branch [nombre de la rama]<br>

- crea una nueva rama<br>

- git branch<br>

- enlista todas las ramas en el repositorio actual<br>

- git branch -d [nombre de la rama]<br>

- borra la rama especificada<br>

- git checkout [nombre de la rama]<br>

- cambia a la rama especificada<br>
<br>
Una vez que hayas probado la nueva funcionalidad y comprobado que cumple el objetivo; estamos listas para mover ese desarrollo a la rama master. Es decir, necesitamos hacer un merge.<br>

- git merge[nombre de la rama]

combina el historial de la rama especificada con la rama actual
Algunas veces, cuando queremos fusionar dos ramas no resulta tan bien, podemos generar un conflicto.

Un conflicto en git se produce cuando se edita la misma linea de código en dos instancias distintas de trabajo y luego se intentan fusionar.Git no puede decidir cual versión elegir y te avisa que tu debes resolverlo; nos proporciona una ayuda diciéndonos que archivo tiene el conflicto, el cual al abrirlo en nuestro editor, nos muestra cuales son los cambios que entran en conflicto.

Tenemos que elegir entre lo que está entre <<<<<<< HEAD y ======= que es contenido que tenemos en la rama donde estamos haciendo el merge o entre ======= y >>>>>>> contenido donde están los cambios hechos en la rama que queremos unir.Arreglamos los cambios elegidos, guardamos, agregamos y hacemos commit de los cambios. De esta manera resolvemos el conflicto y logramos hacer merge con éxito.Otra ventaja de trabajar con git es que podemos colaborar en otro proyectos.

**Algunos conceptos que debes saber son:**

<br><br><br>
![Git](https://miro.medium.com/max/573/1*J36wXW8VsBYnd8cc0p6QOA.png)

- Fork: hace una copia exacta de un repositorio; creando un nuevo en tu cuenta de Github con una url diferente que podemos utilizar como un repositorio git cualquiera. Tendremos dos repositorios independientes y cada uno evoluciona de forma autónoma.

- Pull request: es una petición que el propietario de un fork de un repositorio hace al propietario del repositorio original para que este último incorpore los commits que están en el fork.

Los pasos a seguir para trabajar de forma colaborativa son:
<br><br><br>
![Git](https://miro.medium.com/max/700/0*hPn4TNfoCGT2FSCf.png)

- Hacer fork desde la interfaz de github del proyecto en el cual queremos colaborar.

- Se clona el repositorio creado.

- Crear una nueva branch para desarrollar nuestra aportación.
Realizar commits para describir las modificaciones y/o aportaciones.

- Se hace push de las modificaciones en nuestra copia del repositorio.
Se pide un pull request desde la interfaz de github.<br>
<br><br><br><br>
# Cómo colaborar en un proyecto en GitHub
- Fork del repositorio
- Clonar el repositorio
- Actualizar la rama master
- Crear una rama
- Hacer los cambios
- Hacer un Pull Request
# Fork del repositorio
El primer paso es hacer "Fork" del repositorio.

# Clonar el repositorio
Después de tener el repositorio en nuestra cuenta, seleccionar la dirección del repositorio "SSH o HTTP" y clonar:

$ git clone https://github.com/User/NombreRepo.git

Dentro de la carpeta que genera, comprobar la URL del repositorio:

$ git remote -v

Antes de realizar modificaciones agregar la URL del repositorio original del proyecto:

$ git remote add upstream https://github.com/User/RepoOriginal(Forkeado)

Comprobar

$ git remote -v

# Actualizar la rama Master
Antes de empezar a trabajar, obtener los últimos cambios del Repo Original:

$ git pull -r upstream master

# Crear una Rama
Para crear una rama usar la opción "checkout" de git:

$ git checkout -b feature-nombre-rama

# Hacer cambios
Realizar todos los cambios que se desea hacer al proyecto.

Agregar los archivos y hacer un commit

Después de realizar el commit hacer el push hacia nuestro repositorio indicando la rama que hemos creado.

$ git push origin feature-nombre-rama

# Hacer un Pull Request
Hacer click en "Compare & Pull Request"

Escribir cambios del Pull Request.

Si todo está bien, enviar con el botón "Send Pull Request".

Esperar a que el duelo del repositorio lo revise, acepte y mezcle en la rama correspondiente.

<br><br>
# **Conclusion**
<p>En este reciente trabajo, pudimos comprender más la funcionalidad de Git a la hora de trabajar en equipo, esto con comandos que nos ayudarían más adelante a poder trabajar en conjunto tango en Git como en Github y su flujo de trabajo

## **Bibliografia**

- https://medium.com/laboratoria-how-to/tú-y-yo-usando-git-colaborativo-no-se-piénsalo-62dea67aa2eb
- https://gist.github.com/BCasal/026e4c7f5c71418485c1

 