## FS CheckPoint 10

**Contenido:**

1. [¿Qué es Git?](#qué-es-git-para-qué-se-usa-que-beneficios-tiene-para-tí-sería-obligatorio-el-uso)
1. [¿Qué es GitHub?](#qué-es-github-para-qué-se-usa-que-beneficios-tiene-para-tí-sería-obligatorio-el-uso-existen-otras-opciones-en-caso-de-que-sea-afirmativo-porque-utilizarías-github)
1. [¿Qué hace un archivo .gitignore?](#qué-hace-un-archivo-gitignore-para-qué-se-usa-que-beneficios-tiene-para-tí-sería-obligatorio-el-uso)



### ¿Qué es Git? para qué se usa, que beneficios tiene. ¿para tí sería obligatorio el uso?

Git es un programa informático de control de versiones. Git permite guardar el estado de un código de programación en un punto determinado para, en caso de ser necesario, volver al estado y funcionalidad propias de dicha versión. Des de un punto de vista operativo, Git tiene en cuenta los cambios en los ficheros que se van produciendo en vez de guardar una copia completa de cada versión. La evolución principal de la aplicación en desarrollo se salvaguarda en la denominada rama principal. Aun así, Git permite crear ramificaciones de esta rama principal para, por ejemplo, desarrollar una función determinada. 

Técnicamente, Git es un sistema de control de versiones distribuido. Esto implica que el desarrollador crea una copia local del repositorio plenamente funcional y, consecuentemente, no depende únicamente de un repositorio remoto como en los sistemas de control de versiones centralizados. Una vez el desarrollador ha implementado la funcionalidad en su repositorio local, este se sincroniza con el repositorio remoto, des de donde puede ser usado por los demás desarrolladores. 

Para el desarrollador individual, Git permite controlar el avance del código de programación y volver a una versión anterior en caso de necesidad, actuando de “back up”. El programador puede testear derivaciones alternativas del desarrollo y implementarlas al código principal una vez testeadas o probadas. Además, si el desarrollador es suficientemente ordenado y va anotando los cambios que se realizan paulatinamente, el historial de git (“commits” realizados) es un recordatorio, a modo de diario de anotaciones, del proceso de programación. 

Aun así, la fortaleza y beneficios del uso de Git se expresan plenamente cuando es usado por un grupo de desarrollo, donde conocer el historial y evolución del código es de vital importancia para el avance conjunto del equipo. Varios desarrolladores pueden crear y trabajar en ramas alternativas y, una vez verificadas, implementarlas en la principal. Este paso tiene especial relevancia puesto que hay que asegurarse de que no hay conflictos durante la fusión (“merging”) del código que podría surgir si, por ejemplo, dos programadores han cambiado la misma línea de un mismo fichero existente en la versión del código. 

A modo de resumen, el uso de Git no es indispensable, aunque sí muy recomendable para el desarrollador individual, donde la creación de copias completas del código de manera manual sigue siendo posible. Para el desarrollo de aplicaciones de manera colaborativa, aun sin ser estrictamente necesario, podemos considerar que el uso de un sistema de control de versiones es virtualmente necesario puesto que la complejidad del proceso de coordinación y salvaguardado manual aumenta exponencialmente, sobretodo en proyectos grandes. 

### ¿Qué es Github? para qué se usa, que beneficios tiene. ¿para tí sería obligatorio el uso?, ¿existen otras opciones? en caso de que sea afirmativo porque utilizarías github

GitHub es una plataforma donde se pueden almacenar, compartir y desarrollar código junto a otros desarrolladores. Es decir, permite crear los repositorios remotos mencionados anteriormente. GitHub está pensado principalmente para desarrollar código abierto, aunque también se pueden crear repositorios privados, lo cual conlleva un coste asociado. 

El beneficio principal de GitHub es el de poder sacar todo el provecho a Git, especialmente para el desarrollo conjunto de código sin la necesidad de mantener un servidor dedicado, lo cual requiere de conocimientos, hardware dedicado y comporta un coste económico. Centrándonos en el desarrollador individual, además de los beneficios derivado del control de versiones, permite tener una copia del código en la nube. Teniendo esto presente, el uso de GitHub no es imprescindible ni para el usuario individual ni para los equipos de desarrollo, puesto que las funciones de copia de seguridad o hospedaje se pueden realizar mediante otras alternativas servidores privados o almacenamiento en la nube generalista.  

Además de las opciones generalistas, también existen otras opciones de hospedaje de código competidoras de GitHub como Gitlab, Bitbucket o Gitkraken. La elección de la plataforma depende de muchos factores como integración con entornos de desarrollo empresarial, uso de sistemas de control de versiones (diferentes de Git), hábitos o gustos de los desarrolladores. En términos generales, GitHub es gratuito y muy competitivo para el desarrollo de software libre (permite crear tantos repositorios públicos como se desee) que es para lo cual surgió inicialmente. Gitlab es una buena opción para empresas, entre otras características, por la posibilidad que existe de instalar la aplicación directamente en un servidor privado lo cual evita problemas o incompatibilidades derivadas de la gestión de permisos implementada en el servidor (empresarial). Otra opción interesante es Bitbucket. Una de las características distintivas de Bitbucket es que está integrada con el software de gestión de proyectos Jira y tiene un plan de precios muy interesante. A diferencia de GitHub, la versión gratuita de Bitbucket, permite un equipo de hasta 5 desarrolladores y la creación de un número ilimitado de proyectos privados. 

### ¿Qué hace un archivo .gitignore? para qué se usa, que beneficios tiene. ¿para tí sería obligatorio el uso?

El archivo “.gitignore” es un fichero oculto que se alberga en la raíz del repositorio Git local que nos permite filtrar los archivos que salvaguardamos en el repositorio. Por ejemplo, el código siguiente impide la copia (ignora) de los ficheros dentro de la carpeta “carpetaProyecto”, de cualquier fichero que termine en “.txt” y del fichero “test.html”:

```
carpetaProyecto
*.txt
Test.html
```
A pesar de su simplicidad, este archivo es tremendamente útil puesto que evita que copiemos archivos innecesarios (por ejemplo, modules de una aplicación JS que pueden ser instalados con las dependencias del proyecto) o que puedan contener información sensible como ficheros con claves de acceso o información empresarial sensible. 

El uso de “.gitignore” no es imprescindible puesto que se pueden escoger de manera manual los ficheros que incluyen en cada “commit” (confirmación) de Git, aunque esto puede acabar suponiendo una dedicación temporal y complejidad importantes a lo largo del proyecto. 
