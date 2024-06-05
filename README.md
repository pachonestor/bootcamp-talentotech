# Bootcamp Talento Tech Arquitectura de Nube
Despliegue de una arquitectura de AWS altamente disponible y escalable en AWS

## Planificación


### Requerimientos

* Requerimiento 1
* Requerimiento 2
* Requerimiento 3

### Arquitectura

En la siguiente imagen se muestra el diseño de la arquitectura a partir de los requerimientos
![arquitectura_aws](img/Arquitectura.png)

## Ejecución
* En primera instancia debemos conectarnos con AWS mediante el siguiente comando:
  ```
aws configure
```
Nos pedirá el Key ID y el Secret Access Key que debemos tener previamente configuradas para este ejercicio, como se ve en la siguiente imagen
![LoginAWS](img/LoginAWS.png)
### Pequeña descripcion sobre la fase de ejecución. Se utilizó el servicio de CloudFormation que es un servicio de infraestructura como código para realizar el despliegue de la arquitectura. Utilizamos el siguiente comando para realiza el despliegue de la arquitectura:
Primero debemos realizar la validación

```
aws cloudformation validate-template --template-body file://network.yml
```

```
aws cloudformation create-stack --stack-name network-stack --template-body file://network.yml
```


