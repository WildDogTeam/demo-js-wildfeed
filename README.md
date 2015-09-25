Wildfeed

#利用野狗javaScript Sdk开发的类似的微博的社交应用。

###[演示地址](http://wildfeed.wilddogapp.com/)　

###　授权
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







