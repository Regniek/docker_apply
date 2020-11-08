# Esto es Docker
Hola, en este espacio compartire mis apuntes en docker para que podamos ir avanznado juntos

## "Docker te permite construir, distribuir y ejecutar cualquier aplicación en cualquier lado"

## que es Docker
Es un sistema de contenedores que nos permite evitar el uso de una maquina virtual y utilizar un espacio estandarizado para contruir, distribuir y ejecutar muchos mas rapido.

### para Construir entrega:

+ entorno de desarrollo
+ dependencias
+ entorno de ejecucion
+ equivalencia con entorno productivo
+ servicios externos

### para Distribuir:

+ divergencia dee repositorios
+ divergencia de artefactos
+ versionado

### para ejecutar:

+ compatibilidad con entorno productivo
+ dependencias
+ disponibilidad de servicios externos
+ recursos de hardware

## Virtualización

Permite atacar en simultaneo los tres problemas del desarrollo de software profesional.

## Contenedores (Alternativa a maquinas virtuales)

El empleo de contenedores para construir y desplegar software entrega servicios:

+ flecibles
+ livianos
+ portables
+ bajo acoplamiento
+ escalables
+ seguros

Los contenedores se pueden configurar de tal forma que pueden tener limites en cuanto a lso recurso necesarios, recursos como memoeria ram, disco duro y demas.

## Comandos Basicos de Docker

en la terminal colocaremos el siguiente comando:
```
docker --version
```

eso nos dejara visualizar si ya tenemos docker instalado o no, en dado caso que aun no lo tengas instalado dirigete a la [pagina de docker](https://www.docker.com/) y en la sección de descargas lo conseguiras, su instalación es super sencilla.


ahora que lograste tener el docker ya instalado veremos los siguientes comandos:

```
docker run hello-world
```
este comando traera un contenedor ya estandar de Docker que es conocido como hello-world, al no encontrarlo en tu sistema se tomara un tiempo para buscarlo en la base de docker y mostrartelo.


```
docker ps
```
este comando permite verificar cuales contenedores estan corriendo y se encuentrar operando por eso es muy normal que no encuentre hello-world ya que lo trae pero lo trae apagado.

```
docker ps -a
```
con el -a te van a mostrar todos los comando incluso los que no se estan operando, te puedes dar cuenta por que en su STATUS sale la plabra exited()


```
docker run --name hello-guys hello-word
```
esta instrución nos traera de nuevo un contenedor hello-world pero ahora con un nombre propio puesto por nostros, esto con el fin de de poder hacer un manejo de contenedores mas facil, otra cosa que debemos tener en cuenta es que docker no nos va permitir crear dos contenedores con el mismo nombre.

```
docker rm hello-guys
```

ahora lo que estamos realizando es borrando el contenedor con ese nombre especifico, ya que si no lo vamos a utilizar es bueno tener nuestro espacio de docker limpio solo con lo necesario para nuestro desarrollo.

```
docker container prune
```

tambien tenemos este comando que permite eliminar todos los contenedores que no esta en proceso, o se encuentran apagados(exited()), esta instrucción los eliminara todos.


### PostData:

no olvides pasar por [Regniek.dev](http://www.regniek.dev), y recuerda cualquier feedback es amor y lo recibire con gusto, gracias por leerme.