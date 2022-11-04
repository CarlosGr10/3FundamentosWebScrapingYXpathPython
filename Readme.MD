# Curso de Fundamentos de Web Scraping con Python y Xpath

- Web scraping Es una técnica usada por data scientist y backend developers para extraer información de internet, accede a esto usando el protocolo de tranferencias de hipertexto (HTTP) o a través de un navegador. Los datos extraídos usualmente son guardados en una
base de datos, incluso en una hoja de cálculo para posteriores análisis. Puede hacerse de manera automática (bot) o manualmente.

- Xpath es un lenguaje que sirve para apuntar a las partes de un documento XML. Xpath modela un documento XML como un árbol de nodos. Existen diferentes tipos de nodos: elementos, atributos, texto.

# Entender HTTP

![](https://i.imgur.com/aiDV5MB.png)

HEADERS

Permiten al cliente y el servidor passar información adicional con un request o response HTTP.
Pueden agruparse en las siguientes categorías:

Generales : Aplica para request y responses pero no tiene relación con la data transmitida en el cuerpo
Request : Contienen más información acerca del recurso a ser fetch (extraer)
Response : Contiene información adicional sobre respuestas. Como ubicación o el Server provider.
Entity : Contien información acerca del recurso del cuerpo.
Existen muchas cabeceras o headers como:

Accept
Authorization
Link
Location
Save-Data

Códigos de estado HTTP más comunes

Status code 200 – OK.
Status code 301 – Moved Permanently.
Status code 302 – Moved Temporarily.
Status code 403 – Forbidden
Status code 404 – Not Found
Status code 500 – Internal Server Error
Status code 503 ­– Service Unavailable

### Protocolos debajo

IP - Internet Protocol
Salen las direcciones ipv4 y ipv4 que identifican de manera unica a nuestra computadora en la red

TCP - Transmision Control Protocol
Como se va transferir informacion a bajo nivel

UDP - User Datagram Protocol
Se encarga de proporcionar un servicio de comunicación punto a punto no orientado a conexión, sino a transacciones 

TLC - Transport Layer Security
El encriptado de informacion para que un atacante no pueda ver lo que se esta enviando

DNS - Domain Network System 
Resuleve un nombre de nominio a una IP

![](https://i.imgur.com/wWne1SM.png)

# ¿Qué es HTML?

Define la estructura de una página web

# Robots.txt: permisos y consideraciones al hacer web scraping

Los archivos robots.txt exiten como una forma de administrar una página web.
proporciona información a los rastreadores de los buscadores sobre las páginas o los archivos que pueden solicitar o no de tu sitio web.
Principalmente, se utiliza para evitar que tu sitio web se sobrecargue con solicitudes.
En el contexto de webscraping, le dice al scraper que puede y no extraer. Es decir hasta donde puede llegar. Ya que infrigir en la violación
de estas directivas puede acarrear un problema legal con el sitio web al que estamos scrapeando.

Robots.txt
Contiene entre otros elementos:

USER-AGENT: Identificadores de quienes acceden a tu sitio web, puede ser un archivo.py hasta un googlebot.

DIRECTIVAS

ALLOW: Utiliza esta directiva para permitir a los motores de búsqueda rastrear un subdirectorio o una página, incluso en un directorio que de otro modo no estaría permitido
DISALLOW: Utiliza esta directiva para indicar a los motores de búsqueda que no accedan a archivos y páginas que se encuentren bajo una ruta específica

[.: Mas informacion :.](https://developers.google.com/search/docs/crawling-indexing/robots/create-robots-txt?hl=es&visit_id=638031326822695480-2291008621&rd=1)

Entrar al archivo robots de un sitio web

```
    https://sitioweb.con/robots.txt
```

