## 使用webpack4搭建基础环境，react、es6、scss处理
### . npm start启动程序
### . npm run build 打包
#### .在搭建过程中遇到的坑：<br/>
. 一、目前使用的是webpack4，单独提取css文件使用了extract-text-webpack-plugin，报错后查证此插件版本最新为3.x，不适应webpack4，
解决方案1：使用extract-text-webpack-plugin@next安装，2：替换为mini-css-extract-plugin;<br/>
. 二、使用babel编译es6代码提示解析报错:Cannot find module '@babel/core',排查后发现babel升级到7.x有坑，将babel-core替换为@babel/core，
babel-preset-env替换为@babel/preset-env
