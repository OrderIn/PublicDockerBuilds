# PublicDockerBuilds

1. Build your docker image: `docker build -t <container_name> .`
   1. or docker `build -t <container_name> -f <dockerfile_name> .` to specify the specific docker file to build
2. Get your docker image id: `docker images`
3. Tag your docker image: `docker tag <container_name> <image_tag>`
4. Login to Docker Hub: docker login using the oidevops credentials from LastPass
5. Push your image to Docker Hub: `docker push <container_name>`


**Tips:**
1. If you need to verify anything in the docker image you can connect to its command line using: `docker run -it <container_name> sh`. Once connected, you can run any of the regular shell commands that should be available (if they are available in the environment) e.g `dotnet --version` etc

2. To copy files from you local machine (or vice versa) to the docker image you can run `docker cp some_file.txt <container_name>:/some_file.txt`