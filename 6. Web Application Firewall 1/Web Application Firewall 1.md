Creación de un grupo de destino (target group)
![alt text](Grupo%20de%20destino.png)

Grupo de seguridad
![alt text](Grupo%20de%20seguridad.png)

Creación del balanceador de carga
![alt text](Balanceador%20de%20carga.png)

Comprobación de la conexión
![alt text](Aplicación%20cargada.png)
![alt text](Petición%20de%20conexión.png)
![alt text](Respuesta%20de%20conexión.png)

WEB APPLICATION FIREWALL
Creación de una regla en WAF
![alt text](Regla%20WAF.png)

Comprobación del funcionamiento
- ¿Qué valor devuelve la petición? ¿Es un código 200? Haz una captura de pantalla de la petición y su respuesta.
    El valor de la petición que devuelve el código es 200. Sí, es un código 200.
    ![alt text](Petición%20de%20funcionamiento.png)
    ![alt text](Respuesta%20de%20funcionamiento.png)

- Analiza los logs. ¿Encuentras las peticiones que se han realizado? ¿Puedes ver si se han aceptado o se han bloqueado? Adjunta captura de pantalla de los logs donde se aprecie dicho resultado.
    Sí, he encontrado las peticiones que se han realizado. Puedo ver que se han bloqueado.
    ![alt text](Analizar%20logs.png)

Preguntas adicionales
- ¿Qué precio tiene AWS WAF? ¿Cuánto costaría la Web ACL creada con la regla que hemos configurado? Haz una estimación del coste en AWS Calculator.
    AWS WAF tiene una estructura de precios basada en tres componentes principales: Web ACLs, reglas y solicitudes. Se cobra una tarifa mensual por cada Web ACL creada, además de un costo adicional por cada regla dentro de la ACL. También hay un cargo por cada millón de solicitudes web procesadas por la Web ACL. Los precios exactos pueden variar según la región y pueden cambiar con el tiempo. Para obtener una estimación precisa, lo mejor es utilizar la Calculadora de Precios de AWS, donde puedes ingresar los detalles específicos de tu configuración y obtener un costo estimado.

- ¿Qué servicios se pueden proteger con AWS WAF?
   AWS WAF protege aplicaciones web y se integra con varios servicios de AWS. Entre los principales servicios que pueden beneficiarse de esta protección están Amazon CloudFront, Application Load Balancer (ALB), Amazon API Gateway y AWS App Runner. Estos servicios permiten distribuir contenido y gestionar el tráfico de aplicaciones, y al combinarse con AWS WAF, pueden mitigar amenazas comunes como ataques de inyección SQL, intentos de explotación de vulnerabilidades y ataques DDoS.

- ¿Qué otras reglas se encuentran disponibles dentro de la categoría Free rule groups?
    Dentro de la categoría de grupos de reglas gratuitas (Free rule groups) proporcionadas por AWS Managed Rules, existen varias opciones diseñadas para mejorar la seguridad de aplicaciones web sin costo adicional. Algunos ejemplos son AWSManagedRulesCommonRuleSet, que protege contra vulnerabilidades web comunes, AWSManagedRulesKnownBadInputsRuleSet, que bloquea entradas maliciosas conocidas, y AWSManagedRulesAmazonIpReputationList, que filtra tráfico de direcciones IP con mala reputación. También están disponibles reglas como AWSManagedRulesAnonymousIpList, que bloquea tráfico de VPNs y proxies anónimos, y AWSManagedRulesAdminProtectionRuleSet, que protege páginas de inicio de sesión y paneles de administración.