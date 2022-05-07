# SpringBootAdmin
Spring boot admin project to manage spring boot instances

# Properties
````
spring.application.name=application name
server.port=8081 
#credentials for accessing spring boot admin
spring.security.user.name=admin
spring.security.user.password=password

#configs to connect to self register the admin server as a client
spring.boot.admin.client.url=http://spring_boot_admin_url:port
spring.boot.admin.client.username=${spring.security.user.name}
spring.boot.admin.client.password=${spring.security.user.password}

#configs to give secured server info
spring.boot.admin.client.instance.metadata.user.name=${spring.security.user.name}
spring.boot.admin.client.instance.metadata.user.password=${spring.security.user.password}

management.endpoints.web.exposure.include=*
management.endpoint.health.show-details=always

#mail notifications
spring.mail.host=
spring.mail.username=
spring.mail.password=
spring.mail.port=
spring.mail.properties.mail.smtp.auth=
spring.mail.properties.mail.smtp.starttls.enable=

spring.boot.admin.notify.mail.to=

````
