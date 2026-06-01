# Automatización de Infraestructura Digital – Unidad I

## Alumno

Samuel Reynaldo Olvera Lira

# Introducción

En esta actividad se realizó la instalación, configuración y verificación de las herramientas necesarias para trabajar con automatización de infraestructura digital. Actualmente, las organizaciones utilizan tecnologías de contenedores para facilitar el despliegue de aplicaciones y la administración de servicios, por lo que es importante conocer herramientas modernas que permitan automatizar procesos y optimizar recursos.

Durante la práctica se instalaron herramientas fundamentales como Docker Engine, Docker Compose, Git y Visual Studio Code. Estas herramientas permiten desarrollar, administrar y desplegar aplicaciones de forma más eficiente mediante el uso de contenedores y control de versiones. Además, se realizaron pruebas para comprobar el correcto funcionamiento de cada herramienta, verificando la instalación mediante comandos específicos y ejecutando aplicaciones de prueba.

También se utilizó un archivo YAML para desplegar contenedores con Docker Compose y se comprobó el funcionamiento de una API desarrollada con NestJS y MongoDB. Estas actividades permitieron comprender el funcionamiento de los contenedores, la comunicación entre servicios y la administración de aplicaciones modernas.

El propósito de este reporte es documentar el procedimiento realizado, presentar evidencias de funcionamiento y demostrar que el entorno de desarrollo quedó correctamente configurado para continuar con futuras prácticas relacionadas con automatización de redes e infraestructura digital.

# Desarrollo

## Herramientas utilizadas para automatización

### Docker Engine

Docker Engine es una plataforma que permite crear, ejecutar y administrar contenedores. Facilita la implementación de aplicaciones en entornos aislados y portables.

### Docker Compose

Docker Compose permite definir y administrar múltiples contenedores mediante un archivo YAML. Con esta herramienta es posible iniciar varios servicios utilizando un solo comando.

### Docker Swagger

Swagger es una herramienta utilizada para documentar y probar APIs. Permite visualizar los servicios disponibles y realizar pruebas desde una interfaz gráfica.

### Git

Git es un sistema de control de versiones que permite registrar cambios en los proyectos y mantener un historial de modificaciones.

### Visual Studio Code

Visual Studio Code es un editor de código que facilita el desarrollo de aplicaciones mediante extensiones y herramientas de programación.

# Procedimiento de instalación

## Instalación de Visual Studio Code

Se utilizó Visual Studio Code como entorno de desarrollo para editar archivos de configuración, código fuente y archivos Docker.

## Instalación de Docker

Se instaló Docker Engine para la administración de contenedores.

Verificación:

```bash
docker --version
```

Resultado obtenido:

```text
Docker version 28.1.1
```

## Instalación de Docker Compose

Verificación:

```bash
docker compose version
```

Resultado obtenido:

```text
Docker Compose version v2.35.1
```

## Instalación de Git

Verificación:

```bash
git --version
```

Resultado obtenido:

```text
git version 2.25.1
```

# Evidencia de pruebas de funcionamiento

## Prueba Docker Hello World

Comando ejecutado:

```bash
docker run hello-world
```

Resultado:

La imagen fue descargada correctamente desde Docker Hub y mostró el mensaje "Hello from Docker!", confirmando el correcto funcionamiento de Docker.

## Ejecución de archivo YAML

Comando ejecutado:

```bash
docker compose -f stack-srol.yml up -d --build
```

Resultado:

Se construyeron e iniciaron correctamente los contenedores:

* mysql-db
* phpmyadmin
* sistema-ventas-back
* sistema-ventas-front

## Verificación de contenedores

Comando ejecutado:

```bash
docker ps
```

Resultado:

Los contenedores permanecieron en estado activo y disponibles para su utilización.

## Verificación de API Pokémon

Se verificó el funcionamiento de una API desarrollada con NestJS y MongoDB mediante la consulta:

```text
http://localhost:3000/api/v2/pokemon/pikachu
```

Resultado:

La API respondió correctamente mostrando la información almacenada del Pokémon Pikachu.

# Lista de verificación

| Elemento                     | Estado |
| ---------------------------- | ------ |
| Docker instalado             | ✔      |
| Docker Compose instalado     | ✔      |
| Git instalado                | ✔      |
| Visual Studio Code instalado | ✔      |
| Hello World ejecutado        | ✔      |
| Archivo YAML ejecutado       | ✔      |
| Contenedores activos         | ✔      |
| API Pokémon funcionando      | ✔      |

# Conclusión

Yo, Samuel Reynaldo Olvera Lira, concluyo que la instalación y configuración de las herramientas utilizadas para automatización de infraestructura digital se realizó exitosamente. Durante la práctica fue posible instalar Docker Engine, Docker Compose, Git y Visual Studio Code, herramientas fundamentales para el desarrollo moderno basado en contenedores.

Las pruebas realizadas permitieron comprobar el correcto funcionamiento del entorno de trabajo. La ejecución de la imagen Hello World confirmó que Docker se encontraba instalado correctamente, mientras que Docker Compose permitió desplegar múltiples contenedores utilizando un archivo YAML. Asimismo, se verificó el funcionamiento de servicios como MySQL, PhpMyAdmin, aplicaciones frontend y backend.

También se logró validar el funcionamiento de una API desarrollada con NestJS y MongoDB, demostrando la correcta comunicación entre servicios y la capacidad de administrar aplicaciones mediante contenedores. Gracias a estas actividades se adquirieron conocimientos sobre automatización, despliegue de aplicaciones y administración de infraestructura utilizando tecnologías actuales ampliamente utilizadas en la industria.

# Bibliografía

Docker Inc. (2025). Docker Documentation. https://docs.docker.com/

Git Project. (2025). Git Documentation. https://git-scm.com/doc

Microsoft. (2025). Visual Studio Code Documentation. https://code.visualstudio.com/docs

Swagger. (2025). Swagger Documentation. https://swagger.io/docs/

Menzain, E. (2025). Automatización de Redes. GitHub. https://github.com/edomenzain/automatizacion-redes

