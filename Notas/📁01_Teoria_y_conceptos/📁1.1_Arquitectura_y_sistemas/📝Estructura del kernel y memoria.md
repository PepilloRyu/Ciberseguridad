
**Fuente:** [Red Hat - What is the Linux Kernel](https://www.redhat.com/es/topics/linux/what-is-the-linux-kernel)

## ¿Qué es?

Es la parte central del SO. Actúa como un puente entre las aplicaciones del usuario y el hardware (CPU, Memoria, Dispositivos).
## Funciones del kernel

1. Gestión de la memoria
2. Gestión de los procesos
3. Controladores de dispositivos
4. Seguridad y llamadas al sistema 

## Ubicación del kernel 

Tiene 3 capas : 
1. El hardware
2. El kernel de linux
3. Procesos del usuario

El código que se ejecuta funciona en dos modos : 
- El modo kernel 
	Tiene acceso total al hardware. Si un atacante ejecuta código aquí, el sistema está totalmente comprometido.
	
- El modo usuario
	Acceso restringido. Las aplicaciones "piden permiso" al kernel

