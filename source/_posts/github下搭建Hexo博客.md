---
title: Github下搭建Hexo博客
---

### 准备工作
- GitHub账号
- 安装Git
- 安装NodeJS
  创建仓库，格式必须为<用户名>.github.io

### 安装Hexo
```
npm install -g hexo-cli

hexo -v

hexo init hexo-blog

cd hexo-blog

npm install

hexo clean

hexo g

hexo server
```

浏览器访问 [http://localhost:4000](http://localhost:4000)

### 更换主题
[https://github.com/fluid-dev/hexo-theme-fluid/releases](https://github.com/fluid-dev/hexo-theme-fluid/releases)

```
cd hexo-blog

git clone https://github.com/fluid-dev/hexo-theme-fluid/releases themes/next

// 打开 _config.yml 文件 将主题修改为 next(将主题文件地址放在themes下，theme更改为对应文件名)
theme: next
```

### 发布到GitHub Pages
安装hexo-deployer-git

npm install hexo-deployer-git –save

修改根目录下的 _config.yml，配置 GitHub 相关信息

```
deploy:
  type: git
  repo: git@github.com:xxx/xxx.github.io.git
  branch: master
```

部署到GitHub

hexo g -d

### 部署到nginx
- hexo g 生成静态文件
- 上传到nginx服务器
- 配置nginx访问地址

```
server {
    listen       80;
    server_name  127.0.0.1;

    location / {
        root  /data/www/blog;
        index  index.html index.htm;
    }
}
```