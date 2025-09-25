# 🐙 Git & GitHub Course

## 🔹 Git

### ¿Que es Git?

**Git** es un **sistema de control de versiones distribuido** creado por **Linus Torvalds** en 2005. Con el tiempo, se ha convertido en una herramienta **fundamental para la gestión de código fuente** en proyectos de programación colaborativa. Esto significa que **un clon local del proyecto es un repositorio de control de versiones completo**, lo que permite trabajar **sin conexión o de manera remota** con facilidad.  

Los desarrolladores pueden **confirmar su trabajo localmente** y, a continuación, **sincronizar su copia del repositorio con la copia en el servidor**. Este enfoque es distinto del control de versiones centralizado, donde los clientes deben sincronizar el código con un servidor antes de crear nuevas versiones.  

Git es un **software que maneja versiones** y lo hace de manera **local**, directamente en el dispositivo donde estés trabajando. Esto permite **guardar capturas de distintas versiones** del código que desarrolles, facilitando el seguimiento de cambios y la colaboración con otros desarrolladores.  

💡 *En resumen, Git te permite mantener un historial completo de tu proyecto, trabajar de manera organizada y segura, y colaborar eficientemente con otros desarrolladores.*

---

### Beneficios del uso de un sistema de gestión de versiones

Existen diferentes beneficios cuando usamos un **sistema de gestión de versiones** como lo es **Git**, ya que cumple una función fundamental en el desarrollo de software. Esta herramienta nos ayuda a **gestionar y controlar los cambios** que realizamos en nuestro código, evitando errores y pérdidas de información.  

Podemos imaginar dos posibles escenarios: uno donde utilizamos un sistema de gestión de versiones y otro donde no lo usamos.  

- **Sin un sistema de gestión de versiones:**  
  Imaginemos que estamos trabajando en un proyecto en el cual inicialmente creamos un archivo `index.html`. En un primer momento, le añadimos una estructura base con un **header**, una **barra lateral** y un **footer**, y guardamos esos cambios. Esto equivaldría a crear, por ejemplo, la **versión 0.1**.  

  Más adelante, decidimos integrar **botones, inputs y más elementos de formulario** al HTML, y al guardar tendríamos la **versión 0.2**. El problema es que estos cambios sustituyen por completo la versión anterior.  

  Ahora bien, si después de un tiempo, ya sea por una petición del cliente, por motivos del equipo de trabajo o por decisión personal, se nos solicita **volver al estado inicial** (con solo el header, la barra lateral y el footer), tendríamos que **borrar manualmente** todo lo que añadimos, lo cual es un proceso **tardado, propenso a errores y nada eficiente**.  

- **Con un sistema de gestión de versiones:**  
  Ahora, imaginemos el mismo caso, pero esta vez utilizando **Git**. Cada vez que realizamos un cambio importante en el archivo `index.html`, podemos **guardar una versión (commit)** que registra el estado exacto del proyecto en ese momento.  

  Supongamos que partimos de la **versión 0.1** (con header, barra lateral y footer). Luego añadimos botones, inputs y otros elementos, y guardamos esos cambios como la **versión 0.2**. La diferencia aquí es que **la versión 0.1 no se pierde**, ya que Git mantiene un historial completo de todo lo que hemos hecho.  

  Si en algún momento alguien del equipo o el cliente solicita regresar al diseño inicial, simplemente podemos **volver a la versión 0.1 con un solo comando**, sin necesidad de eliminar manualmente los cambios realizados.  

  Otra gran ventaja es que con Git también podemos **comparar versiones de código** (por ejemplo, ver las diferencias entre la versión 0.1 y la 0.2). De esta manera, podemos identificar con precisión qué líneas se añadieron, modificaron o eliminaron en cada cambio.  

  Además, Git nos permite trabajar de manera **colaborativa**: varios desarrolladores pueden aportar cambios en distintas partes del proyecto, y gracias al sistema de versiones es posible integrar (o revertir) esas modificaciones de forma organizada y controlada.  
