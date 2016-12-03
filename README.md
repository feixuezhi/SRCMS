# 欢迎使用SRCMS·轻响应框架 V1.8正式版
**SRCMS**是专门为中小企业和互联网产品创业团队打造的应急响应中心网站建站框架。有了它，如今你可以像使用办公软件一样容易，为你的企业建立起美观完备的安全应急响应中心。
> * **项目维护:** Martin Zhou
> * **E-Mail**:1009465756@qq.com
> * **QQ交流群：**132108046
> * **最后更新日期：**2016-12-03

---
##免责说明
SRCMS仅为建站软件，任何使用本建站程序搭建的网站其运营的内容所产生的纠纷与本项目无关。 

---
##开源贡献说明
本项目欢迎所有Github开源社区的同学贡献改进代码，让我们一起将SRCMS做的越来越好！ 

---
##框架首次运行配置说明（！第一次使用前请您仔细阅读以下内容！）：
在进行下面的步骤之前，请您确保本地或服务器有运行PHP程序的环境（推荐环境:Apache+PHP5.0及以上[暂不能完美兼容PHP7]+MySQL），接下来您需要：

* 第一步：通过Github代码托管页面将项目源代码下载

* 第二步：在phpmyadmin建立一个名为srcms（可以自定义，但是请参照第四步，调整数据库连接设置）的数据库，然后将./DB目录下srcms.sql文件导入刚刚创建的数据库。

* 第三步：打开./Application/Common/Conf/config.php，按照文件中绿色注释文字的提示,填写网站找回密码、后台登陆报警所需要使用到SMTP服务的相关配置。

* 第四步：打开./Application/Common/Conf/db.php，按照实际情况调整本地数据库连接相关配置。

* 第五步：打开./Application/Admin/Controller/LoginController.class.php,修改第59行sendMail方法内初始值1009465756@qq.com为您自己的安全邮箱。配置完成后，每次管理员登陆后台，该邮箱都将会接收到登陆日志。

* 配置完成：基础配置全部完成，下面您就可以通过在浏览器内输入相应地址体验SRCMS（轻响应）了。后台默认管理帐号为admin/amdin。
---
##版本更新日志

#####2016-12-03（建议等级：推荐更新）
* **修复** 后台无法查看生成的工单
* **修复** 前端页面JS远程资源失效问题
* **修复** 前台用户密码修改设计缺陷（Issued By 藏形匿影）
* **优化** 多处代码提升二次开发可读性
* **新增** 安全工单模块中动态更新功能

#####2016-12-02（建议等级：推荐更新）
* **修复** 一处前台越权漏洞
* **修复** 前台验证码刷新无效问题
* **修复** 后台用户管理逻辑缺陷
* **新增** 用户密码存储加盐（Issued By 华软HRCMS团队）

#####2016-01-26
* **修复** 三处严重的前台个人中心安全问题(Issued By phithon)
* **修复** 富文本过滤不严格的问题(Issued By mramydnei)
* **修复** 后台漏洞审核BUG
* **修复** 关闭开发模式，防止报错显示敏感信息

#####2016-01-24
* **新增** 新版首页：简洁、大方、更为灵活，方便您建立有自己特色的安全应急响应中心
* **新增** 新版前台个人中心：支持支付宝账号的录入
* **新增** 前台礼品兑换功能：用户可以在前台兑换礼品
* **新增** 漏洞报告临时授权查看
* **新增** 安全工单系统：合并进入了快捷方便的安全工单系统，方便安全和开发部门对安全事件的响应
* **新增** 系统配置功能：通过后台配置修改网站标题等配置
* **新增** robots.txt：根目录下增加了robots.txt方便搜索爬虫抓取，同时防止敏感内容被获取
* **优化** 前端静态资源：网站打开更快
* **修复** 漏洞报告中富文本XSS问题(Issued By Ivan)
* **修复** 数据库gbk导致的编码问题(Issued By Del技术菜鸟)

#####2015-10-06
* **新增** 团队博客
* **新增** 后台登陆保护
* **新增** 首页贡献榜管理
* **新增** 漏洞报告分发
* **新增** 联系方式管理
* **修复** 首页前端样式按钮错乱(Issued By Blast)
* **修复** 前台注入安全问题
* **优化** 网站打开速度

---
##框架BUG提交说明
如果您在使用本框架或是二次开发中发现任何SRCMS的问题，都欢迎通过Github将问题issue给我。 

---
##二次开发帮助说明
如果您在二次开发SRCMS，搭建自己的安全应急响应中心时遇到问题，非常欢迎通过QQ或邮件咨询我：1009465756(@qq.com)

---
##致谢
在开发过程中，SRCMS参考借鉴了不少优秀的开源项目,在此向下面的开发者们致谢：

* [ThinkPHP](http://www.thinkphp.cn/)
* [ThinkAdmin](http://www.thinkphp.cn/code/1342.html) 
* [Bootstarp](http://www.bootcss.com/)