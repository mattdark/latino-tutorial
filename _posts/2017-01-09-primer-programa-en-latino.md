---
layout: post
title:  "Primer programa en Latino"
image: '/assets/img/latino-banner.png'
date:   2017-01-09 16:45:00
tags:
- latino
description: ''
categories:
- latino
serie: learn
---


Una vez que Latino está instalado, puedes empezar a escribir código en  este lenguaje, ya sea desde la consola interactiva o creando un archivo con la extensión .lat que contendrá el código fuente del programa. 

## Escribir código desde la consola interactiva

Si estás leyendo esto desde tu distribución GNU/Linux favorita, abre la terminal y ejecuta el siguiente comando:

{% highlight bash %}
latino
{% endhighlight %}

En la terminal debe aparecer la consola interactiva de Latino.

{% highlight bash %}
Latino 0.9.0
Todos los derechos reservados (C) 2015-2016. Latinoamerica
latino>
{% endhighlight %}

Debes escribir el código del programa línea por línea. Para mostrar texto en pantalla, existen dos funciones, **escribir()** e **imprimir()**, y dentro de los paréntesis se coloca entre comillas el texto que se quiere mostrar. Para escribir el típico **¡Hola mundo!** se escribe la función, luego se debe presionar Enter y la consola mostrará la salida correspondiente.

{% highlight bash %}
latino> escribir("¡Hola mundo!")
¡Hola mundo!
{% endhighlight %}

{% highlight bash %}
latino> imprimir("¡Hola mundo!")
¡Hola mundo!
{% endhighlight %}

## Crear archivo con el código fuente

Un archivo que contiene código fuente de Latino tiene la extensión **.lat**. Escribir el código anterior en un archivo, puedes usar tu editor de texto preferido. Se debe ejecutar con el siguiente comando:

{% highlight bash %}
latino hola.lat
¡Hola mundo!
{% endhighlight %}

Espero que esta información sea de utilidad. En el siguiente post publicaré el primer ejemplo. Si tienes alguna pregunta, no olvides consultar el sitio de Latino ([lenguaje-latino.org](http://lenguaje-latino.org/)).
