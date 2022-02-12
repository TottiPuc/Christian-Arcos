---
title: "Nomenclatura básica de redes neuronales"
date: 2022-02-09
tags: [redes neuronales]
header:
  image: "/images/perceptron/nomenclatura.jpg"
excerpt: "Nomenclatura redes neuronales"
mathjax: "true"
---

Uno de los problemas más frecuentes cuando escribimos un artículo o leemos sobre temas complejos como redes neuronales, es sin duda alguna entender la nomenclatura asociada a cada fórmula, es por eso que en este apartado hablaremos sobre como entender de una manera práctica y sencilla las nomenclaturas usadas en AI.
 
Vamos a suponer que queremos realizar un clasificador binario que nos diga si existe o no un perro en la siguiente foto
 
<figure style="width: 40%" class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/images/nomenclatura/ZEUS.png" alt="golden">
</figure>  
 
esto es:
 
1 --> (perro)

0 --> (no perro)
 
donde 0 y 1 representan la salida de nuestro clasificador , matemáticamente representado por la letra 'y'  también conocida como etiqueta o label
 
Sin embargo, presentar una imagen a un computador y que la interprete no es una tarea simple, ya que las imágenes tradicionales que conocemos son la representación de una matriz de números con diferentes valores (conocidos como pixeles), los cuales representan la intensidad del color. Sin embargo no solo se trata de una matriz que representa todos los posibles colores, cada color viene representado por su propia matriz, asi al final una foto tradicional en el formato RGB no es más que una superposición de capas con diferentes colores, como se puede ver en la siguiente imagen.

<figure style="width: 40%" class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/images/nomenclatura/rgb.png" alt="rgb">
</figure> 

 
Ahora, asumiendo que nuestra imagen es de un tamaño de 64x64 pixeles, lo que quiere decir que cada canal de color tambein tiene la misma dimension, es hora de presentarle esa informacion a nuestro ordenador, pero para eso estas intensidades de color (pixeles) se deben presentar como un vector de caracteristicas donde cada fila de nuestras matrices RGB sera puesta en una sola columna una detras de otra para formar asi un vector de características de 1xN, donde N sera la dimensión de nuestra imágen en nuesro ejemplo (64x64).


<figure style="width: 70%" class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/images/nomenclatura/vectores.png" alt="vector">
</figure> 
 
de esta forma nuestro vector (X) de características de entrada será representado por:
 
$$ N_{x}= 12288 $$

