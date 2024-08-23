# ASINCRONIA JS

## ¿Qué es el protocolo HTTP?
Es el lenguaje que utilizan los **navegadores** y los **servidores** (cliente-servidor) para intercambiar información en la web mediante peticiones(**request**).

## ¿Qué es verbos HTTP(Ejemplos)?
El verbo es una acción a realizar (operación/tarea) en una solicitud http. Los verbos más utilizado son:
- **POST**: Envía y crea data en el servidor. *Ejm: Cuando enviamos datos por un formulario.*
- **GET**: Obtiene información del servidor. *Ejm: Cuando abreas una web como google, el navegador usa **GET** para solicitar la info de esta página.*
- **PUT**: Actualiza información en el servidor con datos enviados al servidor. *Ejm: Me olvide mi clave y necesito cambiarla, enviaría la solicitud y se actualizaría la clave*
- **DELETE**: Este verbo sirve para eliminar data en el servidor. *Ejm: Deseo eliminar un usuario registrado, enviaría la solicitud para la respectiva eliminación de ese usuario.*

## ¿Qué es el body en protocolo http?
El **Body** contiene la data que se envia al servidor por ejemplo cuando usamos POST para enviar un usario y clave, body contendrá los datos: **{usuario: Víctor clave: 123456}** en formato **JSON**.

## ¿Qué son los headers en protocolo http?
Es la parte donde se encuentran los metadatos para la debida comunicación web. Los headers **proporcionan información adicional al request** (petición).

Ejm:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" href="./style.css">
```
También es donde se encuentran los **tokens** que es un dato esta se genera cuando usamos un request POST y esta es correcta, tienen ciclo de vida y esta relacionado al tema de seguridad permitiendo la autenticación y autorización en las aplicaciones web. 

## ¿Qué son los code response *(respuestas de codigo en el protocolo HTTP)*?
Los Code Response son los **status** (mensajes) que los servidores emiten en respuesta a un request enviado por los navegadores.

Tenemos los 100-10x, 200-20x, 300-30x, 400-40x y 500-50x.

Ejms.:
- **404** : Página no encontrada.
- **200 OK**: La solicitud ha tenido éxito.
- **500**: Error Interno del Servidor.

## ¿Qué es un request y response en el protocolo HTTP?
Request (solicitud) y response (respuesta) son los componentes principales cómo un **cliente y un servidor se comunican entre sí**.

*Ejm: Validación de password, se ingresa usuario y clave (Request) validación de la clave en el servidor y emite mensaje si es cierto o no (response).*

## ¿Qué es la asincronia en Javascript?

La asincronía se refiere a que JavaScript puede realizar operaciones que **no bloquean la ejecución del código.** En lugar de esperar a que una tarea se complete (modo sincrónico), JavaScript puede ejecutar varias tareas al mismo tiempo, es decir se pueden ejecutar sin esperar que termine una detrás de otra.

*Ejm.: Envío de un formulario mediante un botón mientras se ejecuta el envío se puede interactuar con otros elementos de la web.*

## ¿Cómo realizar peticiones asincronas?
Para relizar las peticiones asincronas o realizar consumo se utilizan los métodos:
- XMLHttpRequest
- fetch()
- Axios (librería)

## ¿Cómo manejar la data luego de la peticion asincrona?
Para manejar la data luego de la petición se realiza mediante:

- Callbacks
- Promises
- async/await
