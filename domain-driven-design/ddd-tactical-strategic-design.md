## DDD: Tactical Design

**Model-Driven Design**: Hace referencia a que modelemos desde nuestro contexto, es decir, dirigir nuestro diseño en base a los modelos. Esto lo conseguiremos a través de:
- Expresar la Semantica de Dominio en términos de:
  - **Services**
  - **Entities**
  - **Value Objects**
  - **Aggregates**: Elementos conceptuales que nos permitirán mantener la integridad de las entidades y encapsular los value objects.
  - **Repositories**: En los que persistiremos nuestras entidades.
- Cada vez que se produzcan cambios en nuestras entidades lanzaremos **Domain Events**, reflejando que algo ha pasado en nuestro sistema.
- Gracias a los **Factories** podremos encapsular nuestras entidades, agregados y value objects. En los repositorios que utilizamos en los cursos podeis ver ejemplos de cómo implementamos el Factory Pattern.
- Generalmente cuando trabajemos con DDD lo haremos a través de una **Arquitectura por Capas** como es el caso de la Arquitectura Hexagonal.
- Propone el uso de **Ubiquitous Language**, es decir, que los nombres de variables, metodos y clases se establezcan con el lenguaje de nuestro dominio.
- Todo ello se define dentro de un **Bounded Context**, que nos va a permitir una mayor autonomía entre equipos además de establecer límites en el lenguaje.

## DDD: Strategic Design

Dentro de nuestro **Bounded Context**, mantenemos nuestro modelo unificado gracias a la **Integración Continua**. Hablamos de **Context Map** para referirnos al mapeo realizado de los términos que utilizamos en real a conceptos lógicos o físicos. Este mapeo nos ayudará además a:
- Separar el **Big Ball of Mud** de nuestra aplicación, y llevar a cabo la publicación de eventos en lugar de adentrarnos en un código costoso de desacoplar.
- Identificar cómo aplicar el **Anticorruption Layer**.
- Cada equipo puede trabajar de forma separada (Podremos, por ejemplo, utilizar distintos lenguajes de programación para los diferentes contextos de nuestra aplicación).
- Facilita la publicación de **Open Host Services** para la comunicación entre los Bounded Contexts y entre la estructura organizacional de nuestra aplicación (**Published Language**).
- Posibilita la relación entre contextos a través de un **Shared Kernel** y en términos de **Customer/Supplier Team** y de **Conformist**.