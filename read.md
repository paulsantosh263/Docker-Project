<!-- Build the Docker Image -->

docker build -t flask-docker

<!-- Run the Container -->

docker run -d -p 8085:5000 flask-docker


<!-- Push the image to Docker Hub -->

docker login

<!-- Tg the image -->

docker tag flask-docker <username>/flask-docker:latest

<!-- Push the Image -->

docker push <dockerhub_username>/flask-docker:latest
