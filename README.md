# ProContacto
## Evaluación Práctica
### Ejercicio 2
**1.	¿Qué es un servidor HTTP?**

•	Tiene muchas partes encargadas del control sobre cómo tienen acceso los usuarios a los archivos. 

•	Un servidor http es una pieza de software que se compredende de URLs (Locación de un recurso en una red de computadoras) y HTPP, que es el protocolo que el navegador utiliza para ver las páginas web.

•	Protocolo que permite enviar documentos de un lado a otro en la web 

**2.	¿Qué son los verbos HTTP? Mencionar los más conocidos**

•	Se utilizan para indicar la acción que se desea realizar. 

•	Los verbos HTTP le indican al servidor qué hacer con los datos identificados por la URL

Algunos de los más conocidos son:

•	Get. Solicita una representación de un recurso especifico. Solo deben recuperar datos. Solo sirve para obtener el modelo de un recurso, no cambia nada en el servidor. 

•	Post. Envía una entidad a un recurso en específico. Creación de recursos en el servidor. El cliente le envía un pedido al servidor, para crear un recurso. 

•	Put. Para crear y remplazar recursos. A diferencia de post es que este en idempotente (cuando hacermos una llamada put podemos repetirla muchas veces y el efecto en el servidor siempre será el mismo).

•	Delete. Usado para eliminar recursos identificado por la URL de la solicitud.

•	Patch. Modificaciones parciales a recursos. A diferencia de PUT, es que PUT es un remplazo total de un objeto, y con PATCH cambiamos solo algunos atributos.

**3.	 ¿Qué es un request y un response en una comunicación HTTP? ¿Qué son
los headers?**

•	El cliente envía una petición (request) al servidor, este ejecuta y devuelve en formato html una respuesta (response). 

•	Las cabeceras http permiten al cliente y al servidor enviar información adicional junto a una petición o respuesta. 

**4.	¿Qué es un queryString? (En el contexto de una url)**

•	Una vez que analizamos un objeto que viene de una URL, queryString  va ser un módulo que nos va a permitir proporcionar el manejo óptimo de esos objetos de URL para convertirlos a consultas de cadenas de texto.

•	Conjunto de valores que le podemos pasar a nuestro servidor web utilizando la URL de una página.

•	Es la parte de una URL que contiene los datos que deben pasar a las aplicaciones web.

**5.	¿Qué es el responseCode? ¿Qué significado tiene los posibles valores
devueltos?**

•	Estos indican si se ha completado satisfactoriamente una solicitud de HTTP especifica. El servidor recibe y procesa la solicitus, y luego devuelve los recursos relevantes junto con un encabezado HTTP.

•	Se agrupan en 5 clases:

   o	**Respuestas informativas (100-199).** Indican que la solicitud iniciada por el navegador continúa
    
   o	**Respuestas satisfactorias (200-299).** Cuando la solicitud del navegador fue recibida, entendida y procesada por el servidor. 
    
   o	**Redirecciones (300-399).** Cuando un nuevo recurso ha sido sustituido por el recurso solicitado.
    
   o	**Errores de los clientes (400-499).** Códigos de error del cliente que indican que hubo un problema con la solicitud.
    
   o	**Errores de los servidores (500-599).** Códigos de error del servidor que indican que la solicitud fue aceptada, pero que un error en el servidor impidió que se compliera.

**6.	¿Cómo se envía data en un Get y cómo en un POST?**


**7.	¿Qué verbo http utiliza el navegador cuando accedemos a una página?**

•	Get

**8.	Explicar brevemente qué son las estructuras de datos JSON y XML dando
ejemplo de estructuras posibles.**

•	**JSON**

   o	Es un formato basado en texto estándar para representar datos estructurados en la sintaxis de objetos de JavaScript. Comúnmente utilizado para transmitir datos en aplicaciones web. Son útiles cuando se quiere transmitir datos a través de una red. 

   o	Está constituido por una colección de pares de nombre y valor o por una lista ordenaad de valores. Cada elemento u objeto comienza por una llave y termina con otra. Cada nombre está seguido de dos puntos y los elementos que están en la misma rama del árbol están separadaos por coma.
  
  o **Ejemplo:**  
  ![JSON](https://user-images.githubusercontent.com/84425580/118745657-3e5fe880-b81c-11eb-92b3-83e8bedd6a26.PNG)

•	**XML**

   o	Uno de los formatos más utilizados para el intercambio de información entre sistemas. Está basado en texto para representar información estructurada: datos, documentos, configuración, etc…

   o	Para diseñar lenguajes de marcado, que permite definir etiquetas personalizadas para descripción y organización de datos. Representa información estructurada en la web, de modo que esta información puede ser almacenada, transmitida, procesada, visualizada e impresa, por diversos tipos de aplicaciones y dipositivos.

  o   **Ejemplos:**
  
  ![XML1](https://user-images.githubusercontent.com/84425580/118745698-5cc5e400-b81c-11eb-8755-85d97d64df94.PNG)
  
  ![XML2](https://user-images.githubusercontent.com/84425580/118745789-98f94480-b81c-11eb-8123-42251a1fe06a.jpg)


**9.	Explicar brevemente el estándar SOAP**

•	Se enfoca en acceder a operaciones con nombre, cada operación implementa alguna lógica de negocios.

•	Construye un protocolo basado en XML sobre HTTP o, a veces TCP/IP.

•	Se necesita de un URL de servicio web y puede llamar a sus funciones sin la necesidad de un código en específico.

•	Es un sucesor de XML-RPC, es muy similar, pero describe una forma estándar de comunicación.


**10.	Explicar brevemente el estándar REST Full**

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

### Ejercicio 5

Explicar que son conceptualmente, qué datos almacenan en forma estándar y cómo se
relacionan el resto (algunos no se relacionan entre sí) cada uno de los siguientes objetos de
Salesforce:
**1. Lead.** Prospecto o un cliente potencial

   **Datos que almacena:**

      •	Company

      •	Created By

      •	Las Modified By

      •	Lead Owner

      •	Lead Status

      •	Name

**2. Account.** Cuenta individual, ya sea organización o persona involucrada, como clientes, socios, etc..

   **Datos que almacena:**

      •	Account Name

      •	Account Owner

      •	Created By

      •	Last Modified By

**3. Contact.** Contacto, persona asociada con una cuenta (Account).

   **Datos que almacena:**

      •	Contact Owner

      •	Created By

      •	Last Modified By

**4. Opportunity**. Oportunidad, una venta o un trato pendiente.

   **Datos que almacena:**

      •	Close Date

      •	Created By

      •	Forecast Category

      •	Last Modified By

      •	Opportunity Name

      •	Opportunity Owner

      •	Probability (%)

**5. Product.** Producto que vende la empresa.

   **Datos que almacena:**

      •	Created By

      •	Last Modified By

      •	Product Name


**6. PriceBook**. Lista de precios de los productos que vende la empresa.

   **Datos que almacena:**

      •	Created By

      •	Last Modifier By

      •	Price Book Name

**7. Quote.** Cotización, registro que muestra los presupuestos de los productos y servicios.

      **Datos que almacena:**

      •	

**8.Asset.** Artículo de valor comercial, producto vendido por la empresa o competidor.

   **Datos que almacena:**

      •	Asset Name

      •	Asset Owner

      •	Created By

      •	Has Lifecycle Management

      •	Last Modified By

**9. Case.** Caso, problema o algún problema con un cliente

   **Datos que almacena:**

      •	Busines Hours

      •	Case Number

      •	Case Owner

      •	Created By

      •	Date/Tome Opened

**10. Article.**

   **Datos que almacena:**

   •	
   
**Diagrama UML de relaciones:**

![Relaciones](https://user-images.githubusercontent.com/84425580/119340107-aae14a00-bc57-11eb-9e37-9f0928d20371.png)


### Ejercicio 6

### Ejercicio 7
Responder las siguientes preguntas brevemente sobre:
Soluciones de Salesforce
A.	¿Qué es Salesforce?
Solución de gestión de relaciones con clientes que una une empresas y clientes. Es una plataforma relacionada al conjutno de prácticas, estrategias de negocio y tecnologías enficadas en la relación con el cliente. Esta brinda a todos sus departamentos, una vista única y compartida de cada cliente

B.	¿Qué es Sales Cloud?
Software de ventas. Administra leads (clientes potenciales) monitorea resultados y automatiza procesos de ventas con facilidad. Potencia a los representates de ventas spara generar más negocios y más rápido.

C.	¿Qué es Service Cloud?
Soluciones de software de servicio al cliente. Perimite que los agentes se conectetn con los clientes para ayudarlos a solucionar los problemas de una manera eficaz. Este sostware puede ayudar a las compañías a optimizar los procesos y las llamadas del equipo de atenión al cliente.

D.	¿Qué es Health Cloud?
Softeare el cual proporciona servicios de atención médica, el cual le permite al usuario interactuar más profundamente con su información e historial, a través de cualquier dispositivo.

E.	¿Qué es Marketing Cloud?
Solución de gestión de campañas de marketing, mediante distintas formas, como son redes sociales o mensajes de email
Funcionalidades de Salesforce

A.	¿Qué es un RecordType?
Determinan los procesos de negocio, los formatos de página y los valores de lista de selección a los que los usuarios tienen acceso. 

B.	¿Qué es un ReportType?

C.	¿Qué es un Page Layout?

D.	¿Qué es un Compact Layout?


E.	¿Qué es un Perfil?

F.	¿Qué es un Rol?


G.	¿Qué es un Validation Rule?

H.	¿Qué diferencia hay entre una relación Master Detail y Lookup?


I.	¿Qué es un Sandbox?

J.	¿Que es un ChangeSet?


K.	¿Para qué sirve el import Wizard de Salesforce?

L.	¿Para qué sirve la funcionalidad Web to Lead?


M.	¿Para qué sirve la funcionalidad Web to Case?

N.	¿Para qué sirve la funcionalidad Omnichannel?


O.	¿Para qué sirve la funcionalidad Chatter?

Conceptos generales
A.	¿Qué significa SaaS? ¿Salesforce es Saas?
Software as a Service. Es una forma de disponer de software de tecnología por medio de Internet, sin la necesidad de instalar, mantener y actualizar hardwares o softwares, solo es neceesaria su conexión a Internet. Saleforce es un ejemplo de Saas.

B.	¿Que significa que una solución sea Cloud?
La información se aloja en servidores externos a los de la empresa a los que se puede acceder en cualquier momento mediante el Internet. Software estandarizado que se configura en función de las necesidades del cliente.

C.	¿Que significa que una solución sea On-Premise?
Sistemas que son instalados en los servidores y dispositivos locales en la propia empresa. Lo cual permite tener aceso físico a la infomación y control directo a la configuración manejo y seguridad de esos datos

D.	¿Que es un pipeline de ventas?
Mapa de actividades diarias, donde se muestra cada una de las etapas del proceso de ventas en alguna empresa. Este va desde que el cliente lo recibe hasta el cierre del negocio.

E.	¿Que es un funnel de ventas?
Sistema para atraer usuarios, convertirlos en leads para finalmente transformarlos en clientes dentro de la empresa. Este proceso sirve para generar confianza con los clientes potenciales.

F.	¿Qué significa Customer Experience?
Hace referencia a la experiencia basada en las interacciones que el cliente vivió dentro de una empresa.  Estos pueden ser observaciones tanto positivas como negativas

G.	¿Qué significa omnicanalidad?
Forma de comunicación utilizado por las empresas para tener una comunicación más eficiente con los clientes. Se busca mantener una relación con los clientes, en donde se pueda ir adaptando al medio que mejor le convenga  

H.	¿Qué significa que un negocio sea B2B?
Business yo business. Modelos de negocio en los que las transacciones de bienes o la prestación de servicios se producen entre dos empresas, por lo tanto, se relaciona principalemte con el comercio mayorista 

I.	¿Qué significa que un negocio sea B2C?
Business to Consumer. Hace referencia a empresas que ofrecen productos o servicios a personas. Está orientado a destacar los beneficios personales que aporta el producto a los consumidores.

J.	¿Qué es un KPI?
Key Performance Indicator. Dato que nos sirve para tomar decisiones. Manera de medir el desempeño de las empresas, unidades de negocios, proyectos o personal en relación con sus metas y objetivos dentro de la empresa

K.	¿Qué es una API y en qué se diferencia de una Rest API?

L.	¿Qué es un Proceso Batch?

Ejecución de un programa, sin la necesidad de la supervisión de algún usuario.

M.	¿Qué es Kanban?
Metodología para un sistema de producción efectivo y eficiente, su objetivo principal el gestionar de manera general como se van completando las tareas.

N.	¿Qué es un ERP? ¿Salesforce es un ERP?




