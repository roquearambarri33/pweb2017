# Instrucciones para añadir tu nombre al listado de estudiantes

En la página [Listado de estudiantes 2017-2018](estudiantes1718.md) recogeremos un listado de todos los estudiantes que formáis parte de la clase de **Proyectos para la web** durante este curso 2017-2018, ordenados por grupos y por orden alfabético de apellidos. Seréis vosotros mismos quienes añadáis vuestro nombre (y enlace) a la lista, siguiendo el proceso de contribución que hemos aprendido en el [tutorial introductorio de GitHub](https://services.github.com/on-demand/intro-to-github/es/). Aquí tenéis una descripción paso a paso de cómo hacerlo:

1. Haz un fork de este repositorio en tu cuenta personal. Un fork es una copia exacta del repositorio sobre la que puedes trabajar sin interferir con el repositorio original:
    - Haz clic en el botón **Fork** arriba a la derecha, debajo de tu foto de perfil
    - Selecciona tu foto de perfil para crear el fork en tu cuenta personal, y no en la _organización_ DeustoPWEB
    - Ahora ya tienes un repositorio `pweb2017` en tu cuenta personal

A partir de aquí, puedes trabajar a través de la interfaz web (como hiciste en el tutorial 101) o en tu escritorio a través de GitHub Desktop (como hiciste en el tutorial 102). No voy a entrar en detalles de cómo hacer eso, porque depende de qué elijas. Si tienes problemas, [crea un issue](https://github.com/DeustoPWEB/pweb2017/issues) en el repositorio de la asignatura.

2. Accede a tu fork y crea un nuevo branch con el nombre TU-USUARIO
3. En el branch TU-USUARIO de tu fork, edita el archivo `estudiantes1718.md`:
    - Bajo el nombre de tu grupo, añade en formato de lista tu nombre y apellidos (`Apellido1 Apellido2, Nombre`) y el enlace a la página web personal que has creado a través del tutorial [GitHub 102: GitHub Pages from GitHub Desktop](https://services.github.com/on-demand/github-desktop/)
    - Si no has terminado el tutorial, añade solo tu nombre de momento, y podrás volver para añadir tu link cuando hayas terminado

A partir de aquí trabaja con la interfaz web.

4. Vuelve al repositorio original para [crear un pull request](https://github.com/DeustoPWEB/pweb2017/pulls):
    - Haz clic en **New pull request**, y luego en el link _compare across forks_ debajo del título _Compare changes_ 
    - Asegúrate de que:
        - `base fork`: `DeustoPWEB/pweb2017` 
        - `base`: `master`
        - `head fork`: `TU-USUARIO/pweb2017`
        - `compare`: `TU-USUARIO`
    - Escribe un mensaje que describa tu modificación (añadir tu nombre al listado) y haz clic en **Create pull request**
5. Si hay algún problema con tu modificación, escribiré un mensaje en tu pull request con las indicaciones necesarias para que puedas corregirlo. Tendrás que volver a tu fork y hacer los cambios necesarios
6. Cuando todo esté bien, combinaré (merge) tu branch con el branch `master` del repositorio de la asignatura y podrás ver tu nombre en el [Listado de estudiantes 2017-2018](estudiantes1718.md)
