# 🧩 Introducción a Git y Github

## 📌 ¿Qué es Git?

**Git** es un **sistema de control de versiones distribuido** creado por **Linus Torvalds** en 2005. Con el tiempo, se ha convertido en una herramienta **fundamental para la gestión de código fuente** en proyectos de programación colaborativa. Esto significa que **un clon local del proyecto es un repositorio de control de versiones completo**, lo que permite trabajar **sin conexión o de manera remota** con facilidad.  

Los desarrolladores pueden **confirmar su trabajo localmente** y, a continuación, **sincronizar su copia del repositorio con la copia en el servidor**. Este enfoque es distinto del control de versiones centralizado, donde los clientes deben sincronizar el código con un servidor antes de crear nuevas versiones.  

Git es un **software que maneja versiones** y lo hace de manera **local**, directamente en el dispositivo donde estés trabajando. Esto permite **guardar capturas de distintas versiones** del código que desarrolles, facilitando el seguimiento de cambios y la colaboración con otros desarrolladores.  

💡 *En resumen, Git te permite mantener un historial completo de tu proyecto, trabajar de manera organizada y segura, y colaborar eficientemente con otros desarrolladores.*  

## 📌 ¿Qué es GitHub?

**GitHub** es una **plataforma en línea** que utiliza el sistema de control de versiones **Git** para **alojar repositorios de código fuente** y facilitar la **colaboración en proyectos de desarrollo de software**. Fue fundada en **2008** por **Tom Preston-Werner, Chris Wanstrath, P. J. Hyett y Scott Chacon**, y desde entonces se ha convertido en una de las **herramientas más importantes y populares para desarrolladores en todo el mundo**.  

En GitHub, los desarrolladores pueden **subir sus repositorios locales a la nube**, compartirlos con otros, trabajar de manera conjunta en el mismo proyecto, **gestionar ramas, issues, pull requests**, y mantener un historial completo de cambios accesible desde cualquier lugar.  

💡 *En resumen, GitHub es la plataforma que lleva la potencia de Git a la nube, permitiendo a equipos de cualquier tamaño colaborar en tiempo real, mantener un flujo de trabajo más ordenado y centralizar sus proyectos de software en un solo lugar.*

---

## ✅ Beneficios del uso de un sistema de gestión de versiones

Existen diferentes beneficios cuando usamos un **sistema de gestión de versiones** como lo es **Git**, ya que cumple una función fundamental en el desarrollo de software. Esta herramienta nos ayuda a **gestionar y controlar los cambios** que realizamos en nuestro código, evitando errores y pérdidas de información.  

Podemos imaginar dos posibles escenarios: uno donde utilizamos un sistema de gestión de versiones y otro donde no lo usamos.  

- **❌ Sin un sistema de gestión de versiones:**  
  Imaginemos que estamos trabajando en un proyecto en el cual inicialmente creamos un archivo `index.html`. En un primer momento, le añadimos una estructura base con un **header**, una **barra lateral** y un **footer**, y guardamos esos cambios. Esto equivaldría a crear, por ejemplo, la **versión 0.1**.  

  Más adelante, decidimos integrar **botones, inputs y más elementos de formulario** al HTML, y al guardar tendríamos la **versión 0.2**. El problema es que estos cambios sustituyen por completo la versión anterior.  

  Ahora bien, si después de un tiempo, ya sea por una petición del cliente, por motivos del equipo de trabajo o por decisión personal o por algún error, se nos solicita **volver al estado inicial** (con solo el header, la barra lateral y el footer), tendríamos que **borrar manualmente** todo lo que añadimos, lo cual es un proceso **tardado, propenso a errores y nada eficiente**.  

- **✔️ Con un sistema de gestión de versiones:**  
  Ahora bien, si aplicamos el mismo ejemplo pero utilizando un **sistema de gestión de versiones**, tendríamos que al crear un archivo `index.html`, en un primer momento le añadimos una estructura base con un **header**, una **barra lateral** y un **footer**. Al guardar estos cambios, podríamos crear una especie de **versión 0.1** mediante un **commit**, el cual consiste en **confirmar una versión en Git** que quedará registrada como un **punto de guardado en nuestro historial**.  

  Más adelante, si decidimos integrar **botones, inputs y más elementos de formulario** al HTML, al guardar podríamos tener la **versión 0.2**. A diferencia de cuando no contamos con un sistema de gestión de versiones, aquí **no se sustituye la versión 0.1**, sino que **todas las versiones anteriores permanecen almacenadas** en el historial del repositorio.  

  De esta manera, si después de un tiempo, ya sea por una petición del cliente, motivos del equipo, decisión personal o incluso por un error se nos solicita **volver al estado inicial** (con solo el header, la barra lateral y el footer), mediante Git tendríamos la posibilidad de regresar fácilmente a esa versión anterior. A este proceso se le conoce como **rollback**.  

  Además, el sistema de gestión de versiones nos permite **comparar el código de diferentes versiones** (pasadas o actuales), pudiendo identificar con precisión qué líneas de código fueron **agregadas, eliminadas o modificadas** en cada commit, lo cual facilita enormemente la depuración y el trabajo colaborativo.  

---

## 👥 Trabajo en equipo

Los sistemas de gestión de versiones nos permiten **trabajar de manera más eficiente en equipo**. Aunque se podría trabajar directamente, por ejemplo, en **Google Drive**, donde el código se actualiza en tiempo real, este enfoque tiene varias desventajas: siempre se necesita **conexión a Internet**, y si un archivo se elimina por error, **se pierde para siempre**, y ninguno de los integrantes tendría una copia.  

Con **Git**, en cambio, podemos trabajar y crear nuestros **commits** de manera **local** en nuestro dispositivo, y posteriormente **subir esos cambios al servidor** cuando queramos. Esto permite **controlar exactamente qué cambios se comparten**, evitando pérdidas accidentales de información.  

Además, Git cuenta con **repositorios remotos**, que son **lugares en la nube donde se almacena el código y todas sus versiones**, siendo **GitHub** la plataforma más utilizada. Todos los integrantes del equipo pueden trabajar localmente, subir sus cambios cuando estén listos y **consultar todas las versiones existentes**.  

💡 *Trabajar de manera local con Git permite que nunca se elimine accidentalmente el trabajo en el repositorio y que solo se suban los cambios que realmente están correctos y aprobados.*

---

## 🚨 ¿Cuándo comenzó a fallar y por qué?

Uno de los grandes beneficios de un **sistema de gestión de versiones** como **Git** es que nos permite **detectar con precisión cuándo comenzó un error en nuestra aplicación**.  

Cuando varios integrantes de un equipo van subiendo cambios a un mismo proyecto, es posible que en algún momento una funcionalidad deje de funcionar correctamente. Gracias al **historial de commits**, Git nos permite **revisar paso a paso las versiones anteriores del código**, identificar en qué momento se introdujo el fallo y, si es necesario, **volver a una versión estable** mediante un **rollback**.  

Sin un sistema de control de versiones, esto no sería posible, ya que no contaríamos con un historial que indique **qué cambios se hicieron, cuándo y por quién**. En Git, cada commit funciona como una **copia de seguridad del estado del código en ese momento**, lo que nos brinda la capacidad de **avanzar o retroceder en el tiempo** según sea necesario.  

💡 *Git nos da la capacidad de rastrear errores, corregirlos de manera eficiente y mantener la estabilidad de la aplicación sin perder el historial de nuestro trabajo.*

---

# ⚙️ Git Config

## 🖳 Terminal de Git

Si bien **Git** es un **sistema de gestión de versiones**, es importante mencionar que se trata de un **programa que debe instalarse** en nuestro equipo. Al hacerlo, no solo obtenemos la herramienta principal, sino también una **terminal propia** llamada **Git Bash**, en la cual podremos ejecutar **comandos específicos** para trabajar con nuestros proyectos.  

Para abrirla, simplemente podemos buscar **"Git Bash"** en la barra de búsqueda de Windows. Otra opción muy práctica es **hacer clic derecho en cualquier carpeta** y seleccionar **"Git Bash Here"**, lo cual abrirá la terminal directamente en esa ubicación. Esto es especialmente útil porque **cualquier acción que realicemos desde Git afectará al contenido de la carpeta actual**, como inicializar un repositorio, confirmar cambios, crear ramas o subir código a un repositorio remoto.  

Desde esta consola podemos realizar diversas acciones como **crear commits**, **subir cambios a GitHub**, **configurar nuestro usuario**, **crear ramas**, entre muchas otras operaciones que nos permiten tener un **control detallado del flujo de trabajo**.  

Por otro lado, algunos entornos de desarrollo como **Visual Studio Code** incluyen herramientas gráficas que facilitan la gestión de Git. Esto significa que podemos **confirmar cambios, crear ramas o sincronizar nuestro repositorio** sin necesidad de escribir comandos en la terminal, lo cual resulta muy práctico para quienes prefieren una interfaz más visual.  

💡 *La terminal de Git es la herramienta más completa para interactuar con el sistema, y abrirla en la carpeta correcta nos permite ejecutar acciones directamente sobre su contenido, mientras que los entornos gráficos ofrecen una alternativa más sencilla y accesible.*

