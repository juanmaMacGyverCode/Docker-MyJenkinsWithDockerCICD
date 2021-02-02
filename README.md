# Para crear la imagen

docker build -t [inserte_aquí_su_usuario_de_docker_sin_corchetes]/[nombre_imagen_sin_corchetes] .

# Para ejecutar Docker

docker run --group-add 0 --name [nombre_contenedor_sin_corchetes] -p 20000:8080 -p 50000:50000 -v //var/run/docker.sock:/var/run/docker.sock [inserte_aquí_su_usuario_de_docker_sin_corchetes]/[nombre_imagen_sin_corchetes]

# Para ejecutar SonarQube

docker run -d --name [nombre_contenedor_sin_corchetes] -p 9000:9000 sonarqube
