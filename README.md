# eteams
Página de login

![image](https://user-images.githubusercontent.com/73826471/169762624-80b16ce5-995c-4b32-aea1-79c5e5bae1c4.png)

Esta será la primera pantalla de nuestra app. De aquí salen 2 opciones que dependerán de si el usuario está registrado o no.
Si está registrado accederá a la pantalla de inicio, en caso de no estarlo, tendra que registrarse y pasará a la siguiente pantalla.
Back
Que recuerde la contraseña en el equipo y es que se pulsa el botón, se hará a través de cookies y un atributo en la base de datos con true or false.
Aquí tendremos que configurar las variables de sesión. 
Front:
En caso de clicar en el link de que has olvidado la contraseña tendrá que abrirse un pop up donde se pueda cambiar. (En este PMV** se gestionará de esta forma).
Tendrá 3 inputs (email, contraseña nueva, repite nueva contraseña) y 2 botones cancelar, aceptar.

**Producto mínimo viable

Pagina de Sing in:
![image](https://user-images.githubusercontent.com/73826471/169762688-33db0197-70d0-43e8-bbb6-d5822a813931.png)

Esta página será donde se creen los nuevos usuarios, una vez creado el usuario, iremos a la pantalla anterior para que inicien sesión.
Por otro lado el link de política de privacidad nos llevará a una página que copiaremos de la PP de (LinkedIn).

** Tendrá que poner correo igual que en la página anterior (NO EMAIL)

Página de creación del perfil


Esta es la primera página que va a ver un nuevo usuario. En ella podrá cambiar el tipo de usuario, y rellenar sus datos. (El tipo EMPRESA de usuario solo es relevante en versiones posteriores de nuestra APP).

En caso de que fuera una cuenta de EQUIPO tendría que aparecer un apartado en el que se pudieran añadir a los usuarios participantes. 
A este usuario le aparecerá una notificación que si acepta aparecerá en su perfil que es miembro del equipo.
Por lo que los usuarios que se agreguen al equipo tendrán estados (esperando, aceptado)
Podremos acceder a esta página de configuración desde nuestro perfil pulsando el lapicito (el cual hay que cambiar por el  ).


En este desplegable que se muestra a continuación, si clickeamos contacto, saltará un popup con estructura de correo donde cualquier usuario podrá mandar una sugerencia, duda o queja. El apartado configuración no estará disponible en este primer PMV.




Página de perfil

   
Esta será la página de perfil de cualquier usuario gamer. Si el usuario fuera de tipo equipo tendrán que aparecer cuántos miembros forman un equipo y que al clickar apareciera un popup con los integrantes (del estilo que cuando se hace click para ver quien le dio a me gusta a una publicación )

En caso de ya seguir al usuario del perfil en el botón aparecerá “Dejar de seguir”
En comentarios, en caso de poner un @ se abrirá un pop up donde aparecerán tus contactos. (si alguien es mencionado aparecerá en notificaciones )
Si clicamos en el  saldrá un popup que nos dejará hacer drag and drop o navegar por las carpetas del equipo (esto último al hacer click en el icono).



saldrá un desplegable con iconos.
Los  abrirá un pop up donde vendran las siguientes opciones
Denunciar → saltara otro popup de confirmación//cancelación



Si clicamos en el número de los comentarios saldrá un pop up que pondrá la lista de las persona que le dieron a me gusta.

Se clickmos en “compartir”  saldra un pop up dandonos a elegir si queremos mostrarlo en nuestro tablon como un post o mandarlo por mensaje privado.





En caso de que el usuario esté viendo su propio perfil, (al cual llegará a través de  , clicando en el botón “ver perfil” del desplegable). El iconito se volverá lila y en este caso no aparecerá el botón lila de seguir

Página de Perfil - FOTOS y VIDEOS

Al clicar en una foto aparecerá un pop up con el post que contiene la foto en cuestión mostrando los detalles del post. Este pop up funcionará igual que si estuviéramos viendo el post en el tablón.



Página de mensajes

Cuando los mensajes no hayan sido leídos aun se pondrá un circulito lila al lado de la conversación.

Para el correcto funcionamiento de los mensajes, deberíamos de tener en cuenta que necesitaremos 2 colecciones.
1- conversación- tendrá dos usuarios, y mensajes.
2- mensaje- tendrá un emisor, un receptor, un contenido, una fecha, un estado

Para colocar las conversaciones lo haremos a través de la criba de las conversaciones que tenga cada usuario, y las colocaremos según la fecha del último mensaje.
Según el estado de los mensajes, la conversación saldrá como leída o no.
Hay que tener en cuenta de que cada vez que se produzca un mensaje, tendrá que generarse un evento que consiga que el icono de los mensajes se ponga así 


Página Home//Inicio


Aquí aparecerán por fecha reciente los post de las personas a las que sigues.
Buscador

En esta pantalla aparecerán post y personas a las cuales no seguimos.
Llegaremos aquí a través de la realización de una búsqueda.
En principio aparecerán tanto posts como personas.
después a través de la elección de etiquetas Usuarios o Post, podremos cribar entre unos u otros.
Para el funcionamiento de esta pantalla, lo que vamos a hacer es que tanto los usuarios como los post, tengan un atributo iteraciones que haga el cálculo de todo tipo de interacciones que tengan.
En función de este atributo se ordenan por relevancia.
**Ojo!! las personas siempre van a tener más interacciones que los post, tendremos que pensar en algo para igualar relevancia…

Notificaciones

En esta página van a salir todas las notificaciones de un usuario. Estas notificaciones vendrán a través de un evento en los siguientes casos, (cada caso con su copy acorde).
 
Cuando un usuario me siga.
Cuando le den a me gusta a un post.
Cuando le den a me gusta a un comentario.
Cuando comenten en un post mio.
Cuando comenten en un comentario mio.
Cuando me mencionen
Cuando compartan mi contenido.
Cuando se solicite un equipo que forme parte de él
—-----------
Siendo un equipo: Cuando un integrante acepte formar parte del equipo.


