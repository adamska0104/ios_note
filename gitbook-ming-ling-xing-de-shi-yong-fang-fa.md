
---
> **gitbook** 是一个基于 **Node.js** 的命令行工具，使用 markdown 语法，可以把你的Markdown文件汇集成电子书，并提供PDF等多种格式输出。你可以把gitbook生成的HTML发布出来，就形成了一个简单的静态网站。Gitbook还有一个同名的平台（gitbook.io），可以发布和销售电子书。

---
---
# 安装命令行 gitbook 流程
## 1. 安装 node
打开 https://nodejs.org/ 点击绿色的 INSTALL 按钮下载安装 node，npm会随着安装包一起安装。

可以查看node和npm是否安装成功

```
$ node -v
$ npm -v
```
## 2. 安装 gitbook 客户端
```
$ npm install gitbook-cli -g
```
  
--- 
# 使用命令行 gitbook 流程
## 1. 初始化 gitbook 项目目录
创建目录，切换到目录下，执行：
```
$ gitbook init
```
完成后会创建2个文件，**README.md** 和 **SUMMARY.md**
**README.md** 是对书籍的简单介绍
**SUMMARY.md** 是书籍的目录结构
如：
![image](/Users/mc/Downloads/1.png)

![image](http://gtms01.alicdn.com/tps/i1/TB1OwZ8JXXXXXbDXVXX_0dR.XXX-876-1228.png)

执行 gitbook init 会根据**SUMMARY.md** 目录生成对应的文件夹和 md 文件，每一个 md 文件对应每一章节，每一章节的内容在对应的 md 文件里编辑。
如果想要新增章节，可以在 SUMMARY.md 里面新增，然后执行 gitbook init 就会新增对应的 md 文件，原有文件不会变化；如果想要删除章节，在 SUMMARY.md 里面删除，然后执行 gitbook init 想要删除的 md 文件并不会删除，需要手动删除。

## 2. 创建电子书
```
$ gitbook build
```

## 3. 查看所创建的电子书
```
$ gitbook serve
```
浏览器预览 http://localhost:4000