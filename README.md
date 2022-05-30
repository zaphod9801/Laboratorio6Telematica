# Laboratorio6Telematica

Como prerequisito para este laboratorio ir al siguiente repositorio y seguir sus pasos: 

## Parte 1

Lo primero es que deberemos entrar a la consola de pyspark, para esto basta con escribir pyspark en la terminal:
![image](https://user-images.githubusercontent.com/71454879/170909081-ed90b890-ae15-4e31-b774-e8eb02f0dda4.png)

A continuación se muestra como sería el codigo en Python para realizar un WordCount en un dataset dado en el hdfs, en este caso el correspondiente a gutenberg-small, es importante destacar que en el primer comando debemos estar seguros de la ruta en la que esté ubicado nuestro datasets en el hdfs:
![image](https://user-images.githubusercontent.com/71454879/170909448-b1d90c73-af12-4a96-90ba-a6b562c5e5d4.png)
Salida del programa:
![image](https://user-images.githubusercontent.com/71454879/170909478-de7564fa-2069-4ed5-a51f-dc18c46d0002.png)

Ahora, para el S3, se puede hacer también desde el nodo maestro del cluster EMR y con el mismo programa, basta con cambiar la ruta a la correspondiente en el S3:
![image](https://user-images.githubusercontent.com/71454879/170910306-52089680-5d90-4ebf-b323-e5fbaa99a6d7.png)
Salida del programa:
![image](https://user-images.githubusercontent.com/71454879/170910349-01bf3896-6a12-4dc0-af93-084d6b5bbf97.png)

Posteriormente, para JupyterHub, lo primero será ingresar mediante el enlace que nos provee el cluster EMR en el apartado de "Application user interfaces":
![image](https://user-images.githubusercontent.com/71454879/170916586-31bf7e65-7824-405d-828b-af592add77a0.png)
Después de logearnos, creamos un nuevo cuaderno de tipo PySpark; aqui irá el mismo codigo que usamos para el S3:
![image](https://user-images.githubusercontent.com/71454879/170917396-2fb6c23a-d761-4bd2-8f4d-a40f303ecaeb.png)
El codigo a continuación:
![image](https://user-images.githubusercontent.com/71454879/170911107-96418c4b-e193-4948-a5d7-8b49dd9bf99f.png)

## Parte 2

Para esta parte, se descargará el archivo dado por el profesor y lo importaremos en nuestro propio JupyterHub:
![image](https://user-images.githubusercontent.com/71454879/170911563-d2c8bb21-cdae-4f3a-b772-f25573827664.png)

Al abrirlo veremos lo siguiente, es importante para que funcione correctamente cambiar el kernel de Python 3 a PySpark:
![image](https://user-images.githubusercontent.com/71454879/170911635-01f753f7-6ad0-4b95-abb8-2cb768a99bb7.png)

Este archivo obtiene un dataset dado, en este caso sample_data.csv, y le realiza varias operaciones tales como obtener sus columnas, sus tipos de datos, seleccionar columnas en especifico para ser mostradas, agregar columnas nuevas usando otra columna como base con modificaciones, realizar diferentes filtros para obtener datos, ordenamiento y agrupamiento; entre otras.
![image](https://user-images.githubusercontent.com/71454879/170913440-d2182aed-fcb4-4615-87da-6c7b02a25c39.png)
![image](https://user-images.githubusercontent.com/71454879/170913455-1f69b1ad-2a3f-48d5-a569-ef2d618890fd.png)
![image](https://user-images.githubusercontent.com/71454879/170913470-3efd02e6-5513-43f4-8b1a-6d47fbf20739.png)
![image](https://user-images.githubusercontent.com/71454879/170913482-8b5dfe4d-3082-47d0-97f2-b753b3721b5e.png)
![image](https://user-images.githubusercontent.com/71454879/170913505-9acad34a-7357-4b50-90d2-ec74a2a3cc1d.png)
![image](https://user-images.githubusercontent.com/71454879/170913524-463c9d3e-be1d-40bf-a8b0-20de5969feda.png)
![image](https://user-images.githubusercontent.com/71454879/170913555-7d80a087-7b7a-4462-a559-3f4e615218e4.png)
![image](https://user-images.githubusercontent.com/71454879/170913572-f098f621-5b2d-4de6-a15b-c1bbdd6e13d6.png)
