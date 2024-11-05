- * Un script de Bash es un fichero de texto con una secuencia de comandos de shell.
  Características
  • Deben empezar con #!, indicando la ruta al ejecutable de la shell. Esta línea es un comentario
  especial que permite ejecutar un script como un ejecutable binario más:
  #!/bin/bash
  Idealmente hay que añadir comentarios.
  Con exit se indica cuando se termina el script.
  Los scripts pueden ser considerados ejecutables. Para invocarlos en la línea
  de comandos como si fueran un archivo compilado más hay que habilitar el
  flag ejecutable de archivo: chmod +x script.sh
- ### Scripts especiales
- La shell ejecuta ciertos scripts durante el arranque. Concretamente, intentará leer los ficheros en este
  orden:
  • /etc/profile. Se ejecuta durante el inicio de sesión.
  • ~/.bash_profile, o bien ~/.bash_login, o bien ~/ profile, el primero que encuentre. Se
  ejecuta durante el inicio de sesión.
  • ~/.bashrc. Se ejecuta en una shell sin inicio de sesión.
  Estos scripts suelen contener opciones de configuración de las sesiones de usuario: definición de
  alias, el texto del prompt (el texto que se muestra en cada nueva línea antes
  de los comandos que introduce el usuario) y cualquier otra personalización
  que cada usuario quiera tener disponible.