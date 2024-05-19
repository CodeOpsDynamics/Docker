FROM node:lts-alpine3.19 as myimage
WORKDIR /app
COPY package.json .
#main build has been copied at initial step to reduce build time
RUN npm install
#npm install runs for package.json only not for entire code
COPY . .
#RUN npm install
RUN npm run build

FROM nginx:alpine
COPY --from=myimage /app/build /usr/share/nginx/html