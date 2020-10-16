# Práctica de sockets en C

## Hecho por Juan Pablo de Jesus Figueroa Jaramillo y Marco Antonio Prado Garcia


### Estructura

- Cliente.c.

- Makefile.

- Servidor.c.

- Socket_Cliente.c.

- Socket_Cliente.h.

- Socket_Servidor.c.

- Socket_Servidor.h.

- Socket.c.

- Socket.h.




### Como comenzar?

Instrucciones para ejecuciòn del ejemplo servidor/cliente

En los ficheros adjuntos hay un pequeño programa Servidor y un Cliente.
Lo ùnico que hacen es establecer conexi�n entre ellos y pasarse las
cadenas de texto "hola" y "adios". Sirve como ejemplo b�sico de c�mo
conectar servidor y cliente y de como transmitir datos del uno al otro.

Para ejecutar los programas en entorno linux, hay que seguir los 
siguientes pasos:

1. Con permiso de root editar el fichero /etc/services y a�adir una linea,
del mismo estilo de las que ya hay, que ponga:
    
            juanpablo-hack@juanpablohack-NBLK-WAX9X:~$ sudo nano /etc/services


2. En la ultima lìnea agregamos lo siguiente:

            cpp_java    tcp/15557

Siendo 15557 cualquier numero que no exista ya en el fichero y que sea
entre 5000 y 65635.

3. Asegurarse que en el fichero /etc/hosts hay una linea en la que aparece 
el nombre "localhost" y la direccion IP 127.0.0.1. Normalmente asi sera:

4. Copiar todos los ficheros en un directorio de linux.

5. En el directorio donde hemos copiado los ficheros, hacer:

            make

6. Se generara un Servidor y un Cliente,desde una ventana, arrancar el Servidor:

            $ ./Servidor

7. Desde otra terminal arrancamos el Cliente:

            $ ./Cliente

Veremos como cada programa escribe en pantalla la cadena que recibe del
otro.
