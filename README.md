# hello-world-cmake-msbuild

Generar y compilar un proyecto con `CMake`

## Compilar en windows con `CMake`

1) abrir simbolo del sistema para desarrolladores
2) ejecute los siguientes comandos

```bash
mkdir build
cd build
cmake ..
```

## Generar el ejecutable `exe` con `MSBuild`

* configure `MXBUILD_PATH`

```bash
set MSBUILD_PATH="C:\Program Files (x86)\Microsoft Visual Studio\2017\BuildTools\MSBuild\15.0\Bin\amd64\MSBuild"
```

* Generar el ejecutable

```bash
%MSBUILD_PATH% hello-world.sln /property:Configuration=Debug /property:Platform=x64
```
