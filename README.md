# Elmer Landana  -  versión 0.1

Efecto lo-fi para Ableton (VST3): saturación de cinta, bitcrusher, reducción de
sample rate, wow & flutter, filtros HP/LP, hiss y crackle de vinilo.

- 1000 presets (25 categorías x 40 intensidades)
- Modo oscuro / claro con un interruptor
- 10 temas de color futuristas
- Visualizador de nivel de salida

## Compilar en Windows
Requisitos: Visual Studio 2022 (carga "Desarrollo para el escritorio con C++"), CMake y Git.

    cmake -B build -DCMAKE_BUILD_TYPE=Release
    cmake --build build --config Release

Resultado: build\ElmerLandana_artefacts\Release\VST3\Elmer Landana.vst3

## Instalar en Ableton
1. Copia la carpeta "Elmer Landana.vst3" a C:\Program Files\Common Files\VST3\
2. Ableton > Preferences > Plug-Ins > activa "Use VST3 Plug-In System Folders" y pulsa Rescan.
3. Aparece en Plug-Ins > Elmer Landana > Elmer Landana.

## Sin instalar nada
Sube esta carpeta a un repositorio de GitHub: la acción .github/workflows/build.yml
compila el VST3 y lo deja como artefacto descargable en la pestaña Actions.
