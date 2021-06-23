FROM node:alpine

WORKDIR /app

ENV PATH /app/node_modules/.bin:$PATH

COPY package.json ./
COPY yarn.lock ./
COPY . ./
# COPY index.html ./public/
# COPY src ./
# COPY public ./

RUN yarn install

CMD ["yarn", "start"]