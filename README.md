# Football Manager (C++)

Este es un proyecto en C++ llamado **Football Manager** que utiliza la biblioteca Crow para crear un servidor web. El proyecto está diseñado para manejar datos de un equipo de fútbol y proporcionar una API para interactuar con esos datos a través de solicitudes HTTP.

## Características

- Servidor web basado en **Crow** (un framework de C++ para crear aplicaciones web).
- Interacción con la API del servidor utilizando **HTTP**.
- Proyecto configurado con **CMake** para la compilación y administración de dependencias.
- Uso de **vcpkg** para la gestión de dependencias como Crow y Asio.

## Requisitos

- **C++17** o superior.
- **CMake** (Versión 3.10 o superior).
- **vcpkg** para la gestión de dependencias.

## Instalación

1. Clona el repositorio:

    ```bash
    git clone https://github.com/tu_usuario/FootballManager.git
    cd FootballManager
    ```

2. Instala las dependencias utilizando **vcpkg**:

    Si no tienes **vcpkg** instalado, sigue las instrucciones en [vcpkg GitHub](https://github.com/microsoft/vcpkg) para instalarlo. Luego, instala las dependencias requeridas:

    ```bash
    ./vcpkg install crow asio
    ```

3. Configura el proyecto con **CMake**:

    Dentro del directorio `build`, configura el proyecto con el archivo de configuración de **CMake**:

    ```bash
    mkdir build
    cd build
    cmake .. -DCMAKE_TOOLCHAIN_FILE=../vcpkg/scripts/buildsystems/vcpkg.cmake
    ```

4. Compila el proyecto:

    ```bash
    cmake --build .
    ```

## Ejecución

Una vez que la compilación se haya completado correctamente, puedes ejecutar el servidor:

```bash
./build/debug/server
