FROM node

WORKDIR /app

COPY . /app/

RUN npm install

# First we set the name and then we set the default value 
ENV PORT 80

EXPOSE $PORT

# This is a annonymous volume in docker file example
# VOLUME [ "/app/feedback" ]

CMD [ "npm", "start" ]
