# 使用方法
1. 解压到网站根目录
2. 登录  你的域名/dmku 进行配置数据库  
3. 修改播放器后台密码  dmku/config.inc.php
4. 登录后台 你的域名/admin  密码为第3步修改的密码
5. 播放器功能可后台设置
6. 接口地址：域名/player/?url=

# 参数说明（player/index.php）
"av":'<?php echo($_GET['av']);?>',//B站av号，用于调用弹幕
"url":"<?php echo($_GET['url']);?>",//视频链接
"id":"<?php echo($_GET['url']);?>",//视频id
"sid":"<?php echo($_GET['sid']);?>",//集数id
"pic":"<?php echo($_GET['pic']);?>",//视频封面
"title":"<?php echo($_GET['name']);?>",//视频标题
"next":"<?php echo($_GET['next']);?>",//下一集链接
"user": '<?php echo($_GET['user']);?>',//用户名
"group": "<?php echo($_GET['group']);?>",//用户组

# 请求示例
#### 基本
https://bbtv.ml/player/?url=https://d.mahua-kb.com/20200615/4MSLOWqX/index.m3u8

#### 高级
除了 url 参数，其他都可以省略

https://bbtv.ml/player/?url=https://d.mahua-kb.com/20200615/4MSLOWqX/index.m3u8&next=https://d.mahua-kb.com/20200615/4MSLOWqX/index.m3u8&sid=1&pic=https://img.xx.com/1.png&user=游客&group=1&name=测试
