FROM ubuntu

# Create app directory
WORKDIR /usr/nodeapp  

COPY ./package*.json ./

COPY . .

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -
RUN apt-get install -y nodejs
RUN npm install
 

CMD [ "npm", "run", "start" ]