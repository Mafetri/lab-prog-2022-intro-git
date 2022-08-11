Introduccion:
	Semaforos, es un mecanismo de sincronizacion donde un proceso/thread se bloquea si al solicitarlo este no posee permisos disponibles o resta un permiso si es que hay alguno.

Guia de Uso:
	En el caso de Java, se importa:
		- import java.util.concurrent.Semaphore;
	Se crea e inicializa:
		- Semaphore x = new Semaphore(y); siendo x el nombre del semaforo e y la cantidad de permisos a inicializar
	Se utiliza:
		- x.acquire(); de esta forma se solicita un permiso al semaforo. (si no hay alguno entonces el hilo se bloquea).
		- x.release(); de esta forma se libera un permiso del semaforo.
