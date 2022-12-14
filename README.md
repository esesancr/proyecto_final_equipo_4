### Proyecto Final
## Optimización de Portafolio.

### Equipo 4

## Distribución de roles por usuario

| github user  | Integrante                |Tarea | Rol             |
|--------------|---------------------------|------|-----------------|
| leonfgz48    |Leon Felipe Gomez Zarza    |  1   | Programación    |
| afuentesc    |Alberto Fuentes Chavarria  |  1   | Programación    |
| RGGA90       |Ricardo Guillermo Granillo Alatorre |  2   | Revisión        |
| esesancr     |Sergio Sánchez Reyes       |  3   | Project Manager |

# Introducción: 

Existen muchas formas de crecer el patromonio de un inversionista. Una de las formas más comunes que existen es el de invertir en el mercado financiero y más especificamente en el de Equity. Esto significará que el dicho inversionista tendrá que seleccionar acciones que cotizen dentro de las Bolsas de valores. La pregunta natural que nace apartir de lo anterior es ¿Qué empresas deberá seleccionar el inversionista para que su dinero este relamente bien invertido?. En este punto deberemos saber que existe una compensación entre el riesgo y el rendimiento, es decir, para aumentar el rendimiento esperado de la inversión, entonces el inversor debe estar dispuesto a tolerar mayores riesgos.

# Teoría Moderna de Portafolio: 

Una vez planteado lo anteriror se puede discutir el concepto de seleccionar el "mejor" portafolio. Esta definición de el "mejor portafolio" fue estudiado con mucho éxito por el premio Nobel Harry Markowitz. Su modelo proporciona una manera de definir carteras que sean eficientes. Una cartera o portafolio eficiente es aquel que tiene el rendimiento más alto con un nivel de riesgo más bajo para una recompensa dada. 

Para ver cómo funciona esto imagina que hay cuatro activos en el mundo, A, B, C y D con cierto rednimiento y riesgo cada uno. Si pudieramos comprar cualquiera de estos ¿cuál comprarías? ¿Elegirías A, B, C o D?. Que pasaría si D tiene el mismo riesgo que B pero menos rendimiento. Por otro lado, si tiene el mismo rendimiento que C pero con mayor riesgo. Podemos descartar D. A lo anterior adicionemos que depende de las preferencias de riesgo de en inversionista, conviertiendo esto es una elección subjetiva.   

La teoría del portafolio estudia el cómo modelar la compensación dada una colección de n portafolios posibles con rendimientos $r_{i}$ para $i= 1, 2, . . . , n$. Los rendimientos $r_{i}$ generalmente no se conocen de antemano y, a menudo, se supone que son variables aleatorias que siguen una distribución normal.

# Problema de Optimización:

Método: Sequential least squares.

EL método sequential least squares es un método iterativo para problemas no lineales de optimización restringidas. 
El problema parte de que la función puede ser aproximada como: $f(x)\approx f(x)+\nabla f(x^k)(x-x^k)+\frac{1}{2} (x-x^k)Hf(x^k)(x-x^k)$, con H como la Hessiana.

Sujeto a las funciones g y h por sus aproximaciones afines locales: 

$g(x)\approx g(x^k)+\nabla g(x^k)(x-x^k)$

$h(x)\approx h(x^k)+\nabla h(x^k)(x-x^k)$

Si el problema solo tiene restricciones de igualdad, entonces el método es equivalente a aplicar el método de Newton a las condiciones de optimalidad de primer orden, o condiciones de Karush-Kuhn-Tucker, del problema.

