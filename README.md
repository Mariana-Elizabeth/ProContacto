# ProContacto
##Evaluación Práctica
### Ejercicio 2
1.	¿Qué es un servidor HTTP?

•	Tiene muchas partes encargadas del control sobre cómo tienen acceso los usuarios a los archivos. 

•	Un servidor http es una pieza de software que se compredende de URLs (Locación de un recurso en una red de computadoras) y HTPP, que es el protocolo que el navegador utiliza para ver las páginas web.

•	Protocolo que permite enviar documentos de un lado a otro en la web 

2.	¿Qué son los verbos HTTP? Mencionar los más conocidos

•	Se utilizan para indicar la acción que se desea realizar. 

•	Los verbos HTTP le indican al servidor qué hacer con los datos identificados por la URL

Algunos de los más conocidos son:

•	Get. Solicita una representación de un recurso especifico. Solo deben recuperar datos. Solo sirve para obtener el modelo de un recurso, no cambia nada en el servidor. 

•	Post. Envía una entidad a un recurso en específico. Creación de recursos en el servidor. El cliente le envía un pedido al servidor, para crear un recurso. 

•	Put. Para crear y remplazar recursos. A diferencia de post es que este en idempotente (cuando hacermos una llamada put podemos repetirla muchas veces y el efecto en el servidor siempre será el mismo).

•	Delete. Usado para eliminar recursos identificado por la URL de la solicitud.

•	Patch. Modificaciones parciales a recursos. A diferencia de PUT, es que PUT es un remplazo total de un objeto, y con PATCH cambiamos solo algunos atributos.

3.	 ¿Qué es un request y un response en una comunicación HTTP? ¿Qué son
los headers?

•	El cliente envía una petición (request) al servidor, este ejecuta y devuelve en formato html una respuesta (response). 

•	Las cabeceras http permiten al cliente y al servidor enviar información adicional junto a una petición o respuesta. 

4.	¿Qué es un queryString? (En el contexto de una url)

•	Una vez que analizamos un objeto que viene de una URL, queryString  va ser un módulo que nos va a permitir proporcionar el manejo óptimo de esos objetos de URL para convertirlos a consultas de cadenas de texto.

•	Conjunto de valores que le podemos pasar a nuestro servidor web utilizando la URL de una página.

•	Es la parte de una URL que contiene los datos que deben pasar a las aplicaciones web.

5.	¿Qué es el responseCode? ¿Qué significado tiene los posibles valores
devueltos?

•	Estos indican si se ha completado satisfactoriamente una solicitud de HTTP especifica. El servidor recibe y procesa la solicitus, y luego devuelve los recursos relevantes junto con un encabezado HTTP.

•	Se agrupan en 5 clases:

   o	Respuestas informativas (100-199). Indican que la solicitud iniciada por el navegador continúa
    
   o	Respuestas satisfactorias (200-299). Cuando la solicitud del navegador fue recibida, entendida y procesada por el servidor. 
    
   o	Redirecciones (300-399). Cuando un nuevo recurso ha sido sustituido por el recurso solicitado.
    
   o	Errores de los clientes (400-499). Códigos de error del cliente que indican que hubo un problema con la solicitud.
    
   o	Errores de los servidores (500-599). Códigos de error del servidor que indican que la solicitud fue aceptada, pero que un error en el servidor impidió que se compliera.

6.	¿Cómo se envía data en un Get y cómo en un POST?


7.	¿Qué verbo http utiliza el navegador cuando accedemos a una página?

•	Get

8.	Explicar brevemente qué son las estructuras de datos JSON y XML dando
ejemplo de estructuras posibles. 

•	JSON 

  o	Es un formato basado en texto estándar para representar datos estructurados en la sintaxis de objetos de JavaScript. Comúnmente utilizado para transmitir datos en aplicaciones web. Son útiles cuando se quiere transmitir datos a través de una red. 

  o	Está constituido por una colección de pares de nombre y valor o por una lista ordenaad de valores. Cada elemento u objeto comienza por una llave y termina con otra. Cada nombre está seguido de dos puntos y los elementos que están en la misma rama del árbol están separadaos por coma.
  
  o Ejemplo:  
  ![JSON](https://user-images.githubusercontent.com/84425580/118745657-3e5fe880-b81c-11eb-92b3-83e8bedd6a26.PNG)

•	XML 

  o	Uno de los formatos más utilizados para el intercambio de información entre sistemas. Está basado en texto para representar información estructurada: datos, documentos, configuración, etc…

  o	Para diseñar lenguajes de marcado, que permite definir etiquetas personalizadas para descripción y organización de datos. Representa información estructurada en la web, de modo que esta información puede ser almacenada, transmitida, procesada, visualizada e impresa, por diversos tipos de aplicaciones y dipositivos.

  o   Ejemplos:
  
  ![XML1](https://user-images.githubusercontent.com/84425580/118745698-5cc5e400-b81c-11eb-8755-85d97d64df94.PNG)
  
  ![XML2](https://user-images.githubusercontent.com/84425580/118745789-98f94480-b81c-11eb-8123-42251a1fe06a.jpg)


9.	Explicar brevemente el estándar SOAP

•	Se enfoca en acceder a operaciones con nombre, cada operación implementa alguna lógica de negocios.

•	Construye un protocolo basado en XML sobre HTTP o, a veces TCP/IP.

•	Se necesita de un URL de servicio web y puede llamar a sus funciones sin la necesidad de un código en específico.

•	Es un sucesor de XML-RPC, es muy similar, pero describe una forma estándar de comunicación.


10.	Explicar brevemente el estándar REST Full

•	“Transferencia de representación de estado”. Considerada una técnica de arquitectura de software, es decir, un conjunto de principios y patrones de comunicación que ayudan a crear una forma de pensar y construir APIs.

•	Servicio que funciona como un estándar para compartir información, en un sistema de doble vía: Request => Response.

•	Un componente es el “HTTP Status Code”, que le informa al cliente o consumidos del API qué debe hacer con la respuesta recibida.

11.	¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?

•	Los HTTP headers son la parte central de los HTTP requests y responses, y transmiten información acerca del navegador del cliente, de la página solicitada, del servidor.

•	El Content-Tyoe es la propiedad de cabecera usada para indicar el media type del recurso. Este dice al cliente que tipo de contenido será retornado

•	Media type, es una cadena que se envía junto con un archivo que describe el formato del contenido.

### Ejercicio 3
1.	Realizar un request GET a la URL: 
    https://reclutamiento-14cf7.firebaseio.com/personas.json
    ![GET1](https://user-images.githubusercontent.com/84425580/118744918-ccd36a80-b81a-11eb-9875-b0a7de64e2e4.png)

2.	Realizar un request POST a la URL anterior, y con body:
{
“nombre”:“Tu nombre”,
“apellido”:“Tu apellido”,
“dni”:11223322
}
Tip: (Marcar la opción “raw” como body)
![POST](https://user-images.githubusercontent.com/84425580/118745025-0310ea00-b81b-11eb-9cc6-52fc7b8f0ced.png)

3.	Realizar nuevamente un request GET a la URL: 
https://reclutamiento-14cf7.firebaseio.com/personas.json 
![GET2](https://user-images.githubusercontent.com/84425580/118745091-1f148b80-b81b-11eb-93c9-01faa8a7340b.png)

4. ¿Qué diferencias se observan?

Gracias el request POST que se realizó en el punto 2, mi información ya aparece en la base de datos al volver a ejecutar el request GET a la URL señalada.

### Ejercicio 4

Realizar los siguientes módulos de Trailhead:

• Fundamento de la plataforma Salesforce

• Fundamentos de Apex y .NET

• Modelado de datos

• Fundamentos y base de datos de Apex

• Desencadenadores de Apex

Liga de Trailhead: https://trailblazer.me/id/marianaperez




