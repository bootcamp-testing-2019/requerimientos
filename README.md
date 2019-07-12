# Requerimientos para el taller de testing 2019

### Virtual machine

Una máquina virtual con la imágen Ubuntu 16.04.6 LTS (Xenial Xerus)](http://releases.ubuntu.com/xenial/) instalada

[32-bit PC (i386) desktop image](http://releases.ubuntu.com/xenial/ubuntu-16.04.6-desktop-i386.iso)

### Login

```
user: bootcamp
password: bootcamp
```

## Software

En Ubuntu abrir una `Terminal` de consola e instalar el siguiente software:

### Actualizar la imagen

```
sudo apt update
```

### Instalar [Git](https://git-scm.com/)

Git es un programa para manejar cambios y versionados de archivos en proyectos.

Permite llevar el rastro de los cambios de todos los archivos, que múltiples personas editen
múltiples archivos, incluso los mismos, al mismo tiempo sin bloquearse entre ellos y manejas
de manera clara las versiones de los proyectos.

Es imprescindible en proyectos de más de una persona.

```
sudo apt install -y git
```

### Instalar [nvm](https://github.com/nvm-sh/nvm#installation-and-update)

`NVM` es el `Node.js Version Manager`.

Es un programa que permite instalar múltiples versiones de `Node.js` en una misma máquina y que cada vesión funcione correctamente sin conflictuar unas con otras.

```
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```

Reabrir la terminal de consola y verificar la instalación con

```
nvm --version
```

La consola debería mostrar el número de version de `nvm`.

### Instalar [Node.js](https://nodejs.org/en/)

Con `nvm` ahora se puede instalar la versión más reciente de node:

```
nvm install node
```

Verificar la instalación con

```
node -v
```

Debería mostrar el número de versión de node.


### Instalar [Mysql](https://www.mysql.com/)

Mysql es una base de datos relacional. Se usa para guardar y administrar los datos de las aplicaciones.

Instalar mysql server

```
sudo apt-get update
sudo apt-get install mysql-server
mysql_secure_installation
```

### Instalar [Sublime Text](https://www.sublimetext.com/docs/3/linux_repositories.html#apt)

Instalar el editor de texto Sublime Text

```
https://www.sublimetext.com/docs/3/linux_repositories.html#apt
sudo apt-get install apt-transport-https
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
sudo apt-get update
sudo apt-get install sublime-text
```
