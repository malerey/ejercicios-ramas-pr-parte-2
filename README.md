# Ramas y PRs en github

Vamos a seguir trabajando con el repo que creaste en los ejercicios anteriores. 

## Creando un PR 

1. En este momento, tu repo local y tu repo remoto en github tienen cuatro ramas: main, rojo, verde y azul.
2. Vamos a hacer un PR desde `rojo` para que los cambios que hicimos allí se vean en `main`. 
3. Desde la consola, navegá a la rama `rojo`. 
4. Modificá el README para que diga "Cambios en la rama rojo que se van a agregar a la rama main`. 
5. Agregá los cambios y hacé un commit. 
6. Hacé un push. 
7. Andá a github. Vas a ver que ahora hay un cartel amarillo que te dice que hiciste push recientes a la rama `rojo`, y te invita a hacer un nuevo Pull Request. 
8. Hacé click en el botón para hacer un nuevo PR (dice "Compare & pull request".
10. Se va a abrir un formulario. Ahi podes agregarle un titulo a tu PR, en donde describis brevemente de que se trata tu cambio. Tambien hay un area mas grande en donde podes agregar mas detalles. Esto es muy util cuando haces muchos cambios. Mas abajo, nota que tenes un detalle de los cambios en tu codigo: a la izquierda vas a ver tu rama main, y a la derecha vas a ver los cambios que hiciste en la rama nueva. 
11. Una vez terminado tu recorrido, hacé click en el botón verde que dice "Create pull request" 
12. Luego de que se actualice tu pagina, vas a ver que ahora en el formulario hay un boton que dice "Merge pull request". **No le des click todavía**
13. Volve a tu repo de github y confirma que ahora bajo la pestaña Pull Request esta el PR que acabas de crear
14. Repeti todos estos pasos para tus ramas verde y azul. 

### Comentarios

Crear un Pull Request significa: Hice cambios en mi rama, y ahora quiero que esos cambios se integren en la rama principal. 

Trabajamos de esta manera porque si todas trabajaramos sobre la rama main, seria muy dificil mantener el orden. 

La idea de un Pull Request es que otra persona, generalmente el lider del equipo, sea el responsable de aceptar ese PR. De esa manera tiene la oportunidad de leer nuestro codigo y aprobar los cambios antes de aceptarlos. 

Hacer un Pull Request **no es** integrar nuestros cambios a la rama main sin mas. Hacer un Pull Request es hacer un **pedido**: pedir que nuestros cambios se vayan a la rama main. 

## Mergeando un PR

1. En este momento deberias tener 3 Pull Request: uno por cada uno de tus ramas. 
2. Anda al Pull Request de la rama `verde`. 
3. Ahora sí, hacé click en el botón "Merge pull request".
4. Te aparecerá otro botón que dice "Confirm Merge". Hace click. 
5. Te deberia aparecer otro cartel que dice "Pull request successfully merged and closed". Tambien te da la opcion de borrar la rama actual. No es necesario hacerlo. 
6. Volve a la pagina principal de tu repo. 
7. Confirma que ahora en el README se ven los cambios de tu rama `verde`.
8. Confirma que ahora solo tenes dos Pull Request en la pestaña. 

### Comentarios

Darle Merge a un Pull Request significa: Acepto los cambios en este Pull Request, y voy a integrarlos a la rama main. 

Es **aceptar** el pedido que implica el Pull Request que hicimos antes y modificar la rama main. 

En el mundo laboral, generalmente está reservado al lider del equipo. 

## Obteniendo los nuevos cambios en nuestro local

1. En este momento la rama `main` esta actualizada con los cambios de la rama `verde` en el repo remoto de github. 
2. Anda a la consola. 
3. Confirma que estas en la rama `main`. 
4. Abri tu README: **no** deberias ver los cambios de la rama `verde`. ¿Por qué pensás que no los podés ver?
5. Corré el comando `git pull`. 
6. Ahora si, deberias ver tu README actualizado. 

### Comentarios

Un Pull Request modifica **el repositorio remoto que está en github**. No modifica tu repositorio local. 

Cuando alguien hace cambios en el repositorio remoto, debemos hacer `git pull` para traernos los cambios a nuestra rama. 

*¿Por qué es importante tener esto en cuenta?*

Cuando estamos trabajando de a muchas personas, hablamos de la importancia de crear nuevas ramas siempre a partir de la rama `main`. Si creas un Pull Request, tus cambios se integran a la rama main. Pero si no actualizas tu rama main, cuando vayas a crear una nueva rama esa rama va a estar desactualizada: no va a tener tus ultimos cambios, ni los de tus compañeras. 

Cada vez que vas a crear una nueva rama desde `main`, debemos primero hacer `git pull` para tener siempre nuestra rama `main` actualizada. 


## Trabajando con una compañera

1. Dale acceso como colaboradora a tu repo a una compañera. 
2. Pedile que clone tu repo, y cree una nueva rama que se llame `prueba-de-a-dos`. 
3. Pedile que modifique el README para que tenga un nuevo párrafo que diga "Este parrafo fue agregado por {nombre}". 
4. Pedile que agregue los cambios, haga un commit, y un push. 
5. Pedile que haga un Pull Request, pero que no lo acepte. 
6. Una vez que tu compañera haya hecho el Pull Request, va a ser tu tarea revisarlo y aceptarlo. 
7. Confirma que puedas ver los cambios de tu compañera en github. 
8. Hace `git pull` de main y confirma que podes ver los cambios de tu compañera en tu repo local. 


