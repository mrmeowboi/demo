# FROM node
# WORKDIR app/
# COPY package*.json .
# RUN npm install --y
# COPY . .
# CMD ["node","app/index.js"]
# EXPOSE 3000

FROM node
RUN mkdir /build
COPY ./build /build
RUN npm install --global serve -y
ENTRYPOINT ["serve","-s","build"]
EXPOSE 3000


# FROM ubuntu
# RUN mkdir /build
# COPY build /build
# RUN curl -sL https://deb.nodesource.com/setup_16.x | bash - 
# RUN apt-get update -y
# RUN apt-get install nodejs -y
# RUN apt-get install npm -y
# RUN npm install --global serve -y
# ENTRYPOINT ["serve","-s","build"]
# EXPOSE 3000




# RUN curl -sL https://deb.nodesource.com/setup_14.x | bash - 
# RUN apt update -y
# RUN apt install nodejs -y
# WORKDIR /abc
# RUN npm install  
# RUN apt-get install npm -y
# WORKDIR /abc
# RUN npm install
