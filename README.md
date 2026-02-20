# Binding Of Isaac -- C++ / SDL2

Clone del gioco *Binding of Isaac* sviluppato in C++ utilizzando SDL2.

Il progetto è stato realizzato nell'ambito del corso di:

Algoritmi e Programmazione di Videogiochi\
Laurea in Ingegneria Informatica e delle Telecomunicazioni (L-8)\
Università degli Studi di Cassino e del Lazio Meridionale (UNICAS)

Corso tenuto dal Prof. Alessandro Bria\
GitHub docente: https://github.com/abria

Il progetto è configurato con CMake e gestisce le dipendenze tramite
vcpkg.

------------------------------------------------------------------------

## Caratteristiche

-   Rendering 2D con SDL2\
-   Gestione sprite animati\
-   Sistema di collisioni\
-   Gestione audio (musica ed effetti sonori)\
-   Struttura modulare (src / include / utils)\
-   Build tramite CMake

------------------------------------------------------------------------

## Requisiti

-   CMake (\>= 3.31)\
-   Compilatore compatibile con C++14\
-   vcpkg\
-   SDL2\
-   SDL2_image\
-   SDL2_mixer

------------------------------------------------------------------------

## Installazione dipendenze

``` bash
vcpkg install sdl2 sdl2-image sdl2-mixer
```

------------------------------------------------------------------------

## Compilazione

``` bash
cmake -B build -S . -DCMAKE_TOOLCHAIN_FILE="C:/path/to/vcpkg/scripts/buildsystems/vcpkg.cmake"
cmake --build build --config Release
```

------------------------------------------------------------------------

## Avvio

Dopo la compilazione:

``` bash
build/Release/BindingOfIsaacCopy.exe
```

Gli assets vengono copiati automaticamente nella cartella
dell'eseguibile durante la build.

------------------------------------------------------------------------

## Struttura del progetto

    BindingOfIsaacCopy/
    │
    ├── assets/
    ├── src/
    │   ├── *.cpp
    │
    ├── include/
    │   ├── *.h
    │
    ├── utils/
    ├── CMakeLists.txt
    ├── vcpkg.json
    └── README.md

------------------------------------------------------------------------

## Release

Una versione Windows precompilata è disponibile nella sezione "Releases"
del repository GitHub.
