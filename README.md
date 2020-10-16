# sd-cpp

Helper git repository for the development of the sdevent and sdbus libraries.
This repository contains both libraries as git submodules.
It also provides a minimal cmake project to compile both libraries reproducibly with tests.

## Dependencies (Fedora)

```sh
dnf groupinstall "Development Tools" "Development Libraries"
dnf install expat-devel gtest-devel cmock-devel cmake ninja-build
```

## Build

```sh
mkdir build
cmake -DCMAKE_BUILD_TYPE=Debug -B./build -G Ninja
cmake --build ./build -- -j 6
```
