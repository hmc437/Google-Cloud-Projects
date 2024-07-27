# Terraform
Terraform permite desplegar infraestructura en provedores de cloud y debe estar declarada en archivos con el lenguaje de terraform. Interprentando esos archivos y haciendo uso de las APIs de las plataformas cloud se encargará de generar toda esa infraestructura.  
  
Se le provee con el código de la infraestructura y se necesita una cuenta en el proveddor de la nube a usar. Al instalar Terraform usará tus permisos.  
  
Terraform va a generar un archivo llamado states donde guardará todo lo que va haciendo como una lista de tareas. También, descargará provider/plugins que necesita para pode generar esa infraestructura.  
  
Las ventajas que proporciona son:  
- Al trabajar todo con código aparecen beneficios como versionamiento, lectura rápida al tenerlo todo en los archivos (en vez de diferentes pestañas en el proveddor de la nube) y poder usar estructuras de datos y modularización.  
- Se pueden replicar ambientes con facilidad. Por ejemplo, un entorno en desarrollo cogiendo esos archivos y con pocas modificaciones se puede replicar en producción.  
- Multi nube al poder ser usado en muchas plataformas de cloud.  

¿Qué cosas pueden hacerse?  
- Poder desplegar máquinas virtuales y diferentes servicios y poder relacionarlos entre ellos, creando la arquitectura de la aplicación.  

Comandos básicos de Terraform:  
- terraform init : se utiliza para iniciar el directorio de trabajo que contiene los archivos de configuración de Terraform.
- terraform plan:   con este comando Terraform realiza una actuaslización y luego determina que acciones son necesarias para alcanzar el estado deseado en los archivos de configuración. Es conveniente usarlo para comprobar que los cambios realizados a la configuración cumplen las expectativas antes de aplicarlos a  los recursos en producción.
- terraform apply: se utiliza para aplicar los cambios realizados o las acciones predeterminadas generadas por el plan de ejecución de Terraform.  
- terraform destroy  

  ![Diagrama HTTPS Content-Based Load Balancer with Terraform](https://github.com/hmc437/Google-Cloud-Projects/blob/45e1fb8dc68337d5ddcee49de3d468c3c99f61a3/Managing%20Cloud%20Infrastructure%20with%20Terraform/diagram.png)
