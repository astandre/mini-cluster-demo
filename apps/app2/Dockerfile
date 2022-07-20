# A minimal Docker image based on Alpine Linux with a complete package index and only 5 MB in size
FROM node:16-alpine
# Debian releases
#FROM node:16-bullseye

#FROM node:16-bullseye-slime


WORKDIR /home/app1

#COPY ./apps/app1 /home/app1
COPY . /home/app1

RUN npm ci

RUN npm run prebuild && npm run build

EXPOSE 3000


CMD ["node", "dist/main.js"]

