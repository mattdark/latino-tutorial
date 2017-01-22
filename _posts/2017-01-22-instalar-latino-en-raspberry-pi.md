---
layout: post
title:  "Instalar Latino en Raspberry Pi"
image: ''
date:   2017-01-22 00:00:00
tags:
- latino
description: ''
categories:
- latino
serie: learn
---

<img src="/latino-tutorial/assets/img/latino-banner.png" alt="Latino banner">

Instalé Ubuntu hace tres meses, la versión 16.04, que actualicé un mes después a 16.10. Es la distribución que he usado desde entonces y por eso el post anterior sobre la instalación de Latino en Ubuntu. Sin embargo, la distribución que uso habitualmente es Manjaro, que reinstalaré en algún momento dentro de los próximos meses. He instalado Arch Linux ARM en una Raspberry Pi B+ y a continuación explico el proceso de instalación de Latino.

Antes de instalar Latino, asegurate de tener instaladas todas las dependencias, para ello ejecuta el siguiente comando en la terminal:

{% highlight bash %}
sudo pacman -S git base-devel cmake jansson hiredis redis curl gtk3
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
Latino 0.9.1
Todos los derechos reservados (C) 2015-2016. Latinoamerica
latino>
{% endhighlight %}

El proceso de instalación debe funcionar en Manjaro o en Arch Linux si tienes instalado alguno de estos sistemas en tu laptop o PC.
