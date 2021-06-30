FROM node:16-alpine
WORKDIR /usr/src/app
ENV PATH /app/node_modules/.bin:$PATH
COPY package.json yarn.lock ./
COPY ./src ./src
COPY ./public ./public
EXPOSE 3000
RUN yarn install
CMD [ "yarn", "start" ]
