# Laboratorio-2-cvds
## La herramienta Maven
1. Cuál es su mayor utilidad:
	1. facilita el proceso de creacion de proyectos con ayuda de los arquetipos.
	2. maven permite: cambiar logs creados directamente de controls de la fuente, referencia cruzada de fuentes, dependencias usadas por el proyecto, reportes de test de unidad que inlcuye coberutra.
	3. provee guias para las mejores practicas de desarrollo.

2. Fases de maven:
	1. Install.
	2. Run
	3. Configure.
	4. Ide integration.
3. Ciclo de vida de la construcción:
	1. Validate: se encarga de validar que el proyecto dispone de toda la informaicon necesaria para ser procesado.
	2. compile: compilar los ficheros fuentes .java y generar en las carpetas de destino los compiladores.
	3. Test: una vez compilado el codigo se ejecutan las pruebas unitarias que se han contruido para el.
	4. package: se encarga de empaquetar nuestro codigo a un formato standart de java que permita ejecucion o despliege en servidor.
	5. verify: se encarga de lanzar los test d eintegracion para confirmar que todo funciona correctamente y qu ela calidad esta bien.
	6. install: desplegar el artefacto en el repositorio local con su verisonado de tal forma que otros artefacto spueden hacer uso de el.
	7. deploy: cuando dispinemos de un aserie de artefactos que desamos compartir entre desarrollos ya que permite desplegar el artefacto en un servidor remoto de tal forma que otros desarrolladores puedan utilizarlo.

4. Para qué sirven los plugins:
	1. los pluggins tienen metas, que segun tecnico son solo metodos java. estas metas ejecutan tareas de contruccion como compilar el proyecto, empaquetarlo e implementarlo en un servidor local o remoto. y estas actividades se correlacionan para contruir fases del ciclo de vida.
5. Qué es y para qué sirve el repositorio central de maven:
	1. El repositorio central de Maven es la ubicación predeterminada para que Maven descargue todas las bibliotecas de dependencia del proyecto para su uso. Para cualquier biblioteca involucrada en el proyecto, Maven primero busca en la carpeta.







#### Referencias:
1. https://www.arquitecturajava.com/que-es-un-maven-lifecycle-y-como-funciona/
2. https://maven.apache.org/what-is-maven.html
3. https://developer.ibm.com/es/articles/j-5things16/
4. https://geekflare.com/es/apache-maven-for-beginners/
