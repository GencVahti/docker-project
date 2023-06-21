FROM node:lts-alpine
# ENV NODE_ENV=production
WORKDIR /usr/src/app
COPY ["app/package.json", "app/package-lock.json*", "./"]
RUN npm install --production --silent && mv node_modules ../
COPY app/ .
EXPOSE 3000
RUN chown -R node /usr/src/app
USER node
CMD ["node", "app.js"]
