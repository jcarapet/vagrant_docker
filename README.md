this is a cookbook to run and create a working ubuntu vm with Docker on it for testing environments.
I find this a little bit nicer to work with than boot2docker, but that is just a preference. 

simply run vagrant up to get docker installed

vagrant ssh into the box to utilize docker

You will need to run a docker build in the specific project directories for images to be downloaded. 

This can be done with 

cd docker_nexus && sudo docker build ./

afterwards, you will need to run "sudo docker run -d -p hostport:containerport image_name" to create the container and launch the application.

