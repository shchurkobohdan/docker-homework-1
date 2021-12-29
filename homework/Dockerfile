FROM node:12-alpine as base
WORKDIR /app
COPY . /app
RUN apk add --no-cache python3 g++ make; \
    yarn install; \
    yarn test

FROM base as production
RUN yarn install --production
CMD ["node", "src/index.js"]
EXPOSE 3000