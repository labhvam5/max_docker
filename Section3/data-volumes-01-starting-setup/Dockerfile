FROM node

WORKDIR /app

COPY . /app/

RUN npm install

EXPOSE 80

# This is a annonymous volume in docker file example
# VOLUME [ "/app/feedback" ]

CMD [ "npm", "start" ]
