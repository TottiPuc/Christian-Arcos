---
title: "Modelos de Lenguaje, una revolucion en el procesamiento del lenguaje natural"
date: 2024-04-09
tags: [LLM]
header:
  image: "/images/posts/llm.png"
excerpt: "Modelos de Lenguaje"
mathjax: "true"
---

Los modelos de lenguaje  han irrumpido en el campo del procesamiento del lenguaje natural (PLN), impulsando avances sin precedentes en diversas áreas. Debido a su capacidad para comprender y generar lenguaje humano de forma automática lo que los convierte en una herramienta invaluable para una amplia gama de aplicaciones, tale como:
{: .text-justify}

Asistencia virtual: Los modelos de lenguaje potencian a los asistentes virtuales, permitiéndoles responder preguntas de manera completa e informativa, seguir instrucciones complejas y ejecutar tareas diversas. Esto facilita la interacción natural entre humanos y máquinas, abriendo un abanico de posibilidades para la atención al cliente, la gestión de tareas y la automatización del hogar.
{: .text-justify}

Automatización de tareas de escritura: Los modelos de lenguaje automatizan tareas repetitivas de escritura, como la identificación y corrección de errores gramaticales en diferentes idiomas. Además, pueden extraer los puntos clave de un texto extenso y presentarlo de forma concisa, ahorrando tiempo y esfuerzo en la creación de resúmenes y análisis.
{: .text-justify}

Pero, que es un modelo de lenguaje y como funciona? Un modelo de lenguaje es un modelo matemático que determina la probabilidad a priori de que una palabra aparezca en una secuencia de texto, dadas la palabras anteriores, con el fin de comprender y generar lenguaje humano de forma automatica. Esta capacidad se basa en el análisis de grandes cantidades de datos textuales, lo que les permite aprender patrones y estructuras en el lenguaje.
{: .text-justify}

Existen tres tipos principales de modelos de lenguaje y pueden ser categorizados como: determinísticos, estadísticos o basados en redes neuronales.
{: .text-justify}

* Modelos determinísticos: estos son definidos por la gramática formal (reglas gramaticales predefinidas) y que restringen el idioma, limitando su flexibilidad y la capacidad de generalización y adaptación, como ejemplo tenemos los sistemas de transcripcion de dragon, que en sus primeras versiones se limitaba por la gramatica y reglas pre-configuradas
* Modelos estadísticos: se basan en estadísticas para predecir la siguiente palabra en una secuencia, utilizando el conexto y la informacion de frecuencia con que las palabras son pronunciadas (n-grams). Como ejemplo, tenemos al conocido sistema Watson de IBM que utilizó estas técnicas estadísticas en sus primeras iteraciones para el procesamiento del lenguaje natural, incluyendo el reconocmiento de voz y el análisis de texto.
* Modelos basados en redes neuronales: en este apartado se encuentran dos tipos de caegorias, los basados en redes neuronales tradicionales que buscan aprender patrones en el lenguaje y los modelos basados en aprendizaje profundo. Estos últimos, entrenados con grandes cantidades de texto, permitiendoles entender y generar lenguaje con un nivel de complejidad, coherencia y creatividad mucho mayor. Como ejemplo tenemos los GPT de OpenAI
{: .text-justify}

Sin embargo, asi como pueden ofrecer varios beneficios, también presentan algunos desafios, como los sesgos, debido a la cantidad limitada de datos con los que se entrenan, lo que puede llevar a resultados descriminatorios o de mala interpretación. Y uno de los mas grandes desafios el mal uso en aplicaciones que pueden crear contenido falso o engañoso generando desinformación.
{: .text-justify}

Para profundizar en los conceptos básicos de los modelos de lenguaje, se recomienda consultar los siguientes enlaces:

1. [Generando n-gramas con python](https://www.youtube.com/watch?v=pEYfD5aVrRI&ab_channel=DouglasStarnes)
2. [Transformes, entendiendo los modelos tras GPT](https://www.youtube.com/watch?v=SZorAJ4I-sA&ab_channel=GoogleCloudTech)
3. [Que es NLP](https://www.youtube.com/watch?v=fLvJ8VdHLA0&ab_channel=IBMTechnology)

