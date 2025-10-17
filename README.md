# Chuleta-Git

Esta es una chuleta básica con las normas de buenas prácticas para trabajar en equipo en un mismo proyecto.
Incluye también un listado de los diferentes comandos con su explicación y ejemplos prácticos.

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

Lista de comandos:

git add . -> Añade todos los cambios de todos los archivos en el stage (el punto intermedio entre local y remoto).
git add "nombre del archivo" -> Añade solo ese archivo con los cambios hechos.
git add *.* -> El asterisco sirve para indicar "todo lo que tenga extensión". Si el asterisco está detrás del punto, es para todas las extensiones. Si está antes del punto, sirve para añadir todos los archivos de una extensión. NO CARPETAS
git commit -m "mensaje" -> Guardas localmente todos los archivos que añadiste en el add como grupo con un mensaje DESCRIPTIVO de los cambios que has realizado.
git push origin "rama" -> Siendo el origin el lugar al que lo envias y la rama el nombre del branch en el que estás trabajando, envías todo el contenido y cambios que has realizado en ella al repositorio que has marcado como origin. Envias el commit anterior.
git pull -> Traes el contenido de la rama a la que se lo pides ACTUALIZADO (cuidado, puede cambiar antes de que envíes lo tuyo). Aqui surgen los conflictos, vigila.
git remote -v ->Nos dice de dónde estamos sacando la información remota. El v nos da la dirección del repositorio de origen (normalmente GHithub)
git branch -> Noa parece en formato "* nombre". El asterisco indica que estamos trabajando en ella. 
git checkout "nombre" -> Nos permite cambiar entre ramas existentes
git checkout -b "nombre" -> Creamos una rama NUEVA con el nombre que le indiquemos y nos mueve a ella. 
git branch -a -> Listado de todas las ramas que existen.
git status -> Lista de los cambios realizados antes de hacer el commit. Nos da los nombres de los archivos editados y si son nuevos, modificados o borrados.
git diff -> Diferencias EXACTAS que hay por las modificaciones. 
git merge rama -> Fusiona la rama que le dices con la rama en la que estás.
