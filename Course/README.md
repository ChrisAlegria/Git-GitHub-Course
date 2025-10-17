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

## 🖳 Terminal de Git
Si bien **Git** es un **sistema de gestión de versiones**, es importante mencionar que se trata de un **programa que debe instalarse** en nuestro equipo. Al hacerlo, no solo obtenemos la herramienta principal, sino también una **terminal propia** llamada **Git Bash**, en la cual podremos ejecutar **comandos específicos** para trabajar con nuestros proyectos.  

Para abrirla, simplemente podemos buscar **"Git Bash"** en la barra de búsqueda de Windows. Otra opción muy práctica es **hacer clic derecho en cualquier carpeta** y seleccionar **"Git Bash Here"**, lo cual abrirá la terminal directamente en esa ubicación. Esto es especialmente útil porque **cualquier acción que realicemos desde Git afectará al contenido de la carpeta actual**, como inicializar un repositorio, confirmar cambios, crear ramas o subir código a un repositorio remoto.  

Desde esta consola podemos realizar diversas acciones como **crear commits**, **subir cambios a GitHub**, **configurar nuestro usuario**, **crear ramas**, entre muchas otras operaciones que nos permiten tener un **control detallado del flujo de trabajo**.  

Por otro lado, algunos entornos de desarrollo como **Visual Studio Code** incluyen herramientas gráficas que facilitan la gestión de Git. Esto significa que podemos **confirmar cambios, crear ramas o sincronizar nuestro repositorio** sin necesidad de escribir comandos en la terminal, lo cual resulta muy práctico para quienes prefieren una interfaz más visual.  

💡 *La terminal de Git es la herramienta más completa para interactuar con el sistema, y abrirla en la carpeta correcta nos permite ejecutar acciones directamente sobre su contenido, mientras que los entornos gráficos ofrecen una alternativa más sencilla y accesible.*

---

# ⚙️ Git Config
El comando **`git config`** se utiliza dentro de la **terminal de Git** y nos permite **realizar configuraciones importantes** para que la terminal sepa cómo manejar nuestro entorno. Gracias a este comando, podemos **personalizar Git según nuestras necesidades**, especificando información como **nombre de usuario, correo electrónico**, editor de texto predeterminado, colores en la terminal y otros parámetros que Git utilizará en nuestros commits y repositorios.  

Estas configuraciones son esenciales porque Git utiliza esta información para **identificar al autor de los commits** y mantener un historial organizado y claro, especialmente cuando trabajamos en **proyectos colaborativos**.  

## 🌐 --global
El parámetro **`--global`** se usa junto con el comando `git config`, quedando de la forma:  

```bash
git config --global
```

Al usar **`--global`**, le estamos indicando a Git que las configuraciones que definamos afectarán a todos los proyectos en nuestro equipo que utilicen Git, y no solo al repositorio en el que estemos trabajando actualmente. Esto es especialmente útil para establecer información general, como nuestro nombre o correo electrónico, que se aplicará automáticamente en todos los commits que realicemos.

## 🧑🏻‍💻 User
El parámetro **`user`** en Git nos permite declarar **dos opciones diferentes**: nuestro **nombre** y nuestro **correo electrónico**. Ambas son de **suma importancia** cuando se trabaja de manera colaborativa, ya que todos nuestros **commits** se registrarán con esta información. De esta forma, cualquier persona que consulte el historial de cambios en plataformas como **GitHub** podrá identificar **quién realizó cada acción** y con qué correo asociado.  

- **`user.name`:**  
  Para especificar nuestro **nombre** en Git utilizamos el comando `user.name`. Aquí, `user` hace referencia a la configuración de nuestro usuario, y `.name` indica que vamos a declarar nuestro nombre. El comando se ejecuta junto con comillas, dentro de las cuales colocaremos nuestro nombre, por ejemplo:  

  ```bash
  git config user.name "ChristianAR"
  ```

- **`user.email`:**
  Para especificar nuestro correo electrónico en Git utilizamos el comando `user.email`. Al igual que antes, `user` indica la configuración del usuario y `.email` señala que vamos a declarar nuestro correo. Es importante que este correo coincida con el que usaremos en nuestro repositorio remoto (GitHub, GitLab, Gitea, etc.), de lo contrario, podrían generarse errores al sincronizar los commits. El comando se ejecuta con comillas, dentro de las cuales colocaremos nuestro correo, por ejemplo:

  ```bash
    git config user.email "christian.alegriar@gmail.com"
  ```

## 🖥 Core
El parámetro **`core`** en Git hace referencia al **núcleo del sistema**, es decir, a aquellas configuraciones que afectan directamente el **funcionamiento fundamental de Git**. A través de este parámetro podemos establecer ajustes esenciales que determinan cómo se comporta Git en nuestro entorno de trabajo.  

Por lo que el parámetro `core` controla aspectos esenciales del funcionamiento de Git, como el editor por defecto, el manejo de archivos y el comportamiento interno del sistema, permitiéndonos personalizar la experiencia de trabajo según nuestras necesidades.

- **`core.editor`:**  
  El parámetro **`core.editor`** en Git nos permite **configurar el editor de texto o código predeterminado** que Git abrirá cuando sea necesario realizar acciones que requieran edición manual, como escribir un mensaje de commit más largo, resolver conflictos de merge o editar configuraciones avanzadas.  

  Por defecto, Git puede abrir editores básicos como **Vim** o **Nano** en la terminal, lo cual puede resultar incómodo si no estamos familiarizados con ellos. Para mayor comodidad, podemos indicar que queremos usar un editor más moderno, como **Visual Studio Code**, **Sublime Text** o cualquier otro editor instalado en nuestro sistema.  

  En el caso de **Visual Studio Code**, su comando de apertura es `code`. Para configurarlo como nuestro editor predeterminado en Git, ejecutaríamos el siguiente comando:

  ```bash
  git config core.editor "code"
  ```

  ⚠️ *OJO: Configurar un editor externo en Git no significa que vayamos a ejecutar los comandos desde ese editor (como git commit o git push). Lo que hace es que, cuando Git necesite que escribamos algo que la consola no maneja cómodamente (por ejemplo, un mensaje de commit largo, una descripción detallada en un merge o la edición de configuraciones internas), en lugar de usar la terminal, se abrirá automáticamente el editor que hayamos configurado.*


  - **`--wait`:**  
    El parámetro **`--wait`** se utiliza junto con `core.editor`, por ejemplo: `core.editor "code --wait"`. Su función es **indicarle a Git que debe esperar a que el editor externo termine de realizar la acción antes de continuar con el comando**.  
  
    Como mencionamos antes, Git abre editores externos para ciertos casos especiales, como escribir mensajes de commit largos o resolver conflictos. Sin embargo, en ocasiones Git puede **interpretar incorrectamente que ya hemos terminado**, ejecutando el comando **antes de que realmente hayamos ingresado la información necesaria** en el editor. Esto puede generar errores o commits vacíos.  
  
    El uso de `--wait` **soluciona este problema**, obligando a Git a **esperar hasta que guardemos y cerremos el editor externo** antes de ejecutar el comando correspondiente. De esta manera, se asegura que todo lo que necesitamos ingresar en el editor sea procesado correctamente por Git. Por lo que el comando completo para configurar Visual Studio Code como editor predeterminado y usar `--wait` sería:  
  
    ```bash
    git config core.editor "code --wait"
    ```

- **`core.autocrlf`:**  
  La mayoría de los servidores de repositorios remotos como **GitHub**, **GitLab** y otros funcionan en entornos **Linux/Unix**, lo que provoca que los **saltos de línea** se manejen de forma diferente en comparación con **Windows**.  

  Aquí es donde entra en juego el parámetro **`core.autocrlf`**, el cual nos permite **indicar a Git cómo manejar automáticamente los saltos de línea según el sistema operativo que estemos usando**.  

  Aunque Git suele detectar nuestro sistema operativo de forma automática, es recomendable **configurarlo manualmente** para evitar errores en los archivos al momento de compartir código con otros desarrolladores que trabajen en sistemas diferentes. Si no lo configuramos correctamente, pueden generarse **conflictos de formato** en los archivos, lo que complica el trabajo colaborativo. Por lo que la estructura básica es la siguiente:  

  ```bash
  git config core.autocrlf <valorSegunSistemaOperativo>
  ```

  Donde **`<valorSegunSistemaOperativo>`** puede variar según nuestro entorno:

  - **En Windows:** normalmente se utiliza `true`, quedando como:
    ```bash
  	git config core.autocrlf true
  	```
    
  - **En Linux/Unix o macOS:** generalmente se utiliza `input`,quedando como:
    ```bash
  	git config core.autocrlf input
  	``` 

  💡 *core.autocrlf nos ayuda a que los saltos de línea se mantengan consistentes entre diferentes sistemas operativos, evitando errores y asegurando que el código sea legible y funcional sin importar desde dónde se edite.*

## ✏️ Edit
El parámetro **`--edit`**, abreviado como **`-e`**, nos permite **editar archivos de configuración** en Git. Dentro de `git config`, este parámetro nos facilita **verificar nuestras configuraciones actuales**, ya sea a nivel de proyecto o de manera global, y **modificarlas si así lo deseamos**.  

Cuando usamos **`git config -e`** o **`git config --edit`**, Git abre nuestro **editor de código externo** mostrando un archivo con toda nuestra configuración según corresponda (por proyecto o global). Este archivo incluye información como el **nombre de usuario**, **correo electrónico**, **origen del repositorio remoto**, **editor predeterminado**, entre otras configuraciones importantes. Ademas cabe mencionar que tanto la forma completa como la abreviada pueden ser ejecutadas y teniendo ambas la misma funcion, siendo las siguientes:

```bash
git config -e
git config --edit
```

Al ejecutar cualquiera de estos comandos nuestro editor de código abrirá un archivo similar al siguiente, donde podremos comprobar y modificar nuestras configuraciones:
```bash
[core]
	repositoryformatversion = 0
	filemode = false
	bare = false
	logallrefupdates = true
	symlinks = false
	ignorecase = true
	editor = code --wait
[remote "origin"]
	url = https://github.com/ChrisAlegria/Git-GitHub-Course.git
	fetch = +refs/heads/*:refs/remotes/origin/*
[branch "main"]
	remote = origin
	merge = refs/heads/main
```

## 📑 Archivo de configuración  
Cuando creamos un proyecto para trabajar con un sistema de gestión de versiones como **Git**, se genera un archivo llamado **`.gitconfig`**, el cual contiene toda la configuración que el proyecto está utilizando. Este archivo puede reflejar tanto configuraciones específicas del proyecto como configuraciones globales aplicadas a todo el sistema, y estará siempre presente en los repositorios que gestionemos con Git. En él se almacenan parámetros importantes como el **editor de texto predeterminado**, el **nombre de usuario**, el **correo electrónico** asociado y muchos otros ajustes que determinan el comportamiento de Git.  

💡 *En resumen, el archivo `.gitconfig` es el lugar donde Git centraliza todas las configuraciones necesarias para que podamos trabajar de manera ordenada y personalizada en cada proyecto.*

# 📟 Comandos Básicos de la Terminal  
Existen diversos **comandos básicos** dentro de la **consola/terminal de Git**, los cuales están basados en los **comandos de Linux**. Estos comandos se pueden utilizar en diferentes momentos y resultan muy útiles para tareas como **ayuda, edición, modificación y gestión general** dentro del entorno de trabajo. La gran ventaja es que la mayoría de ellos son **universales**, es decir, pueden usarse en cualquier proyecto y en prácticamente cualquier situación, ya sea para **aplicar configuraciones globales, solicitar ayuda, realizar ediciones o limpiar la consola**. Son, en definitiva, **comandos clave** que todo desarrollador debe dominar para desenvolverse de manera más eficiente al trabajar con Git.  Por lo que algunos de los más comunes son: 

- **`--edit` / `-e`:**  
  El parámetro `--edit`, que también podemos usar en su forma corta como `-e`, nos permite **editar cualquier archivo de configuración**. Un ejemplo de esto es `core`, un archivo donde se guardan las configuraciones de nuestros proyectos. Si ejecutamos `git config core -e`, se abrirá dicho archivo para **realizar modificaciones manualmente** de manera directa. Por lo que un ejemplo de este seria:

  ```bash
  git config -e
  ```

- **`--help` / `-h`:**  
  El parámetro `--help`, que también puede usarse como `-h`, nos permite **solicitar ayuda a Git**. Al ingresar este comando, se mostrará una **lista de los posibles comandos disponibles** que podemos utilizar. Por ejemplo, `git config -h` nos mostrará todos los comandos disponibles para `git config`, y esto aplica de manera similar para cualquier otro comando o apartado. Por lo que un ejemplo de este seria:

  ```bash
  git config -h
  ```

- **`--list`:**  
  Comúnmente, para verificar información en algún archivo solemos usar `-e` para abrirlo y revisar manualmente su contenido. Con el comando o parámetro `--list`, podemos **extraer directamente la información del archivo** y mostrarla en la consola, sin necesidad de abrirlo manualmente. Esto facilita la **consulta rápida de configuraciones** y datos relevantes. Por lo que un ejemplo de este seria:

  ```bash
  git config --list
  ```

- **`clear`:**   
  El comando `clear` nos permite **limpiar la consola**, eliminando todos los comandos previos y cualquier salida que se haya mostrado en pantalla. Esto no **afecta en absoluto los archivos, configuraciones ni el estado de nuestro proyecto**, simplemente nos ofrece una **pantalla limpia** para continuar trabajando de manera ordenada.

- **`ls`:**  
El comando `ls` nos permite **visualizar el listado de archivos y carpetas** que se encuentran en el directorio donde hayamos abierto la terminal. Por ejemplo, si abrimos la terminal en una carpeta llamada `proyecto` y ejecutamos `ls`, se desplegarán todas las carpetas y archivos que estén dentro de ella. De esta manera, el comando muestra de forma clara el contenido del directorio actual, lo que nos ayuda a ubicar los recursos disponibles sin necesidad de salir de la terminal. Un ejemplo de su uso sería:  

  ```bash
  chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/Git-GitHub-Course (main)
  $ ls
  Course/  Practices/  README.md
  ```

  - **`-a`:**  
  La opción `-a` (**all**) se utiliza junto con el comando `ls` para **mostrar todos los archivos y directorios**, incluyendo aquellos que están **ocultos**. En los sistemas basados en Linux (como Git Bash), los archivos ocultos son aquellos cuyo nombre comienza con un punto (`.`), por ejemplo: `.git`, `.env`, `.config`. De manera predeterminada, el comando `ls` no los muestra, pero al usar `ls -a` sí aparecerán en la lista. Esto resulta muy útil cuando queremos **ver archivos de configuración internos** que normalmente no son visibles, ya que muchos proyectos contienen carpetas y archivos ocultos que son esenciales para su funcionamiento. Por lo que un ejemplo practico seria:                    

  	```bash
  	chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/Git-GitHub-Course (main)
  	$ ls -a
  	./  ../  .git/  index.html  README.md
  	$
  	```

- **`cd`:**  
El comando `cd` (change directory) se utiliza para **movernos entre carpetas** desde la terminal. Por defecto, todos los comandos que ejecutamos en la terminal afectan a la **carpeta en la que nos encontramos actualmente** y, según el caso, a todas las subcarpetas que esta contenga. Por ejemplo, si estamos ubicados en una carpeta llamada `proyecto`, que a su vez contiene dos subcarpetas llamadas `proyecto_1` y `proyecto_2`, cualquier acción que ejecutemos tendrá efecto en `proyecto`.  Ahora bien, si lo que queremos es **acceder a una subcarpeta específica** para trabajar directamente en ella, usamos el comando `cd`. Basta con escribir `cd` seguido del nombre de la carpeta a la que deseamos entrar. Una vez ejecutado, la terminal cambiará su ubicación a esa carpeta, quedando de la siguiente manera:  

  ```bash
  chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/Git-GitHub-Course (main)
  $ cd course

  chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/Git-GitHub-Course/course (main)
  $
  ```

- **`cd ..`:**  
El comando `cd ..` se utiliza para **retroceder un nivel en el árbol de directorios**, es decir, salir de la carpeta en la que nos encontramos actualmente y volver a la carpeta que la contiene. En otras palabras, funciona como la operación **inversa a `cd`**, ya que en lugar de entrar en una subcarpeta, nos permite **regresar a la carpeta padre**. Por ejemplo, si estamos dentro de la carpeta `proyecto_1`, que a su vez está dentro de `proyectos`, al ejecutar `cd ..` volveremos directamente a `proyectos`. La terminal quedaría de la siguiente manera:  

  ```bash
  chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/Git-GitHub-Course/course (main)
  $ cd ..

  chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/Git-GitHub-Course (main)
  $
  ```
  
- **`pwd`:**  
El comando `pwd` (**print working directory**) se utiliza para **mostrar la ruta completa del directorio en el que nos encontramos actualmente** dentro de la terminal. Al ejecutarlo, Git Bash (o cualquier terminal basada en Linux) nos devuelve la **dirección absoluta** de la carpeta en la que estamos trabajando. Es importante no confundirlo con `ls`. Mientras que `pwd` nos indica **en qué carpeta estamos ubicados**, el comando `ls` lista los **archivos y subcarpetas que contiene el directorio actual**. Por ejemplo, si queremos confirmar nuestra ubicación dentro de la estructura de carpetas, podríamos obtener algo como lo siguiente:  

  ```bash
  chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/Git-GitHub-Course (main)
  $ pwd
  /d/Trabajos/Cursos/Git-GitHub-Course
  $
  ```

- **`mkdir`:**  
El comando `mkdir` (**make directory**) se utiliza para **crear nuevas carpetas (directorios)** directamente desde la terminal de Git.  Aunque comúnmente hablamos de "carpetas", en los sistemas basados en Linux (como Git Bash) estas se conocen como **directorios**. Para crear uno, basta con escribir `mkdir` seguido del nombre que le queremos asignar. Por ejemplo, si queremos crear una carpeta llamada `proyecto_3`, podemos hacerlo de la siguiente manera:  

  ```bash
  chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/Git-GitHub-Course (main)
  $ mkdir proyecto_3
  $
  ```

- **`git init`:**  
El comando `git init` se utiliza para **indicarle a Git que la carpeta en la que estamos trabajando será gestionada con su sistema de control de versiones**. Al ejecutar este comando, la carpeta actual se **convierte en un repositorio local de Git**, es decir, un espacio de trabajo donde podremos comenzar a llevar un **historial de cambios (commits)**, gestionar versiones y trabajar con ramas, aunque aún no esté vinculado a un repositorio remoto. En otras palabras, `git init` **inicializa un nuevo repositorio vacío** dentro de la carpeta en la que estamos, creando un directorio oculto llamado **`.git/`**, donde se almacenará toda la información y la configuración necesaria para el seguimiento de versiones. Un ejemplo práctico sería el siguiente:  

  ```bash
  chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/proyectos
  $ git init
  Initialized empty Git repository in D:/Trabajos/Cursos/proyectos/.git/
  ```
  
- **`Abrir editor de código desde la consola`:**  
Desde la terminal podemos **abrir directamente nuestro editor de código** en el directorio en el que nos encontremos trabajando. Esto es muy útil, ya que nos evita tener que buscar manualmente la carpeta desde la interfaz gráfica del editor. El comando que utilizaremos depende del editor que tengamos instalado. Por ejemplo, en el caso de **Visual Studio Code**, basta con escribir:  

  ```bash
  chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/proyectos
  $ code .
  ```

# 〰️ Flujo de Git  
Git trabaja con un **flujo definido** en el cual nuestros archivos van **pasando por diferentes estados** hasta finalmente llegar al repositorio remoto (estado final). Por lo que en total, podemos identificar **4 estados principales** que conforman el flujo de trabajo de Git:  

1. **Local (sin marcar):**  
   El primer paso dentro del flujo de Git sucede cuando tenemos nuestros archivos **locales** en una carpeta de proyecto. Para iniciar este proceso, ejecutamos el comando **`git init`**, con lo cual damos de alta nuestro proyecto en Git. A partir de este momento, Git reconoce que ese directorio será gestionado bajo su sistema de control de versiones, aunque **aún no hace nada con los archivos**. En este estado, simplemente hemos **inicializado el repositorio**, pero los archivos siguen siendo locales sin ningún seguimiento activo.  

2. **Stage (marcados):**  
   El segundo paso es el estado **Stage** (o “staging area”). Aquí usamos el comando **`git add .`**, lo que le indica a Git que tome nuestros archivos y los **marque** para que comiencen a ser rastreados. En este punto, Git crea una **copia temporal de los archivos** y empieza a observarlos. Eso significa que si los modificamos o eliminamos, Git detectará esos cambios. Es importante destacar que en esta etapa Git **no guarda todavía un historial permanente**, simplemente mantiene una **versión sincronizada temporal** de los archivos listos para ser confirmados. Si hacemos modificaciones y volvemos a ejecutar **`git add .`**, estas copias se actualizarán con los últimos cambios.  

3. **Commit (fotografiados):**  
   Este paso es uno de los más importantes y muchas veces se confunde con Stage. La diferencia es que el **commit crea una versión oficial en el historial del repositorio**. Cuando ejecutamos **`git commit -m "mensaje"`**, Git toma los archivos que estaban en Stage (agregados con `git add .`) y los **almacena en el historial como un punto de guardado permanente**, con un mensaje que describe los cambios realizados. A diferencia de Stage, donde solo hay archivos preparados, en el commit ya tenemos una **fotografía exacta del proyecto en ese momento**, registrada de forma cronológica en el historial de versiones.  

4. **Remote (en el servidor):**  
   Finalmente, llegamos al estado **Remote**, que representa el último paso del flujo de Git. Aquí tomamos las confirmaciones locales (commits) junto con su historial de cambios y las **subimos a un repositorio remoto**, como **GitHub, GitLab o Bitbucket**. Para ello utilizamos el comando **`git push`**, el cual envía toda la información al servidor remoto. Cabe destacar que para que esto funcione correctamente debemos haber **configurado previamente las credenciales** y conectado nuestro repositorio local al remoto.  

# ☄️ Git: add, status, comit

## ➕ git add  
  El comando **`git add`** se utiliza para **mover archivos de estado local a Stage**, de modo que Git comience a darles seguimiento. También sirve para **actualizar versiones de archivos que ya están en Stage** si han sido modificados o eliminados. Este comando cumple una función crucial, ya que **si no pasamos archivos de Local a Stage, estos nunca podrán ser registrados en un commit** (es decir, en una versión o copia del historial). Además, si los archivos ya están en Stage y realizamos cambios, **estos cambios no se registrarán en el próximo commit** a menos que volvamos a ejecutar `git add` para actualizar el Stage.  

  Algunas formas de usarlo:  
  - `git add <nombreArchivo>`: agrega un archivo específico al Stage.  
  - `git add <nombreCarpeta>/`: agrega todos los archivos dentro de esa carpeta al Stage.  
  - `git add .`: agrega **todos los archivos y carpetas del proyecto** al Stage, incluyendo los nuevos y los modificados.

Un ejemplo deñ uso de **`git add`** en la terminal es el siguiente:

```bash
chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/Git-GitHub-Course (main)
$ git add decription.txt
```

## 🔀 git commit  
El comando **`git commit`** se utiliza para **realizar un registro o “fotografía” del código** dentro del historial de versiones de Git. Este comando **toma los archivos que están confirmados en el área de Stage** (agregados mediante `git add`) y crea una nueva versión del proyecto.  Si existen archivos en Stage que fueron modificados después del último `git add`, pero **no se volvieron a agregar**, Git los **ignorará** al momento de realizar el commit, tomando como referencia **la versión anterior** que fue registrada con el último `git add`.  En otras palabras, **un commit guarda el estado actual del proyecto**, tomando en cuenta únicamente los archivos **agregados, modificados o eliminados** desde el último commit, **siempre y cuando estén en Stage**.  

Estos commits son **locales**, es decir, se almacenan únicamente en el repositorio de tu máquina. Sin embargo, posteriormente pueden **subirse a un repositorio remoto**, como **GitHub**, lo que permite sincronizar los cambios y compartir el trabajo con otros desarrolladores.  

Una ventaja importante de los commits es que **actúan como puntos de control o versiones de respaldo** del proyecto. Gracias a ellos, podemos:  
- **Volver a versiones anteriores** del código en caso de errores.  
- **Comparar diferencias** entre versiones para analizar cambios.  
- **Visualizar modificaciones o eliminaciones específicas**.  

Comúnmente, el comando **`git commit`** se acompaña del parámetro **`-m`**, el cual significa **message (mensaje)**. Esto se debe a que **todo commit debe tener un mensaje descriptivo** que permita identificar fácilmente los cambios realizados en esa versión. Cabe destacar que **el formato y estilo del mensaje del commit pueden variar** dependiendo de **las normas de la empresa, el equipo de desarrollo o las preferencias personales** del programador. Algunas organizaciones establecen convenciones estrictas (como usar prefijos tipo `feat:`, `fix:`, `refactor:` o `docs:`), mientras que otras permiten mensajes más libres siempre que sean claros y coherentes. Pero por lo general, se escribe una descripción **breve y clara** del propósito del commit, como por ejemplo:  
- `"Se corrigió el bug en la función de login"`  
- `"Se agregó el archivo README.md"`  
- `"Se optimizó el código de validación de formularios"`  


Cuando se ejecuta un commit, Git mostrará en la consola un **resumen informativo**, donde se incluye:  
- La **rama actual** en la que se hizo el commit.  
- El **identificador único (hash)** del commit creado.  
- El **número de archivos afectados**.  
- La **cantidad de inserciones, eliminaciones o modificaciones de líneas**.  

Este mensaje de confirmación indica que **el commit se ha realizado correctamente**, y nos brinda una visión rápida de los cambios registrados. Por lo que un ejemplo de un commit exitoso junto con su mensaje de confirmacion es el siguiente:

```bash
chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/Git-GitHub-Course/Course (main)
$ git commit -m "Update: Git Commit Description"
[main 797cfda] Update: Git Commit Description
 1 file changed, 2 insertions(+)
```

## 📊 git status  
   El comando **`git status`** es una herramienta fundamental en Git que nos permite **consultar el estado actual de los archivos dentro del repositorio**. Con este comando podemos saber exactamente **qué archivos han sido modificados, cuáles están sin seguimiento (untracked), cuáles están en Stage y cuáles están listos para ser confirmados (commiteados)**. Por ejemplo, cuando ejecutamos `git status`, Git analiza el directorio de trabajo y nos muestra información sobre los cambios realizados desde la última confirmación (`commit`). Por lo que un ejemplo de cómo se visualiza el uso del comando `git status` seria el siguiente:

   ```bash
   chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/Git-GitHub-Course (main)
   $ git status
   On branch main
   Your branch is up to date with 'origin/main'.
   
   Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git restore <file>..." to discard changes in working directory)
          modified:   Course/README.md

   Untracked files:
    (use "git add <file>..." to include in what will be committed)
          Practices/

   no changes added to commit (use "git add" and/or "git commit -a")
   ```

Ahora bien, pueden existir diferentes situaciones y funciones dentro del flujo de Git que pueden resultar confusas al principio, especialmente al manejar nuestros archivos. Aquí es donde **`git status`** se convierte en una herramienta clave, ya que nos permite **ubicar fácilmente el estado de nuestros archivos y entender qué acciones podemos tomar**. Recordemos que los **4 estados del flujo de Git** son: **local (sin seguimiento)**, **stage (marcados)**, **commit (fotografiados)** y **remote (en el servidor)**.  

### Archivos en estado Local (sin seguimiento)  
Cuando nuestros archivos están en el estado **local**, Git aún no les está dando seguimiento. En este caso, **`git status` nos mostrará una recomendación para usar `git add .`**, indicando que debemos agregarlos al Stage para comenzar a rastrearlos.  Es importante destacar que si hacemos un commit antes de agregar los archivos, **Git no los incluirá**, ya que aún no están marcados.  Ejemplo de cómo se mostraría un archivo local sin seguimiento:  

```bash
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Practices/
   ```

### Archivos en estado Stage (marcados)  
Una vez que marcamos nuestros archivos con `git add`, pasan al estado **Stage**, donde Git los observa para incluirlos en el próximo commit. Al ejecutar **`git status`** en este caso, la consola nos indicará que **hay cambios listos para ser confirmados**. Además, Git nos muestra sugerencias útiles, como **usar `git restore --staged` para desmarcar archivos y quitarles el estado Steg, regresandolos a estado local, esto sin alterar su contenido**. Ejemplo de cómo se muestra en la consola:  

 ```bash
   Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   "practices/\342\230\204\357\270\217 Git add, status, comit/file.txt"
   ```

### Acciones posibles en Stage antes de Commit  
Con los archivos ya en **Stage**, existen dos posibilidades:  

1. **Realizar un commit**:  
   Esto crea una “fotografía” de los archivos actuales, registrando los cambios en el historial de Git.  

2. **Modificar o eliminar archivos antes del commit**:  
   Si realizamos cambios en los archivos ya marcados, **`git status`** nos mostrará cuáles archivos han sido modificados o eliminados, y nos dará sugerencias de las posibles acciones que podemos realizar:  

   - **Agregar nuevamente los archivos modificados** con `git add .`:  
     Git nos dará esta sugerencia para incluir los cambios en el próximo commit. Esto es importante porque, si hacemos un commit sin agregar los archivos modificados, Git registrará y creará el commit en base a la versión **anterior** de los archivos, dejando fuera los cambios recientes.  

   - **Eliminar archivos** del proyecto usando `git rm`:  
     Git nos sugerirá esta acción para eliminar archivos tanto del Stage como del disco, reflejando correctamente la intención de borrarlos del proyecto. En caso de que un archivo eliminado ya estuviera en alguna versión previa del historial, al realizar un commit con el archivo eliminado, este dejará de aparecer en la versión más reciente del proyecto.  

   - **Quitar archivos del Stage** sin eliminarlos del proyecto usando `git restore --staged <file>`:  
     Esta acción mantiene los archivos dentro del proyecto, conservándolos en el directorio, pero **sin seguimiento temporal en Stage**. Mientras permanezcan fuera del Stage, los cambios no se incluirán en el próximo commit hasta que volvamos a agregarlos.  

   - **Restaurar archivos a la versión previamente agregada o del último commit** usando `git restore <file>`:  
     Esta acción nos permite restaurar nuestros archivos a una versión anterior antes de las modificaciones. Puede tomar como referencia la última versión guardada mediante un **commit** o la versión actual en **Stage** (después de un `git add .`). Si el archivo fue eliminado, se restaurará; si fue modificado, volverá al contenido de la versión previa.

     Ejemplo de cómo se muestran los cambios de archivos marcados con modificaciones o eliminados sin commit:  

     ```bash
     Changes not staged for commit:
          (use "git add/rm <file>..." to update what will be committed)
          (use "git restore <file>..." to discard changes in working directory)
                deleted:    "practices/\342\230\204\357\270\217 Git add, status, comit/file1.txt"
                modified:   "practices/\342\230\204\357\270\217 Git add, status, comit/file2.txt"
     ```

     Ahora bien, cuando realizamos un **commit** y se suben todos nuestros archivos a dicho commit —es decir, cuando absolutamente **todo lo que está en Stage ha sido actualizado y registrado correctamente**—, al ejecutar nuevamente el comando **`git status`**, Git nos mostrará un mensaje indicando que **no hay nada nuevo para confirmar (commit)**. Esto significa que **no existen cambios pendientes**, ya que todos los archivos fueron incluidos en el último commit y el estado del repositorio está completamente sincronizado. Por lo tanto, la consola mostrará un mensaje similar al siguiente:

     ```bash
     chris@LAPTOP-0DNMOIV6 MINGW64 /d/Trabajos/Cursos/Git-GitHub-Course/Course (main)
     $ git status
     On branch main
     Your branch is ahead of 'origin/main' by 1 commit.
       (use "git push" to publish your local commits)

     nothing to commit, working tree clean
     ```

# 😑 Git Ignore

