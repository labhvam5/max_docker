FROM node

WORKDIR /app

COPY . /app/

RUN npm install

# Addign arguments
ARG DEFAULT_PORT=80

# First we set the name and then we set the default value 
# ENV PORT 80

# here we are making use of the arguments
ENV PORT $DEFAULT_PORT

EXPOSE $PORT

# This is a annonymous volume in docker file example
# VOLUME [ "/app/feedback" ]

CMD [ "npm", "start" ]
