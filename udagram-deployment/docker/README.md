# deployment

Tasks
Setup Docker Environment
You'll need to install docker https://docs.docker.com/install/. Open a new terminal within the project directory and run:

Build the images: docker-compose -f docker-compose-build.yaml build --parallel
Push the images: docker-compose -f docker-compose-build.yaml push
Run the container: docker-compose up
