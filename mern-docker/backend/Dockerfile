ARG NODE_VERSION=24.11.0
FROM node:${NODE_VERSION}-alpine
# RUN addgroup app && adduser -S -G app app
# USER app
WORKDIR /app
COPY package*.json ./
# USER root
# RUN chown -R app:app .
# USER app
RUN npm install
COPY . .
EXPOSE 8000
CMD npm start