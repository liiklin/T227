### 开发
下载安装nodejs开发环境后，克隆代码
```
git clone https://github.com/liiklin/T227.git
```

修改数据库连接，文件在/src/common/config/db.js
运行命令
```
npm install

npm start
```

### 部署

采用 docker 部署的方法
```
docker build -t t227_web -f docker/Dockerfile .
docker-compose -f docker/docker-compose.yml up -d
```
启动后需要执行初始化sql.

按 docker-compose.yml 中的配置，可访问 http://localhost:8360