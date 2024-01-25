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
