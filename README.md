## build2oss


## vuepress使用方法：

进到vuepress根目录，确保结构如下，有ossutilconfig文件

```
. 根目录
|--docs
|--|--.vuepress
|--|--|--config.js  vuepress配置文件
|--|--README.md
|--package.json     vuepress所属项目配置文件
|--ossutilconfig    阿里云oss配置参数
```

执行
```
docker run -i --name vuepress2oss -v "$(pwd)/":/var/app -e BUCKET=${BUCKET} autres/build2oss
```

## hexo使用方法：

进到hexo根目录，确保结构如下，有ossutilconfig文件

```
. 根目录
|--dist
|--package.json     vuepress所属项目配置文件
|--ossutilconfig    阿里云oss配置参数
```

执行
```
docker run -i --name vuepress2oss -v "$(pwd)/":/var/app -e BUCKET=${BUCKET} autres/build2oss
```

