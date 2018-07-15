---
title: "¿Cuanta energía solo por moverse?"
layout: post
cover: assets/images/estiramiento-en-el-parque_925x.jpg
navigation: true
date: '2018-07-15 14:15:20'
categories: salud
class: post-template
subclass: post
author: leonel
tags:
- salud
---

Existen muchas publicaciones acerca de la energía que consumimos, pero ¿Cómo tener una estimación simple de esta cantidad?  ¿Cómo se calculan esos 2,000 calorías de una dieta “normal”? ¿Cómo funcionan las aplicaciones Smartphone para este propósito? ¿Podemos calcularlo sin una app? Y las preguntas siguen. Este post pretende mostrar una simple y razonable manera de calcular nuestras calorías sólo por mover nuestro cuerpo.

El concepto básico detrás de esto, viene de la Mecánica clásica, pero no te asustes, es más simple que eso. La fórmula establece que la energía se calcula como la multiplicación entre fuerza y distancia.

**W=F*d**

Lo anterior es la expresión matemática y si consideramos, idealmente, que sólo moveremos nuestro peso, entonces necesitamos esta cantidad y la distancia (utilizaremos las unidades del Sistema Internacional).

![](/assets/images/mecanica-clasica-fuerza-y-distancia.png)

Las unidad de fuerza se mide en Newton (N) y la “magia” ocurre de la siguiente manera:

**F=m*g**

Donde m: es la masa de tu cuerpo en kilo-gramos (kg)
								 g: gravedad en m/s2

Finalmente las Unidades de la Fuerza son:
Funits = kg.m/s2=N


Los pasos para que hagas los cálculos tú mismo:

1. Toma tu peso en kilo-gramos (kg).
2. Considera una gravedad con un valor de 9.81m/s2.
3. Toma un valor aproximado de la distancia que caminas en kilo-metros (km).

O usa la calculadora de energía:

Your weight in kg : <input id="firstNumber" type="text" /><br /><br />
Distance you move in km:<input id="secondNumber" type="text" /><br /><br />
<input onclick="multiplyBy()" type="button" value="Calculate Energy" /><br /><br />

<b><span style="font-size: medium;">The Result is : </span></b><br /><br />
<b><span id="cals" style="font-size: 250%">0</span> food calories</b><br />

<script>
function multiplyBy()
{
	var calo=0;
    num1 = document.getElementById("firstNumber").value;
    num2 = document.getElementById("secondNumber").value;
	calo = parseFloat(document.getElementById("cals").innerHTML = Math.round((num1 * num2 * 9.81)/4.184)).toFixed(2);
}

</script>

Explicaremos las calorías pronto!

[English Version](http://central-hub.blogspot.com/2018/06/how-much-energy-just-for-moving.html)