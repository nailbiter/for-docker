# use an existing docker image as a base
FROM node:alpine

# download and install a dependency
#RUN apk add --update nodejs 
WORKDIR /usr/app
COPY ./package.json ./
RUN npm install
COPY ./index.js ./

# tell the image what to do when it 
# starts as a container
#CMD ["redis-server"]
CMD ["npm","start"]
