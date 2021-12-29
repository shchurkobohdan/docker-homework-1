# Home task
1. Split Dockerfile into two stages:
   1. Run tests
   2. Production
2. The production image should contain minimum data
3. `RUN apk` needed only for tests
4. Use `yarn install --production` to minimize dependencies at production


# To verify run the following command in the root dir:
docker build -t hometask:latest -f homework/Dockerfile ./homework

docker run -p 80:3000 hometask


