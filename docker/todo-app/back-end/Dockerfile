FROM node:14-alpine

WORKDIR /docker/todo-app/backend
ADD node_modules.tar.gz ./node_modules.tar.gz
COPY package.json ./
COPY package-lock.json ./
COPY src ./src
RUN npm install
EXPOSE 3001
ENTRYPOINT [ "npm" ]
CMD [ "start" ]
