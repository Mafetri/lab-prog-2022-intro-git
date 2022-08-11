7.

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

-------------------------------------------------------------

10.

diff --git a/ejemplos/Main.java b/ejemplos/Main.java
new file mode 100644
index 0000000..ad5d2b6
--- /dev/null
+++ b/ejemplos/Main.java
@@ -0,0 +1,22 @@
+
+
+package TP2.PingPong;
+
+public class Main {
+    public static void main(String[] args) {
+        PingPong t1 = new PingPong("PING", 100);
+        PingPong t2 = new PingPong("PONG", 300);
+
+        // Activación
+        t1.start();
+        t2.start();
+
+        // Espera unos segundos
+        try {
+            Thread.sleep(2);
+        } catch (InterruptedException e) {
+        }
+
+        System.out.println("hola");
+    }
+}
diff --git a/ejemplos/PingPong.java b/ejemplos/PingPong.java
new file mode 100644
index 0000000..3f3456d
--- /dev/null
+++ b/ejemplos/PingPong.java
@@ -0,0 +1,24 @@
diff --git a/ejemplos/Main.java b/ejemplos/Main.java
diff --git a/ejemplos/Main.java b/ejemplos/Main.java
new file mode 100644
index 0000000..ad5d2b6
--- /dev/null
+++ b/ejemplos/Main.java
@@ -0,0 +1,22 @@
+
+
+package TP2.PingPong;
+
+public class Main {
+    public static void main(String[] args) {
+        PingPong t1 = new PingPong("PING", 100);
+        PingPong t2 = new PingPong("PONG", 300);
+
+        // Activación
+        t1.start();
+        t2.start();
+
+        // Espera unos segundos
+        try {
+            Thread.sleep(2);
+        } catch (InterruptedException e) {
+        }
:

------------------------------------------------------
13.

	Hay 5 ramas:
		- master (donde se aloja las versiones finales a publicar con sus respectivos tags de version)
		- release (supongo que es la rama previa a unir los cambios de "develop" con la master)
		- develop: es en la rama donde se van haciendo los cambios
		- feature 1 o 2: son ramas transitorias en las cuales se desarrollan, de manera verde, las features a desarrollar sin tocar la rama de desarrollo, una vez que estas features estan completas se la une a la rama de desarrollo.

