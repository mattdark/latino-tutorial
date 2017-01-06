---
layout: post
title:  "Instalar Latino en Ubuntu"
image: ''
date:   2017-01-06 07:15:00
tags:
- latino
description: ''
categories:
- latino
serie: learn
---


En este post explicaré como instalar Latino en Ubuntu, si necesitas instalar en otro sistema operativo, puedes consultar la información disponible en la página, descargar e instalar Latino desde aquí: [lenguaje-latino.org/descargar](http://lenguaje-latino.org/descargar).

Antes de instalar Latino en Ubuntu, asegurate de tener instaladas todas las dependencias, para ello ejecuta el siguiente comando en la terminal:

{% highlight bash %}
sudo apt install git bison flex cmake gcc g++ libjansson-dev libcurl4-openssl-dev libhiredis-dev redis-server curl
{% endhighlight %}

Es probable que te muestre algún mensaje de error al intentar compilar, si fuera el caso instala también los siguientes paquetes:

{% highlight bash %}
sudo apt install build-essential libgtk-3-dev
{% endhighlight %}

Una vez que tengas todas las dependencias instaladas, escribe los siguientes comandos en la terminal:

{% highlight bash %}
git clone --recursive https://github.com/primitivorm/latino
cd latino
git submodule update --init --recursive
cmake .
make
sudo make install
{% endhighlight %}

Para comprobar que la instalación ha salido bien, ejecuta el siguiente comando en la terminal:

{% highlight bash %}
latino
{% endhighlight %}

En la terminal debe aparecer la consola interactiva de Latino.

{% highlight bash %}
Latino 0.9.0
Todos los derechos reservados (C) 2015-2016. Latinoamerica
latino>
{% endhighlight %}

Ahora puedes programar en Latino.
