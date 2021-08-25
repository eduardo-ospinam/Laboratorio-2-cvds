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




## Compilar y Ejecutar:

1. cuál es el objetivo del parámetro "package" y qué otros parámetros se podrían enviar al comando mvn.
	1. package es el comando de empaquetado del proyecto maven. para un proyecto java se ejecuta el paquete y se marca como un paquete jar y para un proyecto web se trata de un paquete war.
	2. otros parametros para mvn son: 
		1. mvn compile: es el comando de compilacion del proyecto maven, los archivos se compilan en archivos de clase y se envian al directorio de destino.
		2. mvn test: comando de prueba del proyecto maven, cmd ejecuta la clase de prueba unitaria en la ubicacion dada.
		3. mvn clean: comando de limpiesa del proyecto maven, elimina el directorio y el contenido en el destino.
		4. mvn install: comando de installacion del proyecto de maven. marcara en un paquete jar o paquete war y lo publicara en el almacen local.

2. cómo ejecutar desde línea de comandos, un proyecto maven y verifique la salida cuando se ejecuta con la clase App.java como parámetro en "mainClass".
	1. se pueden especificar toda la informacion relevante en la configuracion de plugin. dependiendo del caso, tambien se puede especificar alguna o toida la informacion usando propiedades del sistema. en el caso de la linea de comando, con la propiedades del sistema se ejecutaria de la siguiente manera:mvn exec:exec -Dexec.executable="maven" [-Dexec.workingdir="/tmp"] -Dexec.args="-X myproject:dist". 
	2. si se quiere ejecutar u nprograma java en el mismo VM que Maven se puede o modificar del mismo modo, configurando el plugin en el POM. o usando el codigo modificado de: mvn exec:java -Dexec.mainClass="com.example.Main" [-Dexec.args="argument1"] ...




#### Referencias:
1. https://www.arquitecturajava.com/que-es-un-maven-lifecycle-y-como-funciona/
2. https://maven.apache.org/what-is-maven.html
3. https://developer.ibm.com/es/articles/j-5things16/
4. https://geekflare.com/es/apache-maven-for-beginners/
5. https://programmerclick.com/article/81251978045/

