# Modulo_Magento_Seur
Repositorio público del módulo oficial de SEUR para Magento

## v1.16.11
- Quitar espacios en las referencias de bultos, para evitar errores al comunicar envíos
- Corregir problema en procesamiento de código postal de origen

## v1.16.10

- Arreglado problema de compatibilidad con PHP 8.2, limpieza de código


 v1.16.9

- Arreglados errores en la definición de permisos ACL

v1.16.8
Corregido defecto en la operativa contrarreembolso.

v1.16.7
Añadida validación de credenciales ATLAS.
v1.16.6
Corregido defecto en consulta de puntos pickup

v1.16.5
Corregido defecto que impedía generar en ocasiones pedidos desde el backoffice.

v1.16.4
Eliminar campos de configuración obsoletos..

v1.16.3
Eliminar campos de configuración no utilizados.

v1.16.2
Arreglado pequeño bug de código en controlador de backend para obtener costes de un envío.

v1.16.1
Se han modificado las condiciones para agregar comentarios de envío.

v1.16.0
Agregue un nuevo método público para ampliar la funcionalidad de comentarios

v1.15.2
Arreglar inconsistencia entre referencia de expedición y tracking number

v1.15.1
Agregar campo "ecommerceName" a los parámetros de la petición API para comunicar envío nuevo a SEUR

v1.15.0
Migración de petición de coste de envío en backend a nueva API REST (valuate)

v1.14.7
Corrección de incidencias al registrar direcciones de usuario en pedidos "punto de recogida"

v1.14.6
Ajustes para pedidos enviados a punto de recogida
Refactorizar código

v1.14.5
Correcciones para mejorar compatibilidad con checkouts de tipo "one step"

v1.14.4
 - Corregir errores en la generación de manifiestos PDF
 - Eliminar enlace de impresión obsoleto en sección de seguimiento de la página de envío en backend
 - Eliminar código obsoleto

v1.14.3
 - Incluir librería PDFMerger en repositorio
 - Mejoras para evitar errores en checkout especiales en los que
   la dirección de envío puede ser nula cuando se solicita información al módulo SEUR
 - Limpieza de código obsoleto

v1.14.2
- Arreglar error PHP al comunicar envío cuando falta el teléfono en la configuración general de la tienda

v1.14.1
- Arreglar error PHP en procesamiento de método de envío (checkout, agregar productos a carrito)

v1.14.0
 - Agregar información ISO-23412 a comunicaciones de envíos

v1.13.0
- Migrar llamada API para obtención de ciudades a nueva API REST

v1.12.0
- Eliminación de atributos obsoletos para formato especial de campo "street" en direcciones de envío

v1.11.0

- Migración de generación de envíos a API REST (ATLAS)
- Migración de consulta de situaciones a API REST (ATLAS)
- Añadida funcionalidad que permite obtener etiqueta tras cambiar de formato para envíos ya generados.
- Solucionado problema con la generación de envíos con varios bultos.
- Optimización y refactorización de código.
v1.10.6

- Corrección que soluciona error en el fichero 'resource-url-manager.js' al manejar datos de dirección en el checkout.

v1.10.5

- Corrección que soluciona el error de autenticación en el web service de SEUR al solicitar puntos de recogida.

v1.10.4
 - Arreglar página de logs SEUR en backend, pequeño arreglo en código Javascript para puntos de recogida en checkout

v1.10.3
 - Arreglos en código Javascript de checkout

v1.10.2
 - Mejorar formulario de dirección en página de perfil de cliente

v1.10.1
 - Arreglar estilos de campos de dirección SEUR en checkout

v1.10.0
 - Implementar obtención de puntos de recogida usando nueva API de SEUR

v1.9.3
 - Mejorar configuración de campos de dirección de cliente en backend

v1.9.2
 - Arreglar error en fichero de plantilla para teléfono de contacto en método
 de envío de punto de recogida

v1.9.1
 - Arreglar error al generar PDF de manifiesto de envío

v1.9.0
 - Creación de nuevos estados de pedido (pedidos enviados a SEUR, pedidos entregados por SEUR)
 - Implementar URL LiveTrack para seguimiento de pedidos

v1.8.1
 - Añadida capacidad multi CCC
 - Modificado proceso de generación de envíos de internacional (Geolabel) en PDF (No se consume servicio de Labelary).
 - Añadida gestión de manifiesto en local
 - Añadidas funcionalidades de envío de partidas aduaneras y factura por API REST
 - Eliminación de funcionalidad de búsqueda de documentos DigitalDocu

v1.6.6
 - Mejoras en el tratamiento de errores al cambiar el formato de dirección
 - Arreglos en formulario de cliente en backend

v1.6.5
 - Comprueba si está activado el módulo antes de procesar los campos de dirección de cliente, para evitar errores con los campos de dirección.

v1.6.4
 - Corrección para incluir envío de internacional en manifiesto generado por WS

v1.6.2
 - Se cambia método de generación de manifiesto al servicio 'generacionPDFDetalle' (http://cit.seur.com/CIT-war/services/DetalleBultoPDFWebService) por incidencia EJB en CIT.

v1.6.1
 - Corregido proceso de desinstalación

v1.6.0
 - Modificado proceso de desinstalación

v1.5.6
 - Corregido tratamiento de envíos a PT y AD. Se consideran domésticos.

v1.5.4.2
 - Introduce pausa de 1 seg en la consulta situaciones para evitar bloqueos de nuestro WAF por exceso de peticiones por segundo.

v1.5.5
 - Corregido proceso de instalación

v1.5.4
 - Corrige generación adicional de registros en BDD

v1.5.3
 - corrige incompatibilidad con DHL

v1.5.2
 - corrige bug por el que se mostraban variables en checkout

v1.4.0
 - Corregido tratamiento de situaciones de envío

v1.2.3
 - Corregido detalle por el que aparecian campos de variables de programación en el checkout.

v1.2.1.0
 - Revisada compatibilidad del módulo con Magento 2.2.4 y 2.2.6. Modificado nombre del XML comunicado a SEUR.

v1.2.1
 - Añadida comunicación a API de Geolabel (Worldship)
