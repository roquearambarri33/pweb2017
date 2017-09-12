% Introducción a GitHub

## Qué es y cómo funciona git

### ¿Qué hay de nuevo?

[Git para usuarios de Dropbox](git-para-usuarios-dropbox.md)

-------

Dropbox | git
--------|-----
guarda versiones de archivos | guarda versiones del proyecto completo
gestión de conflictos | archivos corruptos

--------

Dropbox | git
--------|-----
archivos borrados, máx 30 días (o de pago) | todos los estados del proyecto 

--------

Dropbox | git
--------|-----
todo es automático | partes importantes son manuales

-------

Funcionamiento de Dropbox:

1. Instalas Dropbox
2. Alguien comparte una carpeta contigo
3. Tu ordenador descarga los contenidos de esa carpeta desde _la nube_
4. Haces algunos cambios a un archivo en la carpeta y los guardas
5. Tus cambios se suben inmediatamente a _la nube_ en Dropbox
6. Los cambios se descargan a los ordenadores de los demás inmediatamente

----

En cambio, con Git:

4. Haces algunos cambios a un archivo en la carpeta y los guardas. Los confirmas mediante `commit`
5. Tus cambios se suben <del>inmediatamente a _la nube_ en Dropbox</del> cuando haces `push`
6. Los cambios se descargan a los ordenadores de los demás <del>inmediatamente</del> cuando hacen `pull`

---

Además, cambia el orden y añade algunos pasos:

6, 4, 6, 5

Es decir, haces `pull`, modificas el archivo, lo guardas, haces `commit`, haces `pull`, haces `push`. El proyecto completo con tus cambios incluidos ya está en la nube.

----

Flujo de trabajo revisado para Git (1 de 2):

1. Haces `pull` para descargar una versión actualizada del proyecto
2. Modificas los archivos necesarios, los guardas, y cuando la modificación tiene sentido propio, haces `commit`. Repite este paso tantas veces como sea necesario

---

Flujo de trabajo revisado para Git (2 de 2):

3. Vuelves a hacer `pull` para incorporar los cambios de los demás. En este punto podrías tener que resolver conflictos
4. Haces `push`. El proyecto y su histórico ya está actualizado y en la nube

---

### Diferencias avanzadas

----

#### Viajes en el tiempo

----

Del libro oficial de Git, [Pro Git](https://git-scm.com/book/es/v2/Inicio---Sobre-el-Control-de-Versiones-Fundamentos-de-Git):

>Cada vez que confirmas (`commit`) un cambio, o guardas el estado de tu proyecto en Git, básicamente toma una foto del aspecto de todos tus archivos en ese momento, y guarda una referencia a esa copia instantánea. (...)

---

Del libro oficial de Git, [Pro Git](https://git-scm.com/book/es/v2/Inicio---Sobre-el-Control-de-Versiones-Fundamentos-de-Git):

>(...) Para ser eficiente, si los archivos no se han modificado, Git no almacena el archivo de nuevo, sino un enlace al archivo anterior idéntico que ya tiene almacenado. Git maneja sus datos como una secuencia de copias instantáneas.

----

![Instantáneas](img/snapshots.png)

----

#### Conflictos 

----

Generalmente Git funciona de manera bastante inteligente y sabrá proponer una resolución satisfactoria, salvo que la modificación se haya realizado sobre la misma línea del archivo. 

### Sugerencias para los commits

----

- Cambios pequeños. Haz un commit cada vez que una modificación o serie de modificaciones tenga sentido en sí misma
- Resume con un infinitivo y de manera informativa en qué ha consistido el cambio (ej. "Cambiar mi salario")
- Es mucho más fácil gestionar las modificaciones y los conflictos sobre documentos de **texto plano (como HTML o Markdown)**



## Qué es GitHub

## Crear una cuenta en GitHub