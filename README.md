# UDG

##### iOS配置

首先需要在代码config.xml里面配置UDG 所需要的sheme，获取UDG的scheme需要到海尔UDG注册获取，具体配置参考[http://mdoc.haier.net/Dev-Guide/app-config-manual](http://mdoc.haier.net/Dev-Guide/app-config-manual)



##### API:

##### 初始化UDG 方法    init: 其中accountId是必须传递的参数，是UDG分配的。

var udg = api.require('UDG');</br>
udg.initUDG({
​    accountId:'xxxx',scheme:'xxxx',channel:'xxxx'
});



##### 设置用户Id: setUserId. 其中userId参数是业务系统的埋点标志

var udg = api.require('UDG');</br>
udg.setUserId({
​    userId:'xxxx'
});

##### 埋点事件：trackEvent,其中eventName是必须传的参数，事件名称

var udg = api.require('UDG');</br>
udg.trackEvent({

​    eventName:'xxxx'，

​    xxx:'xxx'

});

##### 设置页面元素：setpageVariable

var udg = api.require('UDG');</br>
udg.setpageVariable({
​    xxx:'xxxx'
});
