# CONTROL_DE_VERSIONES

## Definición

El Control de Versiones es un sistema esencial para el desarrollo de software que registra y gestiona los cambios y modificaciones realizados en los archivos de un proyecto. Permite realizar un seguimiento detallado de cada modificación, facilita la identificación de responsables, y posibilita revertir a estados anteriores en el tiempo. Esta herramienta no solo es fundamental para el historial de revisiones y la colaboración eficiente en equipos de desarrollo, sino que también desempeña un papel clave en entornos ágiles y en la metodología DevOps, contribuyendo a la automatización y garantizando la entrega rápida y segura de aplicaciones de alta calidad.

## Sistema de control de versiones y herramientas

En el contexto del desarrollo de software en equipos, se destaca la necesidad de llevar un registro efectivo de las continuas actualizaciones y cambios en el código fuente. La gestión de estas modificaciones puede volverse problemática, especialmente cuando varios desarrolladores trabajan simultáneamente en la misma base de código. El control de versiones emerge como la solución a estos desafíos, permitiendo un seguimiento detallado de los cambios. Se tienen dos tipos principales de sistemas de control de versiones: centralizados y distribuidos.

En el caso de los sistemas centralizados (CVCS), se destaca la presencia de un servidor que alberga el repositorio principal con el historial completo de versiones. Los desarrolladores extraen el código del servidor a sus máquinas locales, manteniendo una conexión esencial con el servidor para cada operación. Los cambios deben enviarse al servidor central después de realizar modificaciones.

En contraste, los sistemas distribuidos (DVCS) mantienen la esencia del modelo centralizado pero con una diferencia fundamental: cada usuario actúa como un servidor, teniendo acceso al historial completo de cambios localmente. Esto permite que los usuarios trabajen sin conexión, mejorando la velocidad y rendimiento en comparación con los CVCS.

Se abordan ventajas y desventajas de cada enfoque. Los CVCS son considerados más fáciles de aprender, pero pueden ser más lentos debido a la necesidad constante de conexión al servidor. Por otro lado, los DVCS ofrecen mayor velocidad y rendimiento, permitiendo a los usuarios trabajar sin conexión y acceder al historial completo localmente.

## Historia del control de versiones

El control de versiones es un sistema esencial en el desarrollo de software, registrando cambios en archivos para acceder a versiones específicas. Su origen se remonta a la década de 1980, siendo el Sistema de Versiones Concurrentes (CVS) uno de los primeros, creado en 1986. CVS, aunque popular, carecía de comprobaciones de integridad y no era ideal para archivos binarios.

Posteriormente, Subversion (SVN) surgió en 2000 como sucesor de CVS, abordando las deficiencias de su predecesor con comprobaciones de integridad y mejor soporte para archivos binarios. Sin embargo, SVN era centralizado, presentando inconvenientes en caso de fallos del servidor.

La necesidad de sistemas distribuidos condujo al desarrollo de Mercurial y Git en 2005. La revocación de la licencia de BitKeeper, utilizado por el núcleo Linux, impulsó la creación de Git por Linus Torvalds. Git, un VCS distribuido, ganó popularidad con su diseño y la oferta de alojamiento gratuito en GitHub para proyectos de código abierto, consolidándose como una opción preferida en la comunidad de desarrollo de software.

## Comandos UNIX

### Línea de comandos

La línea de comandos, también conocida como terminal o consola, es una interfaz de texto que permite a los usuarios interactuar con un sistema informático mediante la introducción de comandos específicos. A diferencia de las interfaces gráficas de usuario (GUI), que utilizan elementos visuales como ventanas y botones, la línea de comandos se basa en texto y requiere que los usuarios ingresen comandos de texto para ejecutar acciones y realizar operaciones en un sistema.

Se destaca que la línea de comandos es una herramienta poderosa para interactuar con un ordenador, especialmente para los desarrolladores. Ofrece la posibilidad de realizar una amplia variedad de tareas, desde la gestión de archivos hasta el control de servidores remotos y la automatización de procesos mediante scripts. Aunque puede tener una curva de aprendizaje empinada, se enfatiza que la recompensa por dominar la línea de comandos es significativa, ya que proporciona un mayor control y eficiencia en comparación con otras formas de interacción.

Se alienta a los usuarios a practicar comandos básicos para familiarizarse con la sintaxis y las funciones, y se proporciona ejemplos de comandos prácticos como `cd` para cambiar de directorio, `mkdir` para crear carpetas, `touch` para crear archivos, y `code` para abrir y editar archivos en el editor Visual Studio Code. 

### Comandos UNIX

Los comandos UNIX son instrucciones específicas que se introducen en la línea de comandos de un sistema operativo UNIX para llevar a cabo diversas operaciones y tareas. UNIX, un sistema operativo ampliamente utilizado en entornos de desarrollo y servidores, proporciona una interfaz basada en texto donde los usuarios pueden interactuar directamente con el sistema mediante comandos.

Estos comandos permiten realizar una variedad de acciones, desde la navegación por directorios hasta la manipulación de archivos, la administración de procesos y la configuración del sistema. La flexibilidad y potencia de los comandos UNIX han convertido a esta interfaz de línea de comandos en una herramienta fundamental para administradores de sistemas y desarrolladores.

Aunque puede haber una curva de aprendizaje asociada con los comandos UNIX, la eficiencia y el control que ofrecen son altamente valorados. Ejemplos de comandos UNIX comunes incluyen `cd` para cambiar de directorio, `ls` para listar archivos, `cp` para copiar archivos, `mv` para mover o renombrar archivos, y `grep` para buscar patrones dentro de archivos. La interacción con la línea de comandos UNIX permite a los usuarios realizar tareas de manera precisa y automatizada, brindando una potente herramienta para la administración y manipulación de sistemas.

### Uso de Bash en Windows: Creación y ejecución de Scripts

En el contexto del sistema operativo Windows, se ha abierto la ventana de la terminal para realizar operaciones en el entorno de Bash. Inicialmente, se navega hasta el directorio de inicio utilizando el comando `cd ~`. Posteriormente, se emplea `ls -la` para listar todos los archivos, incluyendo los ocultos, revelando dos archivos clave: `.bashrc` y `.bash_profile`.

El archivo `.bashrc` se destaca como un archivo de configuración ejecutado al abrir la ventana del terminal. Este script contiene ajustes para la consola, como la configuración de colores y preferencias de historial de comandos. Mediante el comando `less .bashrc`, se examina su contenido.

El archivo `.bash_profile` es otro archivo de configuración, frecuentemente utilizado para definir variables de entorno esenciales para el desarrollo. Al ejecutar `less .bash_profile`, se accede a su contenido, que puede incluir configuraciones específicas del sistema.

A continuación, se demuestra la creación de un script de shell simple denominado `testshell.sh` mediante el editor Vim. Este script básico utiliza la orden `echo` para imprimir "Hello World" en la pantalla. Después de guardarlo, se observa que el script no es ejecutable. Se utiliza el comando `chmod 755 testshell.sh` para asignar permisos de ejecución al archivo, permitiendo su ejecución.

Finalmente, se ejecuta el script con `./testshell.sh`, y se verifica que las palabras "Hello World" se imprimen en la pantalla, demostrando así cómo crear y ejecutar scripts simples en el entorno de Bash en Windows. Este proceso implica la combinación de comandos Bash y herramientas como `chmod` para gestionar permisos y Vim para la creación y edición de scripts.

A continuación, se presentan algunos ejemplos referetens a los comandos mencionados anteriormente.

**Ejemplo de configuración en .bashrc:**

```bash
# Archivo de configuración .bashrc
# Configuración de colores y preferencias de la consola

# Establecer colores para la interfaz de usuario
export PS1='\[\e[1;32m\]\u@\h:\w\$\[\e[0m\] '

# Configuración del historial de comandos
export HISTSIZE=1000
export HISTFILESIZE=2000
```

**Ejemplo de configuración en .bash_profile:**

```bash
# Archivo de perfil .bash_profile
# Configuración de variables de entorno para el desarrollo

# Directorio principal de Java
export JAVA_HOME=/ruta/a/java

# Directorio principal de Python
export PYTHON_HOME=/ruta/a/python
```

**Ejemplo de Script de Shell (testshell.sh):**

```bash
#!/bin/bash
# Script de ejemplo para imprimir "Hello World"

echo "Hello World"
```

**Ejemplo de cambio de permisos y ejecución del Script:**

```bash
# Cambiar permisos para hacer el script ejecutable
chmod 755 testshell.sh

# Ejecutar el script
./testshell.sh
```

Estos ejemplos ilustran cómo configurar la interfaz de usuario, establecer variables de entorno y crear un script básico en el entorno de Bash en Windows. Además, se muestra cómo cambiar los permisos y ejecutar un script.

### Cambiar directorios y listar contenidos

**Cambiar Directorios:**

Para cambiar de directorio en la línea de comandos de Bash, se utiliza el comando `cd` seguido del nombre del directorio al que se desea acceder. Aquí tienes algunos ejemplos:

```bash
# Cambiar al directorio de inicio del usuario
cd ~

# Cambiar al directorio superior (padre)
cd ..

# Cambiar a un directorio específico
cd ruta/del/directorio
```

**Listar Contenidos:**

Para listar el contenido de un directorio, el comando comúnmente utilizado es `ls`. Aquí hay algunos ejemplos:

```bash
# Listar archivos y directorios en el directorio actual
ls

# Listar archivos con detalles (tamaño, permisos, propietario, etc.)
ls -l

# Listar todos los archivos, incluyendo los ocultos
ls -a

# Listar archivos con detalles, incluyendo los ocultos
ls -la
```

### Crear y mover directorios y archivos

En el contexto de la línea de comandos Bash, realizar operaciones como crear, mover directorios y archivos es fundamental para la gestión de archivos y la organización del sistema de archivos. Aquí se presentan ejemplos de comandos para llevar a cabo estas acciones.

1. **Verificar Directorio Actual:**
   ```bash
   # Comprobar el directorio actual
   pwd
   ```

2. **Listar Contenido del Directorio Actual:**
   ```bash
   # Listar contenido del directorio actual
   ls -l
   ```

3. **Crear un Nuevo Directorio:**
   ```bash
   # Crear un nuevo directorio llamado "submissions"
   mkdir submissions
   ```

4. **Entrar en un Directorio:**
   ```bash
   # Cambiar al directorio "submissions"
   cd submissions
   ```

5. **Crear Archivos de Texto:**
   ```bash
   # Crear archivos de texto "prueba1.txt" y "prueba2.txt"
   touch prueba1.txt
   touch prueba2.txt
   ```

6. **Volver al Directorio Raíz:**
   ```bash
   # Regresar al directorio raíz
   cd ..
   ```

7. **Crear Otro Directorio:**
   ```bash
   # Crear un nuevo directorio llamado "archive"
   mkdir archive
   ```

8. **Mover Directorio a Otro Directorio:**
   ```bash
   # Mover el directorio "submissions" al directorio "archive"
   mv submissions archive
   ```

9. **Verificar Cambios:**
   ```bash
   # Verificar cambios con lista detallada
   ls -l
   ```

10. **Entrar en un Directorio Movido:**
   ```bash
   # Entrar en el directorio "archive"
   cd archive
   ```

11. **Verificar Contenido del Nuevo Directorio:**
    ```bash
    # Verificar contenido del directorio "archive"
    ls -l
    ```
### Redirección en la Línea de Comandos

Se abordará el concepto de redirección en la línea de comandos de Linux, destacando los tres tipos principales: entrada estándar, salida estándar y error estándar. 

 1. Entrada Estándar:

La entrada estándar representa la información que un usuario ingresa, generalmente desde el teclado. El comando `cat` se presenta como una herramienta que puede registrar esta entrada y almacenarla en un archivo. El ejemplo práctico utiliza el comando `cat`, seguido de un signo mayor que (`>`) y el nombre del archivo (`input.txt`), permitiendo la creación y almacenamiento de la entrada del usuario en un archivo de texto.

```bash
# Ejemplo de Redirección de Entrada Estándar
cat > input.txt
```

 2. Salida Estándar:

La salida estándar es la información generada por comandos como `ls`, que por defecto se envía a la pantalla. La redirección de salida se realiza mediante el uso del signo mayor que (`>`), permitiendo que la salida se guarde en un archivo específico, como se muestra en el siguiente ejemplo:

```bash
# Ejemplo de Redirección de Salida Estándar
ls -l > output.txt
```

 3. Error Estándar:

Cuando se producen errores, es crucial gestionar la salida de error estándar. Se utiliza el número 2 para representar el error, y se puede combinar con la salida estándar utilizando `2>&1`. El siguiente ejemplo muestra cómo manejar errores y salida estándar al mismo tiempo:

```bash
# Ejemplo de Redirección de Error Estándar y Salida Estándar
ls /bin/usr > error_output.txt 2>&1
```

En este caso, si el directorio no existe, el mensaje de error se guarda en el archivo `error_output.txt`, proporcionando un registro detallado.

La redirección es una herramienta poderosa para controlar el flujo de datos en la línea de comandos de Linux, permitiendo un manejo eficiente de la entrada, salida y errores generados por diferentes comandos. Con estos ejemplos, los usuarios pueden comprender y aplicar efectivamente los conceptos de redirección en sus tareas diarias en entornos UNIX y Linux.

### Grep

Grep es una herramienta poderosa en la línea de comandos de Unix y Linux que se utiliza para buscar patrones en archivos y directorios. La sigla Grep proviene de "Global Regular Expression Print". En el contexto del texto, se muestra cómo Grep se utiliza para buscar nombres en un archivo llamado `nombres.txt`.

**Ejemplos de uso de Grep:**

1. *Búsqueda Estándar:*
   ```bash
   grep Sam nombres.txt
   ```
   Devuelve nombres que comienzan por "Sam". Se destaca que Grep distingue entre mayúsculas y minúsculas.

2. *Búsqueda sin Distinguir Mayúsculas y Minúsculas:*
   ```bash
   grep -i Sam nombres.txt
   ```
   Ignora la distinción entre mayúsculas y minúsculas, devolviendo coincidencias independientemente de la capitalización.

3. *Coincidencia Exacta:*
   ```bash
   grep -w Sam nombres.txt
   ```
   Realiza una coincidencia exacta, excluyendo coincidencias parciales de "Sam".

4. *Uso de Pipe para Combinar Comandos:*
   ```bash
   ls /bin | grep zip
   ```
   Combina el comando `ls` con Grep utilizando el pipe (`|`) para filtrar los archivos ejecutables que contienen la palabra "zip".

Grep proporciona flexibilidad en la búsqueda de patrones en archivos y directorios, permitiendo ajustar los resultados según las necesidades. Puede utilizarse para realizar búsquedas sensibles a mayúsculas y minúsculas, coincidencias exactas, y filtrar resultados combinándolo con otros comandos mediante el uso de pipes. En resumen, Grep es una herramienta esencial para aquellos que buscan eficientemente a través de grandes conjuntos de datos en entornos de línea de comandos.

## Git y GitHub 

En el desarrollo web y de software, el control de versiones es esencial para hacer un seguimiento de los cambios en los proyectos. Git y GitHub son dos herramientas fundamentales en este contexto. Git es un sistema de control de versiones diseñado para rastrear cambios en archivos, inicialmente creado para abordar el desafío de gestionar las contribuciones masivas al núcleo del sistema operativo Linux. Ofrece ventajas como velocidad, rendimiento, confiabilidad y una sintaxis accesible.

Por otro lado, GitHub es un servicio de alojamiento basado en la nube que facilita la gestión de repositorios de Git a través de una interfaz de usuario. Va más allá de las funciones de control de versiones de Git, proporcionando herramientas como control de acceso, solicitudes de cambios y automatización. GitHub actúa como una red social para desarrolladores, con proyectos públicos y privados, perfiles de usuarios y la capacidad de aceptar contribuciones globales.

**Detalles clave sobre Git:**

- Sistema de control de versiones diseñado para rastrear cambios en archivos.
- Creado para superar los desafíos de gestionar contribuciones masivas en el núcleo de Linux.
- Ventajas: mayor velocidad, rendimiento, confiabilidad, código abierto y sintaxis accesible.
- Se utiliza principalmente a través de la línea de comandos.

**Detalles Clave sobre GitHub:**

- Servicio de alojamiento basado en la nube para gestionar repositorios de Git.
- Incorpora funciones de control de versiones de Git y añade sus propias herramientas.
- Funciones incluyen control de acceso, solicitudes de cambios y automatización.
- Popular entre los desarrolladores web, actúa como una red social para proyectos.

### Creación y clonación de un repositorio

El proceso de creación y clonación de un repositorio en GitHub se inicia desde el sitio web y luego se completa en la línea de comandos. Al iniciar sesión en GitHub, se utiliza la opción "Crear repositorio" para iniciar un nuevo proyecto. Se elige un nombre, una descripción y la visibilidad del repositorio (público o privado). Además, se puede inicializar el repositorio con archivos como README. Después de la creación, se presenta una URL que se utilizará para clonar el repositorio.

Para clonar el repositorio en la máquina local, se copia la URL HTTPS y se utiliza el comando `git clone` en la línea de comandos. El proceso incluye la creación de un directorio local, la ejecución del comando de clonación y la verificación de la presencia del repositorio clonado en el sistema de archivos local. 

**Pasos Detallados:**
1. Iniciar sesión en GitHub y seleccionar "Crear repositorio".
2. Ingresar el nombre del repositorio, descripción y configuración de visibilidad.
3. Opcionalmente, inicializar el repositorio con archivos como README.
4. Crear el repositorio y obtener la URL de clonación.
5. Copiar la URL HTTPS para clonar el repositorio en la máquina local.
6. En la línea de comandos, crear un directorio y usar `git clone` con la URL copiada.
7. Verificar la presencia del repositorio clonado en el sistema de archivos local.

Este proceso proporciona a los desarrolladores una manera eficiente de crear y clonar repositorios, estableciendo así la base para el trabajo colaborativo y el control de versiones.

**Observaciones Finales:**
- Se destaca la importancia del archivo README.md en el repositorio, utilizado para proporcionar documentación utilizando el formato Markdown.
- Se menciona que cada repositorio tiene una rama principal (main), conocida como la "línea principal", fundamental en el control de versiones.

Al comprender estos pasos, los desarrolladores pueden iniciar y colaborar en proyectos utilizando GitHub de manera efectiva, estableciendo un flujo de trabajo sólido en el desarrollo de software.

### ¿Cómo funciona Git?

Git es un sistema de control de versiones distribuido que permite a los desarrolladores rastrear y gestionar cambios en sus proyectos de software de manera eficiente. Su funcionamiento se basa en un conjunto de principios y comandos que constituyen su flujo de trabajo. Aquí hay una descripción sobre cómo funciona Git:

1. **Creación y Clonación de Repositorios:**
   - Se inicia creando un repositorio local mediante el comando `git init` o clonando un repositorio existente con `git clone`.
   - El repositorio local contiene tanto el directorio de trabajo como una carpeta oculta llamada `.git`, que almacena toda la información sobre el historial y las versiones del proyecto.

2. **Áreas de Trabajo en Git:**
   - **Directorio de Trabajo:** Es donde se encuentran y se editan los archivos del proyecto.
   - **Área de Staging:** Los archivos modificados se colocan en esta área con `git add` para prepararlos para el siguiente commit.
   - **Repositorio Local:** Después de hacer `git commit`, los archivos en el área de staging se guardan en el repositorio local con un mensaje descriptivo.

3. **Ciclo de Vida de los Archivos:**
   - **Modificado:** Archivo editado pero no marcado para commit.
   - **Staging:** Archivo marcado para el próximo commit.
   - **Comprometido:** Archivo guardado en la base de datos del repositorio.

4. **Flujo de Trabajo Básico:**
   - Se inicia un proyecto con `git init`.
   - Los cambios se registran con `git add` para pasar al área de staging.
   - Se confirman los cambios con `git commit`.
   - Este proceso se repite a medida que se realizan modificaciones en el proyecto.

5. **Gestión de Ramas:**
   - Las ramas permiten trabajar en paralelo en funcionalidades o correcciones sin afectar la rama principal (normalmente llamada `main` o `master`).
   - Se crea una nueva rama con `git branch` y se cambia con `git checkout` o `git switch`.
   - Después de realizar cambios en una rama, se pueden fusionar con otras utilizando `git merge`.

6. **Colaboración y Repositorios Remotos:**
   - Repositorios remotos, como GitHub, actúan como puntos de colaboración.
   - `git push` se utiliza para enviar cambios a un repositorio remoto.
   - `git pull` permite obtener cambios de un repositorio remoto, manteniendo el proyecto actualizado.

7. **Manejo de Conflictos:**
   - Git facilita la resolución de conflictos cuando dos ramas contienen cambios en las mismas líneas de código.
   - Se utilizan herramientas como `git diff` y `git merge` para resolver y fusionar cambios conflictivos.

### Añadir y confirmar

A continuación, se describe el proceso de trabajo con Git, centrándose en el manejo de archivos y confirmaciones en un repositorio local. Vamos a comenzar con la visualización del estado del directorio actual mediante el comando `pwd` que muestra la ubicación y `ls -la` para listar todos los elementos, incluyendo archivos ocultos. El comando `git status` se utiliza para obtener información sobre el estado del repositorio, destacando cambios no confirmados, la rama actual y la limpieza del árbol de trabajo.

Posteriormente, se introduce la adición de un nuevo archivo, "test.txt", mediante el comando `touch test.txt`. Para incluir este archivo en la próxima confirmación, se utiliza `git add test.txt`. Se explica que este paso es crucial, ya que prepara los cambios en el área de staging antes de la confirmación.

El texto aborda la gestión de cambios escalonados. Se muestra cómo revertir cambios escalonados usando `git restore --stage test.txt` y cómo realizar una confirmación con `git commit -m "Agrega un nuevo archivo para probarlo"`. Además, se destaca la importancia del área de staging para preparar cambios antes de confirmarlos.

Finalmente, se menciona que los cambios locales se envían al servidor remoto con `git push`. Se subraya que esta acción es crucial en un entorno distribuido, donde los cambios en la máquina local solo se reflejarán en el servidor remoto después de ejecutar el comando `push`.

A continuación, se muestra el código mencionado anteriormente:

1. Visualización del directorio actual y listado de elementos:

```bash
# Comando para mostrar la ubicación actual
pwd

# Comando para listar todos los elementos, incluyendo los ocultos
ls -la
```

2. Obtener información sobre el estado del repositorio:

```bash
# Comando para ver el estado del repositorio
git status
```

3. Creación de un nuevo archivo "test.txt" y adición al área de staging:

```bash
# Comando para crear un nuevo archivo
touch test.txt

# Comando para añadir el archivo al área de staging
git add test.txt
```

4. Revertir cambios escalonados:

```bash
# Comando para revertir cambios escalonados en un archivo
git restore --stage test.txt
```

5. Realizar una confirmación:

```bash
# Comando para realizar una confirmación con mensaje
git commit -m "Agrega un nuevo archivo para probarlo"
```

6. Enviar cambios locales al servidor remoto:

```bash
# Comando para enviar cambios locales al servidor remoto
git push
```

### Ramas

Se detallará el procedimiento para trabajar con ramas en Git. En primer lugar, se inicia con la verificación del directorio actual a través del comando `pwd`, seguido de la exploración de los elementos en el directorio mediante `ls -la`.

Posteriormente, se recomienda ejecutar `git status` para asegurarse de que no hay confirmaciones pendientes y que el estado del shell está limpio. Este comando también informa sobre la rama actual y si está actualizada con la rama principal remota.

Luego, se introduce la creación de una nueva rama denominada "feature/lesson-highlighted" con el comando `git checkout -b feature/lesson-highlighted` o alternativamente usando `git branch` y `git checkout` por separado. Se destaca que la diferencia clave entre estos enfoques radica en que `git checkout -B` no solo crea la rama sino que también mueve el usuario a esa rama recién creada.

La acción siguiente implica la adición de un archivo llamado "test2.txt" a la nueva rama. Se emplean los comandos `touch test2.txt`, `git add test2.txt` para añadir el archivo al área de staging, y `git commit -m "Agrega un nuevo archivo test2.txt"` para confirmar los cambios.

Para compartir estos cambios con el repositorio remoto, se ejecuta `git push -u origin feature/lesson-highlighted`, destacando la práctica de especificar `-u` para recibir actualizaciones de la rama principal.

La solicitud de extracción se realiza en la interfaz de usuario de GitHub, donde se compara y solicita la extracción de los cambios en la rama creada con la rama principal.

La fusión de ramas se efectúa en GitHub, seguida de la opción de eliminar o conservar la rama después de confirmar la fusión. Finalmente, se verifica la presencia de los cambios en la rama principal local mediante `git checkout main`, `git pull`, y la comprobación de los archivos con `ls`.

Este flujo de trabajo detallado proporciona una comprensión completa de cómo trabajar con ramas en Git, desde la creación hasta la fusión, facilitando la colaboración y el desarrollo de software en equipo.

A continuación, se presenta el código correspondiente a las acciones descritas en el texto:

1. Verificar el directorio actual y explorar sus elementos:
   
```bash
pwd
ls -la
```

2. Comprobar el estado de Git:
   
```bash
git status
```

3. Crear y cambiar a una nueva rama:
   
```bash
git checkout -b feature/lesson-highlighted
```
O alternativamente:

```bash
git branch feature/lesson-highlighted
git checkout feature/lesson-highlighted
```

4. Añadir un nuevo archivo y confirmar los cambios:
   
```bash
touch test2.txt
git add test2.txt
git commit -m "Agrega un nuevo archivo test2.txt"
```

5. Compartir los cambios con el repositorio remoto:
   
```bash
git push -u origin feature/lesson-highlighted
```

6. Realizar una solicitud de extracción en la interfaz de usuario de GitHub.

7. Fusionar las ramas en GitHub y confirmar la fusión.

8. Verificar la rama principal local y obtener los últimos cambios:
   
```bash
git checkout main
git pull
```

9. Verificar la presencia de los archivos en la rama principal:
    
```bash
ls
```

Estos comandos representan el flujo de trabajo descrito en el texto para trabajar con ramas en Git.

### Remoto frente a local

En el contexto de Git, se refiere a la distinción entre los repositorios locales y remotos. Un repositorio local es la copia del proyecto que se encuentra en la máquina del usuario, mientras que un repositorio remoto es una versión del proyecto almacenada en un servidor, que puede ser accesible y compartida por varios desarrolladores.

1. **Repositorio Local:**
   - Es la copia del proyecto que reside en la máquina del usuario.
   - Las operaciones como la creación de ramas, confirmación de cambios y experimentación se realizan localmente.
   - Los cambios realizados en el repositorio local no afectan directamente al repositorio remoto.

   Ejemplo de operaciones locales:
   ```bash
   git init  # Inicializar un nuevo repositorio local
   git add <file>  # Añadir un archivo al área de preparación
   git commit -m "Mensaje de confirmación"  # Confirmar cambios
   ```

2. **Repositorio Remoto:**
   - Es una versión del proyecto almacenada en un servidor.
   - Permite la colaboración entre varios desarrolladores, ya que todos trabajan con la misma versión remota.
   - Cambios confirmados en el repositorio local se pueden enviar al repositorio remoto mediante comandos como `git push`.

   Ejemplo de operaciones remotas:
   ```bash
   git remote add origin <URL>  # Asociar el repositorio local a un repositorio remoto
   git push -u origin master  # Enviar cambios locales a la rama principal del repositorio remoto
   ```

**Importancia:**
- La distinción entre local y remoto facilita el desarrollo colaborativo, ya que múltiples desarrolladores pueden trabajar en sus versiones locales y luego compartir y fusionar sus cambios en el repositorio remoto.
- Los repositorios remotos permiten la sincronización y la centralización del código fuente, lo que es crucial para proyectos en los que varios desarrolladores contribuyen.

### Empujar y tirar

**Empujar y Tirar en Git:**

En el contexto de Git, "empujar" y "tirar" son operaciones fundamentales para sincronizar cambios entre un repositorio local y un repositorio remoto. Aquí se detalla cada uno de estos conceptos con ejemplos de códigos:

1. **Empujar (Push):**
   - **Definición:** Empujar se refiere a enviar los cambios confirmados desde el repositorio local al repositorio remoto, actualizando así la versión remota con las últimas modificaciones locales.
   - **Ejemplo de Código:**
     ```bash
     git push origin main
     ```
     Este comando empuja los cambios de la rama local "main" al repositorio remoto llamado "origin".

2. **Tirar (Pull):**
   - **Definición:** Tirar se utiliza para obtener y aplicar los últimos cambios del repositorio remoto al repositorio local, asegurando que ambas versiones estén sincronizadas.
   - **Ejemplo de Código:**
     ```bash
     git pull origin main
     ```
     Este comando tira los cambios de la rama remota "main" al repositorio local desde el repositorio remoto "origin".

**Detalles Adicionales:**
- Antes de realizar un push, es aconsejable ejecutar un pull para obtener los últimos cambios del repositorio remoto y reducir la posibilidad de conflictos.
- El comando `git status` muestra información sobre la relación entre las ramas local y remota, indicando si hay cambios pendientes de empujar o si la rama local está adelante de la rama remota.

**Importancia:**
- Empujar y tirar son esenciales en un entorno colaborativo, donde varios desarrolladores trabajan en un proyecto. Facilitan la colaboración y aseguran que todos estén trabajando con la versión más reciente del código.
- Git maneja automáticamente fusiones si no hay conflictos, simplificando el proceso de mantener actualizados tanto el repositorio local como el remoto.

