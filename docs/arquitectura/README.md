# Arquitectura de referencia

Os mostramos a continuación la arquitectura de referencia de los componentes principales que podéis emplear en el reto.

![Arquitectura](../images/arquitecturaref.png)

La arquitectura consta de una pieza central, que es el asistente virtual, basado en tecnología [IBM Watson Assistant](../watsonai).
Este asistente guiará al usuario final a través de un diálogo programado para determinar las intenciones, palabras clave, etc.

En caso de que el asistente necesite acceder a información adicional para ofrecer una respuesta más compleja, o para hacer más rico el propio diálogo, puede acceder a diversos servicios en el backend. Para conseguir esto, existen varias opciones:

* Funciones serverless que acceden a una [base de datos](../ibmcloud#servicios-de-bases-de-datos) a buscar o actualizar información.

* Integración con [Watson Discovery](../watsonai#que-es-watson-discovery) para localización de información en base a determinados parámetros.

Para la capa de front end, también contamos con varias alternativas, que van desde una integración sencilla del asistente en una página web, o integración con diferentes sistemas de mensajería que por defecto soporta Watson Asssitant, como Facebook Messenger, Slack o WhatsApp. 

!!! info 
    Otra opción es desarrollar vuestro porpio cliente e integrar ahí la funcionalidad de Watson Assistant [invocando su API](../watsonai#que-son-watson-apis). 
    Un ejemplo de esto es también la [integración específica con Discord](../ejemplo), que se ha desarrolldo ad-hoc para que podáis consultar cómo acceder al API de Watson Assistant.
