---
layout: post
title:  "Por qué usar Jekyll para tu blog?"
date:   2015-08-16 13:10:53
categories: jekyll
---
Tiene rato que quiero empezar mi propio blog. Actualmente soy Desarrollador Web de tiempo completo trabajando principalmente con tecnologías Open Source.

A lo largo de mi tiempo como desarrollador he "pepenado" (copy-paste) más código, del escrito por mi mismo. 

La filosofía Open source es precisamente compartir código. Mientras que la filosofía Unix nos dice que hagamos funciones sencillas que funcionen y funcionen bien.


Gracias a diferentes proyectos he podido trabajar con Wordpress, Drupal, Mezzanine y Blogspot. De los cuatro el que más recomiendo es Wordpress, en mi opinión la interfaz administrativa es la mejor, bastante intuitiva que te permite crear contenido presentable y rápido. Adicionalmente es fácil encontrar un desarrollador que le sepa mover; cuenta con un número grande de templates y aún más de widgets. Inclusive no solo para blogging, he visto startups que corren su prototipo en Wordpress y así lo sacan al mercado, no se requiere ser un desarrollador, basta con seguir un par de tutoriales para levantar tu primer Wordpress, por tanto tu costo de inversión es bajo.

Entonces por qué Jekyll?

Bueno, como desarrollador levantar un blog localmente con Jekyll, es cosa de 3 comandos:

{% highlight ruby %}
$ gem install jekyll
{% endhighlight %}

Nota: Tomaré por hecho que sabes dónde ejecutar este comando, en caso de que no, te recomiendo te avientes un tutorial de "cómo instalar paquetes ruby".

Listo, ya tengo Jekyll <b>instalado</b>, ahora simplemente tengo que crear un proyecto el cuál será mi blog:

{% highlight ruby %}
$ jekyll new dev-blog
{% endhighlight %}

Jekyll es un paquete de ruby que al mandarle la palabra "new" y dándole un nombre, en este caso "dev-blog" se encarga de generar una estructura de archivos bajo la carpeta "dev-blog", los cuales conforman mi blog.

Es importante mencionar que no tendre una Base de Datos, por tanto mi blog no tendrá registro de usuarios (por el momento), ni comentarios. Lo que me importa ahorita es "tener mi blog y tenerlo bien". Y para eso Jekyll me da la solución que estoy buscando, es por eso que lo prefiero sobre Wordpress. Porque como desarrollador me facilita los procesos de: <b>Instalación, Redacción y Publicación.</b>

OK, y el tercer comando?

El tercer comando es meterme al proyecto (carpeta) recién creado y ejecutar:

{% highlight ruby %}
$ jekyll serve
Server address: http://127.0.0.1:4000/
{% endhighlight %}

<div class="printscreen">
	<img src="https://s3-us-west-2.amazonaws.com/challenge-202/esp/porque-usar-jekyll/jekyll-instalacion.png" alt="jekyll instalacion"/>
	<p>Comandos para instalar Jekyll</p>
</div>

Listo, mi blog ya está corriendo de manera local, entonces ahora es momento de lo bueno: <b>Redacción</b>.

Yo la redacción la hago en un documento de google, pues me ayuda con los horrores ortográficos y a tener el contenido accesible 24-7. Una vez que ya estoy satisfecho con mi contenido entonces me voy a Sublime y abro la carpeta del blog.

Dentro de la carpeta "_posts" modifico el primero archivo que Jekyll da por default. Le cambio el nombre al archivo, le pego el contenido y ajusto tags. Listo, mi primer post.

<div class="printscreen">
	<img src="https://s3-us-west-2.amazonaws.com/challenge-202/esp/porque-usar-jekyll/jekyll-proyecto-sublime.png" alt="jekyll estructura proyecto sublime"/>
	<p>Estructura del proyecto vista en Sublime</p>
</div>

Como el Servidor está corriendo localmente, y Jekyll es lo suficientemente inteligente para detectar cambios en los archivos, entonces cada que guardo mis ajustes, puedo ver en el navegador los cambios reflejados (refrescando obviamente).

El blog está corriendo de manera local en la dirección: `http://127.0.0.1:4000/`
Al abrir este link en el navegador (obvio Chrome) veré la página que viene por default, así como el título del primer post que estamos apenas generando.

<div class="printscreen">
	<img src="https://s3-us-west-2.amazonaws.com/challenge-202/esp/porque-usar-jekyll/jekyll-homepage.png" alt="jekyll pagina default"/>
	<p>Página por default de Jekyll</p>
</div>

Nota: Si no estas relacionado con `127.0.0.1`, te recomiendo leas "Qué es un servidor local".

Si le doy click al título veré mi primer post (ouh yeah).

<div class="printscreen">
	<img src="https://s3-us-west-2.amazonaws.com/challenge-202/esp/porque-usar-jekyll/jekyll-primer-post.png" alt="jekyll primer post"/>
	<p>Primer post en Jekyll</p>
</div>

Y la <b>publicación</b>?

Bueno la "publicación" quedará para otro post, pues hay otros ajustes en otros archivos que quiero hacer antes de oficialmente sacar este blog al ciberespacio. 

Con esto termino este primer post,
Gracias por leerlo.

<br />
Referencia: Página oficial de [Jekyll][jekyll].

[jekyll]:   http://jekyllrb.com/
