docker
```
// 构建容器
docker image build -t demo .
docker image ls

// 运行容器
docker container run -p 8000:4000 -it demo /bin/bash

// 以上命令执行完自动进入容器，以下为容器内部的运行命令
rm -rf build

// node-gyp 安装
npm i -g node-gyp --registry=https://registry.npm.taobao.org
npm run install

apt-get update
apt-get install build-essential libcairo2-dev libpango1.0-dev libjpeg-dev libgif-dev librsvg2-dev
node-gyp configure

npm run pretest-server
npm run test-server
```