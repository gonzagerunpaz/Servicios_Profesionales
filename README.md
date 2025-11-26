# Servicios profesionales

En este ejercicio, se nos pide modelar empresas que ofrecen los servicios de profesionales


## Etapa 1 - profesionales y empresas

De cada **profesional** se debe poder obtener:
- en qué _universidad_ estudiaron, esto se debe asignar para cada profesional.
- sus _honorarios por hora_ de trabajo, cómo se determina depende del tipo de profesional.
- en qué _provincias_ puede trabajar, cómo se determina depende del tipo de profesional.

De cada **universidad** nos va a interesar: en qué provincia está, y qué honorarios por hora de trabajo recomienda para los profesionales.

Deben contemplarse distintos tipos de profesionales, de acuerdo a lo que se indica a continuación.
- **Profesionales vinculados a una universidad**:  
  pueden trabajar solamente en la provincia donde está la universidad, los honorarios son los que recomienda la universidad.
- **Profesionales asociados del Litoral**:
  pueden trabajar en Entre Ríos, Santa Fe y Corrientes, cobran 3000 pesos por hora de trabajo.
- **Profesionales libres**:
  se indica para cada uno en qué provincias pueden trabajar y los honorarios por hora, además de la universidad.
  
  
Cada **empresa de servicios** contrata a varios profesionales. Para cada una se indica un honorario de referencia.

A partir de este modelo, tiene que poder obtenerse para una empresa:
- cuántos (un número) de sus profesionales contratados estudió en una determinada universidad.   
- el profesional _más barato_ (o sea, que sus honorarios son los más bajos).



### Comentario que puede ayudar para la resolución  
Cada universidad debe acordarse provincia y honorarios recomendados, se le setean y listo.  
Por otro lado, _está mal_ que los profesionales vinculados se acuerden de qué provincias tienen habilitadas y cuáles son sus honorarios; le tienen que pedir estos datos a la Universidad.
  
De paso: **OJO** que la Universidad está en _una_ provincia, pero el profesional tiene que devolver una _colección_ de provincias. Un profesional vinculado devolverá una colección con un solo elemento.

<br>


## Test de la etapa 1

Tenemos estas universidades:
- de San Martín: está en la provincia de Buenos Aires, los honorarios recomendados son de 3500 pesos.
- de Rosario: está en la provincia de Santa Fe, los honorarios recomendados son de 2800 pesos.
- de Corrientes: está en la provincia de Corrientes, los honorarios recomendados son de 4200 pesos.
- de Jose C Paz: está en la provincia de Buenos Aires, los honorarios recomendados son de 8800 pesos.

y estos profesionales
- Juana, vinculada, estudió en la Univ. de Rosario.
- Melina, asociada el Litoral, estudió en la Univ. de Corrientes.
- Rocío, libre, estudió en la Univ. de Jose C Paz, honorarios 5000 pesos, puede trabajar en Santa Fe, Córdoba y Buenos Aires.
- Luciana, libre, estudió en la Univ. de Rosario, honorarios 3200 pesos, puede trabajar en Santa Fe y Entre Ríos.

Una empresa que contrate a estos cuatro profesionales, y cuyos honorarios de referencia son 3500 pesos, debe tener
- dos de sus profesionales estudiaron en Rosario, uno en Jose C Paz, ninguno (o sea cero) en San Martín.
- como _profesional más barato_ a Juana.


Hacer los tests que sean necesarios para verificar esto.  


