7.


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
