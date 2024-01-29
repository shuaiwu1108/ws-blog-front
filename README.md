# ws-blog-front
个人博客系统


## 开发与编译
### hexo命令的安装
> npm install hexo-cli -g

### 通过hexo初始化博客工程
> hexo init ws-blog-front  
cd ws-blog-front  
npm install  
hexo server  

### 安装fluid主题
> npm install -S hexo-theme-fluid

### 复制默认_config.yml配置，重命名为_config.fluid.yml

### 修改参数
> theme: fluid  
language: zh-CN

### 创建关于页
> hexo new page about  
修改关于页内容，在其中增加layout: about，以及书写正文

### 更新主题
> npm update -S hexo-theme-build

### 修改头部图片
> xxx.banner_img: /img/bg/example.png # 对应资源放在source下

## 通过Git Page发布
### 安装git插件
> npm install hexo-deployer-git --save

### 在_config.yml配置中，配置git仓库
> deploy:  
type: git  
branch: master  
repo: https://github.com/shuaiwu1108/ws-blog-deploy.git

### 部署
> hexo deploy

### 效果预览
![image](https://github.com/shuaiwu1108/ws-blog-front/assets/26000304/3f047d72-1dfe-452b-b799-9c026f5e7ae4)
