### Wildfeed

###利用野狗javaScript Sdk开发的类似的微博的社交应用。

###[演示地址](http://wildfeed.wilddogapp.com/)　

### 授权
```HTML
var wilddog = new Wilddog("https://wildfeed.firebaseio.com/");

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
你可以可以使用ruby进行构建
```
bundle exec heel -p 3000 --no-launch-browser -r www/
```

## 支持
如果在使用过程中有任何问题，请提 [issue](https://github.com/WildDogTeam/demo-js-wildfeed/issues) ，我会在 Github 上给予帮助。

## 相关文档

* [Wilddog 概览](https://z.wilddog.com/overview/guide)
* [JavaScript SDK快速入门](https://z.wilddog.com/web/quickstart)
* [JavaScript SDK 开发向导](https://z.wilddog.com/web/guide/1)
* [JavaScript SDK API](https://z.wilddog.com/web/api)
* [下载页面](https://www.wilddog.com/download/)
* [Wilddog FAQ](https://z.wilddog.com/faq/qa)


## License
MIT
http://wilddog.mit-license.org/

## 感谢 Thanks

We would like to thank the following projects for helping us achieve our goals:

Open Source:

* [firefeed](https://github.com/firebase/firefeed)






