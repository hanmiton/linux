linux es un kernel
	linus torvalds
Primera version 1991

Pinguino Tux
Niveles de linux
	Usuario
		modo usario 
			shell 
			editores
			compiladores
			programas
		usuario y hardware
			librerias sistema operativo linux
			interaccions con el hardware
Kernel
	componente de E/s
		sistema d earchivos
		protocolo de red
		driver controladore sde disco
	compoente de administracion de la memira
		memoria vitual
		reemplao de paginas de paginacion
		cache de pagians
	component de adminsitracion de los proceso
		manejo de señaes
		creacion teminacion de proceos hilos
Distribucions de linux
	fedora
	centos
	debian
	ubuntu
	redhat
	archlinux
Linea de ocmandos en linxu
	CLI Command Line INterface
	Usuario ->
	Interprete de comandos
		librerais 
		Aplicacones
	Sistema operavico
CLI no es igual a shell emulador de terminal
Shell Interfaz a servicios de os
Emulado rde treminal
	simula una terminal de compudaro

Ejemplos de CLI
	grep
	curl
		interactuar con protocolos
	python
		python -c "print('hola mundo')"
			-c  para pasar un comando
		python -c "print('hola mundo')" >ejemplo.txt
			> para manda a un archiv la salida y eroores
Shell
	Graficos
		gnome
		kde
		xfce
	texto
		bash
		zsh
		bourne shell
shell 
	intrefaz para la comunicacion oxn los servicios dle sistema
emuladore sd eteminales
	teminator
	konsole
	tmux
	iterm
	xterm
	sakura
Usar emulador terminator

VIM tiene cuatro modos de trabajo adicionales en comparación a VI:

- Modo de línea de órdenes
- Modo visual
- Modo selección
- Modo ex

YUM (Yellowdog Updater, Modified) - Fedora / CentOS
Es una herramienta de código abierto desarrollada en Python utilizada para hacer la instalación de paquetes de software en distribuciones que usan RPM (RPM Package Manager) como formato de empaquetamiento, como Red Hat Enterprise Linux, Fedora, CentOS, SuSe y Mandriva.

1. Para instalar un software:

yum install <nombre del paquete>

2. Para desinstalar un software:

yum remove <nombre del paquete>

3. Para actualizar un software:

yum update <nombre del paquete>

4. Para actualizar todo el sistema:

yum update

APT (Advanced Packaging Tool) - Debian, Ubuntu y más derivados de Debian
APT no es en sí un sistema gestor de paquetes directo al usuario sino un conjunto de librerías C++ que utilizan otros programas para la distribución de paquetes de software como apt-get, apt-cache y aptitude. APT se utiliza más que todo para la gestión de software que viene empaquetado en formato deb, utilizada en sistemas Debian y derivados.

Algunos comandos de apt-get y aptitude son:

1. Para instalar un software:
aptitude | apt-get install <nombre del paquete>

2. Para desinstalar un software:
aptitude | apt-get remove <nombre del paquete>

3. Para actualizar un software:

aptitude install <nombre del paquete> | apt-get  --only-upgrade install <nombre del paquete>


4. Para actualizar todo el sistema:

aptitude safe-upgrade | apt-get upgrade

Los sistemas *NIX (También llamados Unix-like o UN*X) son sistemas que se comportan  de forma muy similar al sistema operativo UNIX original de AT&T, el término se puede referir a software con cualquier tipo de licencia: libre o de código abierto, privativo o comercial.

Existen multitud de sistemas *NIX, algunos de los más famosos son GNU/Linux, FreeBSD, Mac OS X, Minix, Solaris. Estos sistemas se rigen por el estándar POSIX (Portable Operating System Interface, la X al final es por UNIX);
A nivel de servidores son muy utilizados los sistemas *NIX como GNU/Linux, FreeBSD, Solaris, incluso UNIX como tal.

1. Ya que no existen recursos reservados si uno de los sitios web alojados en el servidor consume el 100% de los recursos pueden empezar a fallar los demás sitios alojados por la falta de recursos de procesamiento y almacenamiento. La mayoría de los proveedores han desarrollado técnicas para evitar este problema, pero no es 100% efectiva y nos lleva al segundo inconveniente.

2. Si nuestro proveedor de hosting detecta que estamos consumiendo “muchos recursos” nos pueden eliminar la cuenta sin derecho a respaldos ni a devolución del dinero. Un ejemplo claro se puede hacer con los sistemas CMS como WordPress, si se empiezan a recibir muchas visitas concurrentes (es decir, al tiempo) el consumo de recursos obviamente aumenta y el proveedor nos suspende la cuenta, sin importar que el consumo sea con un programa que hasta ellos ofrecen en sus paneles. 

3. Muchos proveedores ofrecen hosting ilimitado en todas sus características por un precio irrisorio, lastimosamente casi siempre es un fraude, ya que si tenemos en cuenta que siempre compartiremos recursos con un “vecino” y que además no hay un servidor con recursos ilimitados, esto nos lleva a pensar que es solo un truco de mercadeo para atraer más clientes, y si al igual que tú, cientos de personas compran el mismo hosting “ilimitado”, por cada nuevo cliente se va haciendo menos “ilimitado”.

4. Otro inconveniente, que a mi parecer es el más grave, es el tema de la seguridad en este tipo de servicios, muchas veces se encuentra software en versiones sin ningún tipo de soporte y la velocidad de actualización a las últimas versiones es muy lenta, provocando que gran parte de los sitios alojados sean vulnerables a algún tipo de ataque. En la práctica muchos de los sitios que son “hackeados” están alojados en hosting compartidos.

Alternativas al hosting compartido

 VPS (Virtual Private Server) en donde tienes una cuota clara y definida de recursos. Un servidor virtual es muy similar a un servidor físico, con la diferencia de que acá hay ciertas restricciones de cuota del CPU

 Algunos proveedores de CLOUD como AWS (Amazon Web Services) manejan eso como ECU (EC2 Compute Uni) con otro tipo de cálculo de procesamiento, en ese caso 1 ECU es aproximadamente 1-1.5 Ghz de un procesador físico, pero sigue el mismo principio de restricción o de reserva de recursos físicos. Si deseas tener todo un servidor  te recomendamos VPS, servidores dedicados o servidores cloud.

 articulo de servidores
 	https://platzi.com/clases/linux/concepto/intro-linux/por-que-no-comprar-quothosting-compartidoquot/material/

 DNS

	git

DNS
	la ip nos identifica en internet
	0-255 son 4 numeros

	dig
		consulta dns a cualqueir dominio
		dig mejorando.la
	ns 
		name server
	dig mejorando.la ns

ping vac.io
ttl tiempo de vida
	60 segundos para ver el cambio cuando cambia la ip
subdominios
	tipo A simpere va apuntar a una ipx
 CNAME
 	es un alias
 MX
 	especifica hacia donde va ir el correo
 dig mejorando.la MX
 	tiene un prioridad
 		mientras el nuemro sea mas bajo
 	TXT
 		configurar texto plano que soporta los dominiso
 		para evitar el spam en los correos
Permisos en sistemas linux
	dar o restringir permiso
		propios
		grupo
		personas exterior
archivo o fichero
	-archivo
	d directorio
	----
	1ro permiso de usuairo
	2do permiso de gupro
	3ro permiso de otros

	cd : change directory
	r : 4
	w: 2
	ejecucion :1
	chmod usuiaorguprootros

Sistema de archivos (/)
	bin
		donde se encuentra todos los archovs compilados y baniros y las app q se queiran ejecutar
		comando del sistema
	boot
		es toda la informacion para el arranque del sistema
		mvr y kernel que se esta arrancando
	dev
		todo lo qeu tenga que ver con memoiras externas
		dispositivos
		null hueco negro(todo se pierde)
		zero (para formatear una unidad la llena de cero a bajo nivel)
	etc
		archivos de configuracin del sistema
	home
		toda la informacion dle usuario
	lib32
	lib64
		tienen todas las librerais 
		de terceros
	media
		todos dispositivos extrenos extraibles
	mnt
		punto de montaje temporal
		por ejemplo backup disco duro
	opt
		archivos de terceros que esta staticamete ocmpilados
	proc
		sistema virtual dinamico y algunas cosas con el kernel
		sistema de archo temporal
		siempre esta modifcando la informacon
		ver memoria disco duro
		ver proceoss
	root
		solo tiene archvos 
	sbin
		intreface de red
		configuracion trajetas de red
	sys
		ventilador
		cosas q interactura directament con el kernel
	usr
		donde estan todos los programs que nosotros tenemos
	var
		carpeta variable todos los archvos variables se ubican 
		correos
		logs
		como se comparte el sistrema
		informacion basic adel navegador
		www
		cache
		backupps

alt+f2 para abrir un comando
	manjador de vnetanas
		permite administrar cda uan de las ventas de consolas

promt
	donde se puedeningresas comandos
~ comodin indica el home del usuario
ubunut 
	empezar con ese sistema de distribucion de linux
ufi
	istalacion mas facil
todo usuairo tiene un home
_ es para hacer un escape
	por lo q si se necesita un espaico se lo hace con _

archivos q empiezand con . son archivos ocultos
	.ocultos par ahcer configuracones del sistema
	-r borra directrrios y todo los que estan dentro de ellos
editores de texto por la terminal
	no usar editores de texto para traer y despues mandar el archiovo al servidor
ver vimtutor
	i es ppara insertar 
	esc sale modod de insercion
	:wq escribir y salir
herrmientas de solo lectura
	cat permite ver ocnteido archivo y lo direcciona sober la terminal
less permite bajar y subir en el archivo
