FROM node

WORKDIR /app

COPY . /app/

RUN npm install

EXPOSE 80

# This make sure that the /app/feedback folder in the container is mapped to a folder in the host machine to copy files
VOLUME [ "/app/feedback" ]

CMD [ "node", "server.js" ]
