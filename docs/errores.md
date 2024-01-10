La API de Tecopos usa como guía las convenciones de los código de estado de respuestas HTTP para indicar el éxito o fallo de una petición.

</br>

| HTTP | Código de estado | Resumen |
| ---- | ---- | ---- |
| 200 | OK | Todo funcionó como se esperaba |
| 201 | Created | La petición fue un éxito y un nuevo recurso fue creado como resultado |
| 400 | Bad Request | El servidor no procesará algo que es percibido como error del cliente, como por ejemplo un parámetro requerido que falta |
| 404 | Not Found | El servidor no puede encontrar el recurso solicitado |
| 406 | Not Acceptable | El parametro como identificador único falta |



