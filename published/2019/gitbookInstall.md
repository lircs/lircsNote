# 1. 安装`git`
```shell
sudo apt install git
```

# 2. 安装 nodejs

```shell
# nodejs 官网
# https://nodejs.org/en/

# 解压 node-v10.16.3-linux-x64.tar.xz
xz -d node-v10.16.3-linux-x64.tar.xz
tar -xvf node-v10.16.3-linux-x64.tar

# 建立软链接
sudo ln -s /home/jam/software/nodejs/node-v10.16.3-linux-x64/bin/node /usr/local/bin/node
sudo ln -s /home/jam/software/nodejs/node-v10.16.3-linux-x64/bin/npm /usr/local/bin/npm

# 检查是否安装成功
node -V
npm -V
```

# 3. 安装 gitbook

```shell
# 安装 gitbook
npm install -g gitbook-cli

# 检查是否安装成功
gitbook -V
```

# 4. gitbook 使用

```shell
gitbook -h

# 初始化一本电子书
gitbook init

# 生成 web 服务并查看，localhost:4000
gitbook serve
```

# 5. Todo

- [ ] 对生成 pdf 电子书的支持
