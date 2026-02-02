# Suma de arreglos en paralelo (OpenMP)

Este proyecto contiene un ejemplo minimalista de suma paralela de arreglos
con OpenMP, alineado con la guia y las instrucciones de la tarea.

## Requisitos
- Windows con Visual Studio 2022 (Desktop development with C++) o VS Build Tools
- CMake 3.20+ (si compilas con CMake)

## Configuracion en Visual Studio (sin CMake)
1. Crea un proyecto de consola en C++.
2. Activa OpenMP: Project Properties -> C/C++ -> Language -> OpenMP Support -> Yes (/openmp).
3. Si tu proyecto usa precompiled headers por defecto, desactivalos:
   C/C++ -> Precompiled Headers -> Not Using Precompiled Headers.
4. Copia `main.cpp` y compila.

## Build con CMake
```sh
cmake -S . -B build
cmake --build build --config Release
```

Ejecuta:
```sh
build/Release/suma_arreglos.exe
```

## Notas rapidas
- `N`, `chunk` y `mostrar` son constantes para tamano, pedazos y cantidad a imprimir.
- `imprimeArreglo` imprime los primeros `mostrar` valores del arreglo.

