---
title: "GPU conceptos basicos"
date: 2020-07-05
header:
  image: "/images/GPU/GPU1.PNG"
excerpt: "Machine Learning, Perceptron, Neural Network"
mathjax: "true"
---


En este artículo hablaremos de las Unidades de Procesamiento Grafico o *(GPU)* por sus siglas en ingles  

{% include figure image_path="/images/GPU/gpus.PNG" alt="gpu tesla" caption="GPUs Nvidia"%}


Uno de los principales conceptos cuando se habla de *machine learning* es el de programación paralela, muchos de los procesos realizados en algoritmos de aprendizaje de maquina son secuenciales esto es se deben ejecutar una serie de funciones de manera continua, una tras de la otra lo que hace que el tiempo de ejecución sea elevado, sin embargo muchas de las funciones o métodos de los algoritmos de aprendizaje pueden ser ejecutados de forma paralela reduciendo el tiempo computacional haciendo que nuestros algoritmos sean mucho más eficientes. 
{: .text-justify}

Para esta razon se hace uso de las GPUs que son dispositivos especializados en procesar grandes cantidades de operaciones matemáticas de punto flotante, y  que ofrecen una alta capacidad de procesamiento masivo paralelo en cálculos que exigen un volumen grande de datos, permitiendo un rápido acceso  tanto a memoria como en las operaciones vectoriales y de interpolación.
{: .text-justify}


{% include figure image_path="/images/GPU/gp.PNG" alt="gpu tesla" caption="CPU vs GPU"%}


Sin embargo para poder hacer uso de las bondades y aprovechar el poder que ofrecen las GPUs es indispensable contar con *frameworks* que nos permitan programarlas. Para este ofjetivo Nvidia desarrollo la plataforma  *Compute Unified Driver Arquitecture* (CUDA)  que soporta lenguajes de programación como C, C++, Fortran Python y Matlab, y que permite a los progrmadores desarrollar aplicaciones escalables sin la necesidad de incorporar nuevos componentes de programación.
{: .text-justify}


Para entender cómo funcionan estos dispositivos tan poderosos es importante conocer su arquitectura

{% include figure image_path="/images/GPU/arqui.PNG" alt="gpu tesla" caption="Arquitectura GPU"%}



En este ejemplo contamos con dos *streaming multiprocessors* (MS) que son el corazón de las GPUs cada MS posee diferentes *streaming processors* (SP) o también llamados *cuda cores* (la cantidad de SPs depende del *compute capability* o capacidad de cálculo de la GPU, entre mayor sea el *compute capability* mejor será la arquitecturas de GPUs), los cuales pueden interactuar con el registrador, cada SM contiene diferentes tipos de memorias siendo la más común la *device memory* que puede ser accedida por todos los SP tanto  para lectura como para escritura de datos y que es común para todas las SMs, esto es realmente importante para poder administrar que cantidad de memoria queremos utilizar en nuestra aplicación, ya en la parte interior de cada SM se cuenta con una *shared memory* que puede ser accedida por todos los SPs también para lectura y escritura, finalmente existen dos tipos especiales de memoria interna a cada SM la *Constant Memory* y la *Texture Memory* teniendo como características principales que estas dos memorias solo tiene capacidad de lectura de datos y no de escritura 
{: .text-justify}


Pero como escoger la mejor GPU para nuestros modelos de *deep learning*? Esta pregunta puede ser respondida de la siguiente forma:

* Buscar la que realice un numero máximos de operaciones de punto flotante que pueda resolver (FLOPS)
* Buscar si son de precisión simple o doble. Esto hace la diferencia en modelos que requieran demasiada precisión como por ejemplo la detección de pacientes con cáncer.
* Total de memoria GPU
* Compute capability
* Arquitectura

Un consejo importante para montar una estación de trabajo es iniciar sabiendo que GPU se va a utilizar y hacer desde ese punto una regresión del resto de componentes, o sea para esa GPU que placa madre me sirve y que plataforma CUDA soporta cual procesador serai el mas adecuado y caunta memoira RAM puede ser adicionada. 
{: .text-justify}



La siguiente es una lista de links de interes para conocer un poco mas sobre GPUs:
1. [Multicore and GPU Programming: An Integrated Approach](https://www.amazon.com.br/Multicore-GPU-Programming-Integrated-Approach-ebook/dp/B00QWZ2690/ref=sr_1_1?ie=UTF8&qid=1496876593&sr=8-1&keywords=Multicore+and+GPU+Programming%3A+An+Integrated+Approach)
2. [Computer Architecture: A Quantitative Approach Fourth Edition](https://users.dimi.uniud.it/~antonio.dangelo/OpSys/materials/Computer_Architecture.pdf)
3. [Parallel Computing Center](http://parallelcompute.sourceforge.net/parcom.php)
3. [What is GPU Accelerated Computing](http://www.nvidia.com/object/what-is-gpu-computing.html)
3. [Compute Capability](https://developer.nvidia.com/cuda-gpus)
