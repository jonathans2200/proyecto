Demo Project 

## GENERAR LA IMAGEN CON MAVEN
    mvnw clean package jib:dockerBuild

## Levantar el conenedor
  docker-compose up

## Ingresamos al url
  https://localhost:8080/jenkins

## Verificamos la contraseña que se genero
docker exec -it 4a8b19d6829 /bin/bash
  ### dentro del contenedor ingresamos el siguiente comando 
  
  cat /var/jenkins_home/secrets/initialAdminPassword


  # Usuario y contraseña del jenkis 

  username: jonathan
password: admin



# Error 1

User
java.lang.NoSuchMethodError: No such DSL method 'dependencyCheckPublisher'

## Solucion

Instalar el plugin
OWASP Dependency-Check Plugin


# Error 2
Also:   org.jenkinsci.plugins.workflow.actions.ErrorAction$ErrorId: fdf6955b-fc70-4972-b4b5-16cd7f20f6f4
java.lang.NoSuchMethodError: No such DSL method 'spotBug

## Solucion
Instalar el plugin
Warnings


# Error 3 

java.lang.NoSuchMethodError: No such DSL method 'publishHTML'

## Solucion 
 instalar el plugin HTML Publisher 
 # Error 4 

 Also:   org.jenkinsci.plugins.workflow.actions.ErrorAction$ErrorId: 21a558fa-5ddf-45d8-a981-e1f63ad4e020
java.lang.NoSuchMethodError: No such DSL method 'withSonarQubeEnv' found among steps [archive, bat, build, catchError, checkout, deleteDir, dependencyCheckPublisher, dir, echo, emailext, emailextrecipients, 
 
# Solucion 
Instalar el publig  SonarQube Scanner


# Error 5 


ERROR: SonarQube installation defined in this job (sonarqube-server) does not match any configured installation. Number of installations that can be configured: 0.
If you want to reassign jobs to a different SonarQube installation, check the documentation under https://redirect.sonarsource.com/plugins/jenkins.html
Finished: FAILURE

## Solucion:

Instalar el publing sonarque


