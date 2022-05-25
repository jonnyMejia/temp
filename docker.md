# Docker

## ¿Que es Docker?

Es una herramienta Open-Source que permite realizar una virtualizacion ligera con la que podemos empaquetar aplicaciones y sus dependencias para poder desplegarla en cualquier sistema que tenga esa tecnología.

## Docker vs Maquinas Virtuales

* La gran diferencia esque una maquina virtual necesita contener todo el sistema operativo, mientras que un contenedor Docker aprovecha el sistema host y las librerias necesarias. 
* Una maquina virtual puede ocupar varios gigas dependiendo del sistema operativo, mientras que docker no llega ni a medio giga.
* Docker hacen uso mas eficiente del sistema anfitrion porque solo usan la memoria y capacidad necesaria
* Es más practico y rapido usar docker
* Las instancias se arrancan en pocos segundos
* Es facil de automatizar e implantar en entornos de integracion continua
* Existen multitud de imagenes que pueden descargarse y modificarse libremente 

## Ventajas

### Desarrolladores de aplicaciones

1. Levantamientos de calidad superior
2. Mejor escalabilidad de aplicaciones
3. Mejor aislamiento de aplicaciones

### Arquitectos de TI
1. Escalabilidad horizontal más rápida
2. Ciclos de prueba más corto
3. Menor errores de implementacion

### Operaciones de TI
1. Lanzamientos de calidad superior
2. Sustitucion eficiente de todas las maquinas virtuales en produccion
3. Gestion de aplicaciones mas facil.



## Componentes

* **Imagenes**: Describen los contenidos que tienen el contenedor. (Configuracion Proceso, aplicaciones)
* **Registros**: Las imagenes que se crean, se guardan en registros publicos(docker hub) o privados.
* **Contenedor**: Es la imagen ejecutandose

## Algo que anotar

* Analogía relacionada a POO: La clase es la imagen, y el objeto es el contenedor
* Las imagenes no se ejecutan
* Los contenedores tienen un ciclo de vida
* Las imagenes se pueden copiar entre host, pero el contenedor NO
* Solo se puede crear contenedores de imagenes descargadas en el sistema

## Comandos Principales

* docker pull: Descargar imagenes
* docker push: Subir imagenes
* docker image: Llamar mis imagenes descargadas
* docker ps: Ver los contenedores que estan corriendo, con -a los que ya se ejecutaron y terminaron
* docker start: Para iniciar los contenedores detenidos
* docker stop: Para parar los contenedores 
* docker restar: Para reiniciar el contenedor
* docker exec: Para ejecutar comandos en un contenedor, exponer puertos etc.
* docker attach: Mostrar los inputs outputs errores de un contenedor


## Imagenes

* Es de solo lectura
* Pueden contener una aplicacion, un sistema operativo, etc.

## Redes

* **Bridge**: La red estandar que usan los contenedores
* **host**: El servidor

## Contenedor

* **Puertos**: -p Definir el puerto local y del contenedor
* **Volumenes**: -v Compartir una ruta temporal
* **Variables**: -e POSTGRESS=contraseña

## DOCKERFILE

Es un documento de texto que contiene todos los comandos que un usuario podria llamar en la linea de comandos para ensamblar una imagen. Docker build crea una imagen a partir de un Dockerfile
