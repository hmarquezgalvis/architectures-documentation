## Resumen

### La importancia del Dominio

- El DDD se centra en la importacia de **entender bien el dominio** de nuestro problema para crear buen software.
  - En contraste con el enfoque tradicional de centrarse en la tecnologia o en los casos de uso.

Para identificar los elemnetos del dominio del problema, se deben seguir los siguientes pasos:
- Establecer el **Lenguaje Ubicuo**, que es donde se documenta y define todos los nombres, adjetivos y vertos que teienen que ver con el dominio del problema. Para ello, se deben realizar sesiones de **brainstorming** y **analisis del dominio**.
- Identificar los **Bounded Contexts**, dividir el dominio completo del sistema en bounded contexts, que son subdominios del dominio completo del sistema. Cada bounded context tiene su propio lenguaje ubicuo y sus propias entidades y reglas de negocio.
- Modelado del Dominio, que es un diagrama que refleja la comunicacion y las dependencias entre los distintos bounded contexts. En este diagrama se identifican las entidades, value objects y aggregates que componen el dominio del problema.

Todo esto se hace con el fin de **separar la logica de la aplicacion** (casos de uso) **de la logica del dominio**,
- Los casos de uso varian mucho mas frecuentemente que las reglas del dominio.

### Modelar el dominio

**Entidades**
- Elemnentos del dominio con entidad propia.
- Estas tienen comportamiento y datos.

**Value Objects**
- Elementos que solo almacenan datos.
- Creados para representar de forma mas clara los atributos de las entidades.

**Aggregates**
- Conjunto de entidades y value objects con un sentido comun en el dominio.

**Domain Services**
- Son elementos del dominio con logica que no tienen cabida en ninguna de las entidades.