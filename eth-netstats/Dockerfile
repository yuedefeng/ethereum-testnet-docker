FROM node:9

RUN git clone https://github.com/cubedro/eth-netstats --depth 1

WORKDIR /eth-netstats

RUN npm config set unsafe-perm true
RUN npm install --registry=https://registry.npm.taobao.org
RUN npm install -g grunt-cli --registry=https://registry.npm.taobao.org
RUN grunt

EXPOSE 3000

CMD ["npm", "start"]
