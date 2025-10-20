# Chuleta-Git

Esta es una chuleta básica con las normas de buenas prácticas para trabajar en equipo en un mismo proyecto.
Incluye también un listado de los diferentes comandos con su explicación y ejemplos prácticos.
Se ha añadido un archivo index.html para aprovechar y practicar un poco más otros componentes de Bootstrap, como elementos colapsables o carruseles.

Lista de normas:
- Lo que no te toca no se toca
- No se trabaja en main
- No se trabaja en develop
- Siempre hacer push a tu rama de trabajo
- Los commits y las ramas deben tener nombres descriptivos
- Antes de un push, se hace un pull de develop
- Antes de empezar a trabajar, se hace un pull de develop
- Al crear ramas nuevas, hacer un push para crearlo en Github
- Cuando se incluyan cambios en develop, hacer un pull
- Si hay conflicto en el código, usar el editor interno de Github (es más sencillo, tendrás menos problemas).

Lista de comandos -> Explicación -> Ejemplo práctico

git add . -> Añade todos los cambios de todos los archivos en el stage (el punto intermedio entre local y remoto) -> Cuando has terminado de trabajar por el momento y quieres preparar los archivos modificados o creados para almacenarlos en la nube y compartirlos
git add "nombre del archivo" -> Añade solo ese archivo con los cambios hechos -> En caso de querer preparar sólo un archivo o archivos concretos
git add *.js / git add archivo.* -> El asterisco sirve para indicar "todo". Los ejemplos son "todo archivo con extension .js"/"todo archivo que se llame así, con cualquier extensión". NO CARPETAS -> Para preparar solo archivos con un mismo nombre o extensión.
git commit -m "mensaje" -> Guardas localmente todos los archivos que añadiste con el add como grupo con un mensaje DESCRIPTIVO de los cambios que has realizado. -> Tras usar el add. Es la forma de aplicar un mismo mensaje descriptivo a todos los archivos,
git push origin "rama" -> Siendo el origin el lugar al que lo envias y la rama el nombre del branch en el que estás trabajando, envías todo el contenido y cambios que has realizado en ella al repositorio que has marcado como origin -> Para enviar el commit anterior al servicio en la nube.
git pull -> Traes el contenido de la rama a la que se lo pides ACTUALIZADO (cuidado, puede cambiar antes de que envíes lo tuyo). Aqui surgen los conflictos, ya que intenta fusionar lo que hay en remoto con lo que tienes en local, vigila. -> Cada vez que se vaya a empezar a trabajar con contenido compartido y antes de enviar en lo que tú has estado trabajando, porque así te aseguras que lo que tienes está actualizado.
git remote -v ->Nos dice de dónde estamos sacando la información remota. El -v nos da la dirección del repositorio de origen (normalmente enlace de Ghithub). ->Puede ayudarnos a asegurarnos de que estamos sacando la información y la estamos enviando al sitio correcto.
git branch -> Nos aparece en formato "* nombre". El asterisco indica que estamos trabajando en ella. -> Nos aseguramos de que no estamos tocando en la rama "main/master"
git checkout "nombre" -> Nos permite cambiar entre ramas existentes -> La usaremos para poder trabajar en diferentes ramas de forma paralela. 
git checkout -b "nombre" -> Creamos una rama NUEVA con el nombre que le indiquemos y nos mueve a ella -> En caso de empezar a trabajar en otro objetivo, crearemos una nueva rama hasta que lo tengamos todo terminado y funcionando como debe.
git fetch -> Dice si en el remoto ha habido cambios, pero es solo informativo ya que no aplica cambios -> *Suposición más que certeza* Podemos comprobar si el pull es necesario AUNQUE SIEMPRE ES NECESARIO
git branch -a -> Listado de todas las ramas que existen -> Podemos comprobar los diferentes elementos en los que se está trabajando de forma paralela.
git status -> Lista de los cambios realizados antes de hacer el commit. Nos da los nombres de los archivos editados y si son nuevos, modificados o borrados -> Podemos asegurarnos de que los cambios están en los archivos que deben
git diff -> Diferencias EXACTAS que hay por las modificaciones -> Nos aseguramos de que los cambios son correctos.
git merge rama -> Fusiona la rama que le nombras con la rama en la que estás -> En caso de elementos en los que se ha trabajado de forma paralela pero que se necesitan o complementan para funcionar.