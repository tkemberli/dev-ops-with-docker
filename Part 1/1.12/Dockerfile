FROM node:16-alpine3.15

WORKDIR /usr/src/app 

COPY . .

RUN npm install

RUN npm run build

RUN npm install -g serve

ENV REACT_APP_BACKEND_URL=http://localhost/

CMD ["serve", "-s", "-l", "5000", "build"]

EXPOSE 5000
