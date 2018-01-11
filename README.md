# My-Learn-Note
This is my study notes, the basic daily updates, the main record daily learning content, come on!


### 2018.1.11 星期四 明日天气 -1° ~ -6°

> ## Express##
>
> 基于Node.js 平台，快速、开放、极简的 web 开发框架。

下载地址： `$ npm install express —save`

* 使用方法  

```javascript
// 1. 引入 expressconst 
Express = require('express')

// 2. 实例化 express
const app = Express()

app.get('/',(req,res)=>{    
res.send('链接成功');
})

//设置静态资源目录
app.use(Express.static('public'))

app.listen(3000,()=>{//默认习惯监听3000
console.log('server running in http://localhost:3000')
}) 
```







> ## 上传文件夹到服务器

` (终端处于文件夹上层目录) $ scp -r 文件夹 @rootIP地址:/root/服务器文件`

* 例如：  scp -r myFile @140.142.155.246:/root/myFirstFile

__注意：端口号不能重用__





> ## PM2
>
> Node服务器端管理工具

下载地址： `$ npm install pm2 -g `



* 常用命令:
  * $ pm2 start app.js # 启动app.js应用程序
  * $ pm2 list # 列表 PM2 启动的所有的应用程序
  * $ pm2 logs # 显示所有应用程序的日志
  * $ pm2 stop all # 停止所有的应用程序
  * $ pm2 restart all # 重启所有应用
  * $ pm2 delete all # 关闭并删除所有应用
  * $ pm2 save # 保存当前应用列表



>## node.js event事件



```javascript
const Event = require('events')

// es6 创建类 继承与 EventEmitter
class MyEvent extends Event{}

let event = new MyEvent()

let even = () => {
    Event.bind(even);
    console.log(this)
}

// on 监听器 listeners
event.on('suibian',even);
// emit触发器
event.emit('suibian')

//当触发 xxx时 做什么事 xxx代表事件类型 触发代表 emit 做什么事代表监听器
```



#### Node.js中文网API

> 大多数 Node.js 核心 API 都采用惯用的异步事件驱动架构，其中某些类型的对象（触发器）会周期性地触发命名事件来调用函数对象（监听器）
>
> 所有能触发事件的对象都是 `EventEmitter` 类的实例。 这些对象开放了一个 `eventEmitter.on()` 函数，允许将一个或多个函数绑定到会被对象触发的命名事件上。 事件名称通常是驼峰式的字符串，但也可以使用任何有效的 JavaScript 属性名。
>
> 当 `EventEmitter` 对象触发一个事件时，所有绑定在该事件上的函数都被同步地调用。 监听器的返回值会被丢弃。



> ## Homework

* 利用HEXO+Github搭设自己的blog
  *  [HEXO+Github,搭建属于自己的博客](https://www.jianshu.com/p/465830080ea9)
* 每天一道面试题
  * [2018前端校招总结](https://segmentfault.com/a/1190000011635556#articleHeader8)
* 完成socket.io聊天室
  * [雷哥的聊天室](http://140.143.155.246:8080/123)
* 周一考试
  * [考试题](http://www.jianshu.com/p/6a74ef2bdb03)





























#####   

###### 














