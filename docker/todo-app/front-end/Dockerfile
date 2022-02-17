FROM node:14-alpine

WORKDIR /docker/todo-app/front-end
ADD node_modules.tar.gz ./node_modules.tar.gz
COPY package.json ./
COPY package-lock.json ./
COPY src ./src
RUN npm install
EXPOSE 3000
ENTRYPOINT [ "npm" ]
CMD [ "start" ]
