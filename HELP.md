# Comenzando

### Documentación de referencia
Para más información, por favor considera las siguientes secciones:

* [Documentación oficial de Apache Maven](https://maven.apache.org/guides/index.html)
* [Guía de referencia del plugin Maven de Spring Boot](https://docs.spring.io/spring-boot/3.5.0/maven-plugin)
* [Crear una imagen OCI](https://docs.spring.io/spring-boot/3.5.0/maven-plugin/build-image.html)
* [Spring Web](https://docs.spring.io/spring-boot/3.5.0/reference/web/servlet.html)
* [Spring Data JPA](https://docs.spring.io/spring-boot/3.5.0/reference/data/sql.html#data.sql.jpa-and-spring-data)
* [Thymeleaf](https://docs.spring.io/spring-boot/3.5.0/reference/web/servlet.html#web.servlet.spring-mvc.template-engines)

### Guías
Las siguientes guías ilustran cómo usar algunas características de manera concreta:

* [Construyendo un servicio web RESTful](https://spring.io/guides/gs/rest-service/)
* [Sirviendo contenido web con Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Construyendo servicios REST con Spring](https://spring.io/guides/tutorials/rest/)
* [Accediendo a datos con MySQL](https://spring.io/guides/gs/accessing-data-mysql/)
* [Accediendo a datos con JPA](https://spring.io/guides/gs/accessing-data-jpa/)
* [Manejo de envío de formularios](https://spring.io/guides/gs/handling-form-submission/)

### Sobrescrituras del padre Maven

Debido al diseño de Maven, los elementos se heredan del POM padre al POM del proyecto.
Aunque la mayoría de la herencia es adecuada, también se heredan elementos no deseados como `<license>` y `<developers>` del padre.
Para evitar esto, el POM del proyecto contiene sobrescrituras vacías para estos elementos.
Si cambias manualmente a un padre diferente y realmente quieres la herencia, necesitas eliminar esas sobrescrituras.

