
Ansible-Playbook

This Playbook file is used to automate building docker image, since we are using a lot of commands to build, remove, and push images also to stop, remove and run containers so this file contains all the commands that you are going to use while testing building, pushing an image and run container.

The file should do the following:

-  Stop the current running container if exist
-  Remove the stopped container if exist
-  Remove the built image if exist
-  Build a new image from the Dockerfile
-  Create a tag to the image
-  Push the new built image to Dockerhub
-  Run a container from the new built image

So as you see this file is idempotent file that can run miltiple times without changing the output plus you can use only one image name and one container name so you don't get lost by the number of images and names that you are going to build with different names.
