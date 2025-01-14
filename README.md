# Acortador de Links [![Netlify Status](https://api.netlify.com/api/v1/badges/2a89b1b0-54bc-4a97-9d36-1355b7df4502/deploy-status)](https://app.netlify.com/sites/boisterous-entremet-341979/deploys)

En Tiempo y Espacio se hace uso de esta herramienta para proveer a nuestros clientes de enlaces cortos y accesibles que permiten llegar con más facilidad a nuestra página, redes, ofertas y otras páginas de utilidad, los vinculos cortos nos permiten cumplir con esta tarea de forma rápida y sencilla que el usuario puede emplear con gran facilidad.

Para esto contamos con el dominio https://tye.ar que funciona como acortador de vínculos. Por defecto redirige el tráfico a nuestra [página web][TiempoYEspacio] sin embargo a través de este repositorio es posible agregar nuevos enlaces de acceso rápido, en muy poco tiempo.

## Instalación

Para instalar este repositorio y poder agregar nuevos enlaces, deberás seguir los siguientes pasos:

### 0. Preparación

Antes de comenzar necesitarás tener [Git](https://git-scm.com/downloads) y [Node.js](https://nodejs.org/es/) instalados. Se sugiere que a la hora de instalar Git en Windows, el comando `git` esté disponible desde la terminal Cmd.

Para saber si Git y Node.js están correctamente instalados se pueden usar los siguientes comandos:

```sh
git --version
node --version
```

Una vez instalados, deberás [configurar las llaves SSH](https://docs.github.com/es/free-pro-team@latest/github/authenticating-to-github/connecting-to-github-with-ssh) para poder pushear el código a GitHub, usando Git. Este proceso es complejo así que deberás seguir los tutoriales del enlace.

### 1. Clonar

El primer paso de la instalación será clonar el repositorio.

**Es importante que lo clones, y no lo descargues.**

Al momento de clonar, se creará una carpeta con el nombre del repositorio, en el directorio actual. El comando a usar es el siguiente:

```sh
git clone git@github.com:Tiempoyespacio/tye.ar.git
```

### 2. Instalar Paquetes

Una vez clonado el repositorio ingresamos a la carpeta:

```sh
cd tye.ar
```

Y una vez allí deberemos instalar los paquetes usando NPM:

```sh
npm install
```

Con esto nuestro repositorio se encontrará instalado correctamente.

### 3. Link

El siguiente comando, crea un ejecutable `tye` que estará disponible en cualquier directorio. Este paso es opcional pero recomendado.

```sh
npm link
```

## Uso

### Si seguiste el paso 3

Si has seguido el [paso 3](#3__link) podrás correr el siguiente comando en cualquier terminal:

```sh
tye [link] [name]
```

Esto acortará el `link` a `https://tye.ar/name`

### Si NO seguiste el paso 3

Para usar el comando deberás abrir una terminal en la carpeta del proyecto y correr el siguiente comando:

```
npm run shorten [link] [name]
```

Esto acortará el `link` a `https://tye.ar/name`

## Licencia

Este proyecto es una instancia de [Netlify Shortener](https://github.com/kentcdodds/netlify-shortener) por lo que la licencia de este proyecto es MIT, y el Copyright es de [Kent C. Dodds](https://github.com/kentcdodds)

[TiempoYEspacio]: https://tiempoyespacio.com.ar/
