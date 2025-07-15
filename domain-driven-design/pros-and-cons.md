## Pros y Contras del DDD

### Aspectos Positivos

- **Lenguaje comun compartido** por todso los integrados del proyecto. Perfiles tecnicos y no tecnicos; evitando malentendidos.
- Al tener logica de aplicacion y dominio separadas, el **coste de realizar modificaciones suele ser menor**, ya que el dominio es mas estable.
- El codigo del dominio es autoexplicativo, es decir, el codigo refleja el dominio del problema y es facil de entender.
- **Mayor velocidad de desarrollo a medio y largo plazo**. Mucho mas mantenible.

### Aspectos Negativos

- El desarrollo es **mas lento al principio** de un proyecto, ya que es una arquitectura mas complejo y requiere mas tiempo de analisis y diseño.
- Require tener **expertos en el dominio del problema**
- Cambio de mentalidad de los desarrolladores para enfocarse en las funcionalidades mas que en los datos.
- Los frameworks actuales nos "empujan" a un modelo anemico y a pensar centrandonos en los datos.
### Cuando Usar DDD?

- Proyectos complejos con un **largo tiempo de vida esperado**
- Cuando hay una **incertidumbre en los casos de uso**. Prevision de cambios en el futuro.
- Problemas con una **logica de dominio presente**. Si lo unico que necesitas es un CRUD, no es necesario usar DDD.
- Disponibilidad de un equipo comprometido en analizar detalladamente el dominio del problema.