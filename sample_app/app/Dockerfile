# syntax=docker/dockerfile:1
FROM node:12-alpine
RUN apk add --no-cache python g++ make
WORKDIR /app
COPY . .
# ENV MYSQL_HOST=mysql
# ENV MYSQL_USER=root
# ENV MYSQL_PASSWORD=secret
# ENV MYSQL_DB=todos  
RUN yarn install --production
CMD ["node", "src/index.js"]