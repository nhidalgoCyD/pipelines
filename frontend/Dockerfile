FROM node:alpine3.16
WORKDIR /app
COPY package.json ./
# COPY package.json yarn.lock ./
RUN yarn install --frozen-lockfile
COPY . .
RUN yarn build
EXPOSE 3000
CMD ["yarn", "start"]