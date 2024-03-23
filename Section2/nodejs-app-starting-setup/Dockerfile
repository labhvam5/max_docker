# # Pulling the base image from local or Dockerhub
# FROM node

# # This sets the working directory and all the CMD commands will run relative to this WORKDIR
# # In this case the WORKDIR is /app
# WORKDIR /app

# # COPY will take 2  pathes
# #  first . = The host file system or our local file system.
# #  second . = The image/container file system
# #  In this case the . folder which is the base folder will copy all the files to ./app folder in docker image.
# COPY . /app

# # This RUN will run any command specified in the WORKDIR directory while building the image
# # In this case the npm install command is ran in the /app directory
# RUN npm install

# # EXPOSE will expose port from your host to the image.
# # In this case the server is running on 80 port so 80 is the port that we exporse from our local to the image 80 port.
# EXPOSE 80

# # This CMD sepcifies a command that will run when we are trying to run a container from this image.
# # In this case we are running "node server.js" everytime once at the end when we try to run contianer/containers.
# CMD ["node", "server.js"]



# Second version 


# After the layering process 
# We will be copying the package.json file and then run npm install
# and then we copy all the source code this will help in not runnign npm install even if server.js is changed.



# Pulling the base image from local or Dockerhub
FROM node


WORKDIR /app

COPY package.json /app

# This RUN will run any command specified in the WORKDIR directory while building the image
# In this case the npm install command is ran in the /app directory
RUN npm install

# COPY will take 2  pathes
#  first . = The host file system or our local file system.
#  second . = The image/container file system
#  In this case the . folder which is the base folder will copy all the files to ./app folder in docker image.
COPY . /app

# EXPOSE will expose port from your host to the image.
# In this case the server is running on 80 port so 80 is the port that we exporse from our local to the image 80 port.
EXPOSE 800

# This CMD sepcifies a command that will run when we are trying to run a container from this image.
# In this case we are running "node server.js" everytime once at the end when we try to run contianer/containers.
CMD ["node", "server.js"]