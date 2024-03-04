# Proyecto de Examen de la 2ª Evaluación

Este repositorio contiene el código del proyecto de examen para la 2ª evaluación. A continuación se detallan los pasos realizados para realizar la release v1.0 del proyecto.

## Pasos Realizados

### Paso 1: Fork del Proyecto

Antes de comenzar a trabajar en el proyecto, se realizó un fork del repositorio original para poder realizar cambios y contribuir de manera independiente.
Para ello desde github se realizó el fork y se hizo un clonado por terminal.

### Paso 2: Creación del Readme

Se creó una nueva rama llamada `readme` donde se agregó el archivo `Readme.md` para ir registrando los pasos, comandos y justificaciones de las decisiones tomadas durante el proceso de release.
Es el documento que estamos leyendo en este momento.

### Paso 3: Trabajo en las Ramas

Se trabajó en las diferentes ramas del proyecto:
- **main**: Se mantuvieron solo los commits etiquetados a las diferentes releases.
- **datos**: Contiene la clase de conexión a una base de datos.
- **interface**: Encargada de la parte gráfica.

### Paso 4: Revisión y Exclusión de Commit en la Rama Interface

Durante la revisión del código en la rama `interface`, se identificó un commit con código no deseado para la versión final. Se decidió no incluir este commit en la versión v1.0.

### Paso 5: Fusión (Merge)

Se realizó la fusión de todas las ramas en la rama `main`, excluyendo el commit no deseado de la rama `interface`.
Para eso hicimos un revert commit en la rama interface al anterior commit de esta forma el último commit de la rama interface queda registrado
por el caso de que algún momento queramos volver a é pero no queda dentro de nuestro commit, podemos verlo bien en la siguiente
imagen:

![RevertCommit](/home/dam/Escritorio/ExamenCOD/img/Screenshot_20240304_090046.png)


### Paso 6: Etiquetado del Último Commit como v1.0

Una vez finalizada la fusión, se etiquetó el último commit en la rama `main` como v1.0 para marcar la versión final del proyecto.
git commit -m "v 1.0"
git tag -a v1.0 -m "versión finalizada EXAMENCOD"



### Paso 7: Actualización del .gitignore

Se descubrió que el archivo `.gitignore` no estaba incluido en el proyecto y que además estaba incompleto. Se completó el `.gitignore` y se agregó al commit etiquetado como v1.0 para garantizar que los archivos no deseados no se incluyan en futuras versiones.
Por ello vamos a añadir el .gitignore posteriormente.
git add .gitignore
git commit --amend

### Paso 8: Push y Creación de la Release

Con todos los cambios realizados y el proyecto listo para la release v1.0, se realizó el push de los cambios al repositorio remoto y se creó la release correspondiente.

## Repositorio Entregado
