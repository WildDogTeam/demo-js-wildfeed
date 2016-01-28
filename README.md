# demo-js-wildfeed

利用野狗javaScript Sdk开发的类似的微博的社交应用。

## 实例

可以参考[wilddog demo](http://wildfeed.wilddogapp.com) 

[![一个demo页面的快照](screenshot.png)](http://wildfeed.wilddogapp.com/)

### 授权
```HTML
var wilddog = new Wilddog("https://wildfeed.wilddogio.com/");

// 监控登录状态的变化
var authClient = new WilddogSimpleLogin(chatRef, function(error, user) {
    if (error) {
        console.log(error);
    } else if (user) {
        console.log('User ID: ' + user.id + ', Provider: ' + user.provider);
    } else {
        // logged out
    }
});

authClient.login('qq');
```


## 本地运行

首先确认本机已经安装 [Node.js](http://nodejs.org/) 运行环境，然后执行下列指令：

```
git clone git@github.com:WildDogTeam/demo-js-wildpad.git
cd  demo-js-wildfeed
```

安装依赖：

```
npm install
```

启动项目：

```
gulp
```
或者使用ruby进行构建
```
bundle exec heel -p 3000 --no-launch-browser -r www/
```
## 更多示例

这里分类汇总了 WildDog平台上的示例程序和开源应用，　链接地址：[https://github.com/WildDogTeam/wilddog-demos](https://github.com/WildDogTeam/wilddog-demos)

## 支持
如果在使用过程中有任何问题，请提 [issue](https://github.com/WildDogTeam/demo-js-wildfeed/issues) ，我会在 Github 上给予帮助。

## 相关文档

* [wildfeed　ios版本](https://github.com/WildDogTeam/demo-ios-wildfeed)
* [Wilddog 概览](https://z.wilddog.com/overview/introduction)
* [JavaScript SDK快速入门](https://z.wilddog.com/web/quickstart)
* [JavaScript SDK 开发向导](https://z.wilddog.com/web/quickstart)
* [JavaScript SDK API](https://z.wilddog.com/web/api)
* [下载页面](https://www.wilddog.com/download/)
* [Wilddog FAQ](https://z.wilddog.com/faq/qa)


## License
MIT
http://wilddog.mit-license.org/

## 感谢 Thanks

We would like to thank the following projects for helping us achieve our goals:

Open Source:

* [firefeed](https://github.com/firebase/firefeed) Firefeed is a web app that lets users post small messages called sparks to their feed. You can follow other users, and their sparks will appear on your feed






