#继续


#腾讯视频签到Github Action版

##今日签到

[ ![百度贴吧自动签到] ( https://github.com/bigoceans/TencentVideoAutoCheck/actions/workflows/main.yml/badge.svg ) ] ( https://github.com/bigoceans/TencentVideoAutoCheck/actions/workflows/main.yml ) 

##使用说明
###配置流程

1. Fork 本仓库，然后点击你的仓库右上角的Settings，找到Secrets，添加LOGIN_COOKIE 和 AUTH_COOKIE 两个变量。

2.设置好环境变量后点击你的仓库上方的` Actions `选项，第一次打开需要点击` I understand... `按钮，确认在 Fork 的仓库上启用 GitHub Actions 。

3. 任意发起一次commit，可以参考下文流程修改readme文件。

-打开` README.md `，点击修改按钮
-修改任意内容，这里在空格中插入了空格。位于最下面，点击提交。

4.至此自动签收就完毕了。

### login_cookie、auth_cookie的获取
1.网页登录腾讯视频

2.进入该网页：https://vip.video.qq.com/fcgi-bin/comm_cgi?name=hierarchical_task_system&cmd=2

3. F12 输入document.cookie然后回车，得到全部信息就是login_cookie；
4. auth_cookie是login_cookie的一部分，找到login_cookie中内容为` vqq_vusession= `的地方，将等号之后的内容全部删掉。之前的全部内容就是auth_cookie了。
5.获取配置信息的效果图如下：
![获取配置信息] ( https://github.com/bigoceans/TencentVideoAutoCheck/blob/main/img/1.jpg?raw=true )

###配置工作流执行信息写入run.log
1.仓库顶部设置
![配置workflow执行信息写入run.log ] ( https://github.com/bigoceans/TencentVideoAutoCheck/blob/main/img/2.jpg?raw=true )

![配置workflow执行信息写入run.log ] ( https://github.com/bigoceans/TencentVideoAutoCheck/blob/main/img/3.jpg?raw=true )

![配置workflow执行信息写入run.log ] ( https://github.com/bigoceans/TencentVideoAutoCheck/blob/main/img/4.jpg?raw=true )



