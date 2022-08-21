#Setting a base-image.
FROM node

#Setting the work directory path inside the container.
WORKDIR /app

#Copying files into the conteiner.
#1st param: Files to be copied.
#2nd param: Path to paste the files. Could be changed to '.' or './' of WORKDIR is setted.
COPY . /app

#npm install to install all nodejs dependencies.
#If WORKDIR is not setted, this will be run on the root folder.
RUN npm install

#Exposes a certain port from the container to the local machine. 100% optional, since it doesn't really expose the port.
#Instead, you can use the flag –p "[LOCAL_PORT]:[DOCKER_EXPOSED_PORT]" to expose docker ports.
EXPOSE 80

#Command that runs when a CONTAINER with the image is started.
CMD ["node", "server.js"]

