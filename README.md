# PublicDockerBuilds

1. Build your docker image: docker build -t <image_tag> .
2. Get your docker image id: docker images
3. Tag your docker image: docker tag <image_id> <image_tag>
4. Login to Docker Hub: docker login using the oidevops credentials from LastPass
5. Push your image to Docker Hub: docker push <image_tag>
