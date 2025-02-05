# ProyectoProgra1

-Archivo main.c esqueleto base de toda la aplicacion
-Function.h archivo con todas las funciones que hacen funcionar el programa
-Static.h archivo con todas las struct y variables globales que el programa necesita
# Ultima Version

- Problema de reproduccion de audio arreglados
# ProyectoProgra1

-Archivo main.c esqueleto base de toda la aplicacion
-Function.h archivo con todas las funciones que hacen funcionar el programa
-Static.h archivo con todas las struct y variables globales que el programa necesita
# Ultima Version

- Problema de reproduccion de audio arreglados

# Como correr el juego en Visual Studio
1. Seguir la guia de instalacion de SDL2 para Visual Studio 2019: https://lazyfoo.net/tutorials/SDL/01_hello_SDL/windows/msvc2019/index.php
2. Instalar SDL2_ttf (https://github.com/libsdl-org/SDL_ttf/releases), SDL2_Image (https://github.com/libsdl-org/SDL_image/releases), SDL2_mixer (https://github.com/libsdl-org/SDL_mixer/releases)
3. Agregar las biblotecas adicionales a las configuraciones: Solution explorer -> Properties -> C/C++ -> General -> Additional Incluude Directories 
> "C:\SDL2\SDL2-2.x.x\include"
> "C:\SDL2\SDL2_ttf-2.x.x\include"
> "C:\SDL2\SDL2_image-2.x.x\include"
> "C:\SDL2\SDL2_mixer-2.x.x\include"
4. Agregar las bibloteas adicionales al Linker: Solution explorer -> Properties -> Linker -> General -> Additional Libary Directories 
> "C:\SDL2\SDL2-2.x.x\lib\x64"
> "C:\SDL2\SDL2_ttf-2.x.x\lib\x64"
> "C:\SDL2\SDL2_image-2.x.x\lib\x64"
> "C:\SDL2\SDL2_mixer-2.x.x\lib\x64"
5. Agregar biblotecas a dependencias adicionales: Solution explorer -> Properties -> Linker -> Input -> Additional Dependencies 
> "SDL2.lib"
> "SDL2main.lib"
> "SDL2_ttf.lib"
> "SDL2_image.lib"
> "SDL2_mixer.lib"
6. Copiar los dll junto al ejecutable del proyecto (donde esta el .exe o el vcxproj)
> "SDL2.dll"
> "SDL2_ttf.dll"
> "SDL2_image.dll"
> "SDL2_mixer.dll"
7. Cambiar los include dentro del codigo: #include <SDL2/SDL2.h> -> #include "SDL.h"
8. Agregar todos los archivos del juego al proyecto (en root)

