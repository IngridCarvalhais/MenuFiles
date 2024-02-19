# MenuFiles 

## Fundamentos de Sistemas operativos 

## Autores: Isabella Huerta, Raquel Bascones, Ingrid Carvalhais 

### Nuestro menú se basa en 4 opciones:  

*Creamos una función llamada –mostrar_menú()-: 

Dicha función imprimirá el menú con el comando –echo-: 

  echo "Menú de opciones:" 

  echo "1. Crear carpeta y archivos" 

  echo "2. Mover archivos a una carpeta" 

  echo "3. Eliminar archivos o carpetas" 

  echo "4. Salir" 

* Crear carpetas y archivos: 

En primer lugar, utilizamos el comando read –p para pedir al usuario que introduzca el nombre de la carpeta que desea crear y almacena la entrada del usuario en una variable, carpeta. 

Luego, empleamos el comando mkdir “$carpeta” para crear la carpeta con el nombre introducido por el usuario, de tal forma que se creará una carpeta con dicho nombre. 

Después, empleando echo “Carpeta creada: $carpeta” la función muestra un mensaje con el nombre de la carpeta creada. 

A continuación, se vuelve a utilizar el comando read –p , pero en este caso, para solicitar al usuario que ingrese el nombre del primer archivo. El nombre se almacenará en la variable archivo1. Empleamos el comando touch “$carpeta/$archivo1” para crear un archivo dentro de la carpeta recién creada y el cual tendrá el nombre ingresado por el usuario. 

Para la creación del segundo archivo cuyo nombre se almacenará en la variable archivo2 se sigue el mismo procedimiento que para el archivo1, solo que en este caso haciendo uso de la variable archivo2. 

 

* Mover archivos a una carpeta: 

     Usamos el comando read para solicitar al usuario que ingrese la ubicación de la carpeta donde se      encuentra el archivo que desea mover. 

    Echo para imprimir la ubicación. 

    El ls lista los archivos en la carpeta especificada. 

    Nuevamente read para ingresar el nombre del archivo y a que carpeta se desea mover. 

    Finalmente, el comando mv (move) lo utilizamos para mover el archivo desde su origen a la ubicación de  destino y echo para imprimir el archivo movido. 

 

* Eliminar archivos en una carpeta: 

    Usamos el comando read para solicitar al usuario que ingrese la ubicación de la carpeta donde se encuentra el archivo que desea eliminar. 

    Echo para imprimir la ubicación. 

    El ls lista los archivos en la carpeta especificada. 

    Nuevamente read para ingresar el nombre del archivo a eliminar. 

    Finalmente, el comando rm (remove) lo utilizamos para eliminar el archivo y echo para imprimir el archivo eliminado. 

*Bucle para repetir el menú y condicional para ejecutar las diferentes opciones: 

    Creamos un bucle -while ; do- con un booleano, para que las opciones del menú aparezcan por pantalla recurriendo a la funcion –mostrar_menu()-  hasta que no seleccionemos salir de él. 

    Dentro del bucle, usamos los condicionales -if-, -elif- y -else- para ejecute las diferentes opciones del menú, para salir de éste, usando un -break-, o en casa que elijamos una opción incorrecta, que se nos avise por pantalla y vuelva a imprimir el menú, para intentarlo de nuevo. 
