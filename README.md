# mpx云开发示例

此实例是按tcb的blog demo做的。仅为演示mpx里如何使用小程序的云开发能力。


## 使用

> 注意：云开发要求一定要有appid，不可以是测试号

首先clone本项目，安装依赖，编辑project.config.json修改appid。

还需要到functions/addblog文件夹下安装依赖。

npm run watch启动开发。

开发者工具上选择云开发，创建环境blog-demo（此处随意），会生成一个envid。这个环境下再创建一个数据库集合取名blog。

搜索代码中todo备注的要修改的env，换成刚刚你生成的那个envid。

开发者工具中编辑器里，选中functions文件夹，右键上传并部署。

## 备注

此项目在标准脚手架模板上做了一些改动，正式的解决方案在思考是否提供多套脚手架模板。

改动主要是在build/build.js中，增加了对functions文件夹的复制。

另，本项目暂时不支持跨小程序平台构建。
