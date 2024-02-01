# Configuración de nuestra terminal en windows y linux para darle un mejor estilo

<br>

## 1. Configuración de la terminal de Windows

### Imagen de muestra de como quedaría nuestra terminal ya configurada

![Windows Terminal Complete](Windows.Terminal/Windows-Terminal-Complete.jpg)

### Para la configuración vamos a necesitar tener instalado lo siguiente:

1. Windows Terminal (Instalar desde Microsoft Store): Una versión nueva de la terminal que nos permite configurar diferentes opciones.
2. PowerShell (Instalar desde Microsoft Store): Ultima versión de la PowerShell de Microsoft Windows.
3. OhMyPosh (Instalar desde powershell): OhMyposh permite agregarle un tema a nuestra terminal, sea powershell en windows o alguna como bash en linux, en este caso lo usaremos en windows.
4. Terminal-Icons (Instalar desde powershell): Terminal-Icons es un módulo que nos permite visualizar diferentes íconos a nuestras carpetas y archivos al usar comandos en nuestra powershell.

Para instalar OhMyPosh debemos ver la documentación en su [Web oficial](http://ohmyposh.dev) donde vienen todos los pasos.

Les dejo los archivos de mi configuración al igual que el documento [WindowsTerminalPwshell.md](https://github.com/infinityxgame/Windows-Linux-Terminal-Config/blob/main/WindowsTerminalPwshell.md) donde viene detallado todo el proceso que se debe realizar, así les ahorro tiempo en leer la doc oficial e incluso vienen otros detalles que no vienen con OhMyPosh y son de utilidad.

Archivos de configuración (Dentro de la carpeta Windows-Config):
1. settings.json 
2. Microsoft.PowerShell_profile.ps1
3. InfinityxGame.omp.json

**settings.json**: contiene la configuración de la terminal donde dentro esta mi tema personalizado, es solo copiar el código del tema y pegarlo en el lugar correspondiente dentro de la configuración de la misma, ojo esto es el tema como tal de la terminal no el de la línea de comandos

**Microsoft.PowerShell_profile.ps1**: configuración predeterminada que debe debe ejecutar PowerShell al abrir la terminal 

**InfinityxGame-Linux.omp.json**: El tema personalizado que uso en OhMyPosh, es una versión del tema half-life.omp.json que viene incluído dentro del programa pero con cambios a mi gusto. Si desean utilizar este tema solo tienen que descargar el archivo y copiarlo en la siguiente ruta: C:\Users\username\AppData\Local\Programs\oh-my-posh\themes\, cambiando lo que dice "username" por tu nombre de usuario en windows y para aplicarlo editar el $PROFILE de powershell y editar el nombre del tema.

## 2. Configuración en la terminald de Linux

### Imagen de muestra de como quedaría nuestra terminal ya configurada

![Linux Terminal Complete](Linux.Terminal/Linux-Terminal-Full.jpg)

Nota: No se fijen en el nombre de la ventana ya que dice powershell pero en realidad es ubuntu, eso pasa porque tengo instalado ubuntu en wsl (subsistema de windows para linux) y como estoy utulizando la nueva terminal a veces no pone bien el nombre al abrir wsl. 

### Para la configuración en linux solo vamos a necesitar tener instalado dos cosas:


1. OhMyPosh (Instalar desde la terminal): OhMyposh permite agregarle un tema a nuestra terminal, sea powershell en windows o alguna como bash en linux, en este caso lo usaremos en linux.

2. lsd: LSD es un proyecto cuya finalidad consiste en colorear la salida del comando ls con su respectivos iconos

Para instalar OhMyPosh debemos ver la documentación en su [Web oficial](http://ohmyposh.dev) donde vienen todos los pasos.

Les dejo los archivos de mi configuración al igual que el documento [WindowsTerminal.md](enlace aquí) donde viene detallado todo el proceso que se debe realizar.

Como archivos de configuración solo voy a dejar uno que sería mi tema personalizado, es el mismo que uso en la PowerShell pero tiene un cambio menor para poder identificar cuando estoy en una terminal o en la otra.

Archivos de configuración (Dentro de la carpeta Linux-Config):

1. InfinityxGame.omp.json

**InfinityxGame-Linux.omp.json**: El tema personalizado que uso en OhMyPosh, es una versión del tema half-life.omp.json que viene incluído dentro del programa pero con cambios a mi gusto. Si desean utilizar este tema solo tienen que descargar el archivo y copiarlo en ruta que usted desee, en mi caso lo tengo en el HOME de mi usuario de sistema en una carpeta que cree llamada ".poshtheme", y para aplicar el tema solo tienen que poner dentro de su archivo .bashrc o .profile dependiendo de tu distribución y de la consola que uses lo siguiente:

```eval "$(oh-my-posh init bash --config ~/.poshthemes/InfinityxGame.omp.json)"```

Donde "~/.poshthemes/InfinityxGame.omp.json" es la ruta donde esta el archivo de mi tema.

### Espero te sirva, adios :wave:.
