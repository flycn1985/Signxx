# Sign++网络验证系统

![logo](http://img0.ph.126.net/uUl-CxZ3kzPRi5U6EWuPXQ==/6632043032514045099.png)

## 开源原因

这是我个人开发的php网络验证系统，原本是想等用户多了寻找盈利模式的，无奈服务器费用积少成多而且用户一直不多，索性就把它开源了。

## 这个东西是干嘛的？

用途是给易语言和按键精灵所写的游戏脚本的进行收费管理，还有我配套开发的客户端dll动态链接库，用于脚本集成，[客户端demo下载](http://signxx.ys168.com/)。

## 详细功能介绍

服务端（php）介绍：

* 官网，用于展示、注册登录、忘记密码等；
* 后台网站，用户统计、软件管理、注册码管理、推荐人规则等功能；
* 供客户端调用的接口，请求数据使用rsa和des加解密，确保封包安全；

客户端（dll）介绍：

* 登录；
* 试用；
* 解绑；
* 离线；
* 推荐人加时；

## 客户端接口（供脚本调用）

```
----------------------------------------
 signxx_init
----------------------------------------
 功能:初始化
 参数:
    s  软件编号
    v  软件版本
 返回值:
    无
----------------------------------------
 signxx_reg
----------------------------------------
 功能:注册
 参数:
    code  注册码
 返回值:
    0=成功 -1=失败
----------------------------------------
 signxx_try
----------------------------------------
 功能:试用
 参数:
    无
 返回值:
    0=成功 -1=失败
----------------------------------------
 signxx_unbind
----------------------------------------
 功能:解绑
 参数:
    code  注册码
 返回值:
    0=成功 -1=失败
----------------------------------------
 signxx_check
----------------------------------------
 功能:校验
 参数:
    无
 返回值:
    0=成功 -1=失败
----------------------------------------
 signxx_offline
----------------------------------------
 功能:下线
 参数:
    无
 返回值:
    无
----------------------------------------
 signxx_getmsg
----------------------------------------
 功能:获取上一个函数返回的提示文字
 参数:
    无
 返回值:
    字符串
----------------------------------------
 signxx_recommend
----------------------------------------
 功能:推荐人加时
 参数:
    code  注册码
    recommendcode  推荐码
 返回值:
    0=成功 -1=失败
----------------------------------------

```

## 后台截图

![logo](http://img2.ph.126.net/Kck9QNwRtkY6ud670oG2SQ==/6631977061816373810.png)

![logo](http://img2.ph.126.net/mSt-J1V0yuVqpuei8opRWg==/6632018843258224193.png)

![logo](http://img2.ph.126.net/OfltlQQWUZj6JqLsbsE58g==/6631838523351277550.png)

![logo](http://img0.ph.126.net/MOqEiy5dGMV_iPcDcYkUqA==/6632093610048917631.png)

![logo](http://img2.ph.126.net/gk9hqTsF3zu8hi3Kxd2qYw==/6632080415909383718.png)

![logo](http://img0.ph.126.net/Z3yMMvC4sUUpmP2N_MJFcQ==/6631926484281493275.png)
