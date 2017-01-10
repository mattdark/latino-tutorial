---
layout: post
title:  "Suma de tres números"
image: '/assets/img/latino-banner.png'
date:   2017-01-13 10:00:00
published: false
tags:
- latino
description: ''
categories:
- latino
serie: learn
---

El código en Latino que permite realizar la suma de tres números es el siguiente:

{% highlight python linenos %}
# Suma de tres numeros
escribir("Introduce un numero")
a = leer()
escribir("Introduce un numero")
b = leer()
escribir("Introduce un numero")
c = leer()
suma = a + b + c
escribir("La suma es: " . suma)
{% endhighlight %}

## Obtener un valor del usuario

Para pedir datos al usuario y que los instroduzca desde el teclado se usa la función **leer()**. En el código de arriba se usa la función para pedir cada número que debe sumarse, cada valor introducido por el usuario se almacena en una variable (**a**, **b** y **c**).

## Comentarios
En programación los comentarios son líneas de código que sirven para agregar información sobre el programa y así comprender que es lo que hace, por ejemplo, para que sirve una variable, que hace una función, etc. Además, los comentarios no se muestran cuando se ejecuta el programa. En Latino se pueden agregar comentarios como se muestra a continuación:

{% highlight python %}
# Este es un comentario de una línea
{% endhighlight %}


{% highlight python %}
// Este es otro comentario de una línea
{% endhighlight %}

{% highlight python %}
 /*
 Esto es un comentario
 que tiene
 varias
 líneas
 */
{% endhighlight %}

## Operación

En Latino el operador de suma es **+**. El resultado de la operación se almacena en la variable **suma**.

## Imprimir resultado

Para concatenar se usa el punto, por lo que la salida del programa será: **La suma es: valor_suma**. Imprimiendo el texto y el valor de la variable **suma** en la misma línea.

Puedes comprobar el código anterior ejecutando el código desde la consola interactiva o bien desde un archivo con la extensión **.lat**.
