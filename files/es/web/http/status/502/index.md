---
title: 502 Puerta de enlace no válida
slug: Web/HTTP/Status/502
tags:
  - Codigo de Estado
  - Error de servidor
  - HTTP
translation_of: Web/HTTP/Status/502
---

{{HTTPSidebar}}

El código de respuesta de error del servidor de HTTP **`502 Bad Gateway`** indica que el servidor, mientras actuaba como una puerta de enlace o proxy, recibió una respuesta no válida del servidor ascendente.

> **Nota:** Una {{interwiki("wikipedia", "Puerta_de_enlace", "puerta de enlace")}} puede referirse a cosas distintas en redes y un error 502 no es algo que normalmente puedas arreglar, ya que requiere correcciones por parte del servidor o los proxies a través de los que intentas acceder.

## Estado

```
502 Bad Gateway
```

## Especificaciones

| Especificación                                               | Título                                                        |
| ------------------------------------------------------------ | ------------------------------------------------------------- |
| {{RFC("7231", "502 Bad Gateway" , "6.6.3")}} | Hypertext Transfer Protocol (HTTP/1.1): Semantics and Content |

## Compatibilidad con navegadores

{{Compat("http.status.502")}}

## Vea también

- {{HTTPStatus(504)}}
