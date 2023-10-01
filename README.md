# Configuración de la terminal de windows para darle un mejor estilo

### Imagen de muestra de como quedaría nuestra terminal ya configurada

![Windows Terminal Complete](Windows.Terminal/Windows-Terminal-Complete.jpg)

### Para la configuración vamos a necesitar tener instalado lo siguiente:

1. Windows Terminal (Instalar desde Microsoft Store): Una versión nueva de la terminal que nos permite configurar diferentes opciones.
2. PowerShell (Instalar desde Microsoft Store): Ultima versión de la PowerShell de Microsoft Windows.
3. OhMyPosh (Instalar desde powershell): OhMyposh permite agregarle un tema a nuestra terminal, sea powershell en windows o alguna como bash en linux, en este caso lo usaremos en windows.
4. Terminal-Icons (Instalar desde powershell): Terminal-Icons es un módulo que nos permite visualizar diferentes íconos a nuestras carpetas y archivos al usar comandos en nuestra powershell.

Para instalar OhMyPosh debemos ver la documentación en su [Web oficial](http://ohmyposh.dev) donde vienen todos los pasos.

Les dejo los archivos de mi configuración al igual que el documento [WindowsTerminal.md](https://github.com/infinityxgame/Windows-Terminal-Config/blob/main/WindowsTerminal.md) donde viene detallado todo el proceso que se debe realizar, así les ahorro tiempo en leer la doc oficial e incluso vienen otros detalles que no vienen con OhMyPosh y son de utilidad.

Archivos de configuración:
1. settings.json 
2. Microsoft.PowerShell_profile.ps1
3. InfinityxGame.omp.json

**settings.json**: contiene la configuración de la terminal donde dentro esta mi tema personalizado, es solo copiar el código del tema y pegarlo en el lugar correspondiente dentro de la configuración de la misma, ojo esto es el tema como tal de la terminal no el de la línea de comandos

**Microsoft.PowerShell_profile.ps1**: configuración predeterminada que debe debe ejecutar PowerShell al abrir la terminal 

**InfinityxGame.omp.json**: El tema personalizado que uso en OhMyPosh, es una versión del tema half-life.omp.json que viene incluído dentro del programa pero con cambios a mi gusto. Si desean utilizar este tema solo tienen que descargar el archivo y copiarlo en la siguiente ruta: C:\Users\username\AppData\Local\Programs\oh-my-posh\themes\, cambiando lo que dice "username" por tu nombre de usuario en windows y para aplicarlo editar el $PROFILE de powershell y editar el nombre del tema.
