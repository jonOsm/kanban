# build stage
FROM node:lts
WORKDIR /app
# COPY package*.json ./
# RUN npm install
RUN npm install -g @vue/cli

# COPY . .
EXPOSE 8080
# CMD [ "npm", "run", "serve" ]
# # production stage
# FROM nginx:stable-alpine as production-stage
# COPY --from=build-stage /app/dist /usr/share/nginx/html
# EXPOSE 80
# CMD ["nginx", "-g", "daemon off;"]