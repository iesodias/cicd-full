# Build the Docker image

Let’s proceed to build the image with the command below:

´´´
docker image build -t flask_docker .
´´´


# Run the container

After successfully building the image, the next step is to run an instance of the image. Here is how to perform this:

´´´
docker run -p 5000:5000 -d flask_docker
´´´

This command runs the container and its embedded application, each on port 5000 using a port-binding approach. The first 5000 is the port that we allocate to the container on our machine. The second 5000 is the port where the application will run on the container.