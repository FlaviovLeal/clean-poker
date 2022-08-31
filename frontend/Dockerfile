FROM node:latest
COPY my-app/ home/my-app/
RUN cd home/my-app/
WORKDIR /home/my-app/
RUN npm install
RUN npm audit fix
RUN npm run build
RUN apt install curl

CMD ["node", "./build/index.js"]