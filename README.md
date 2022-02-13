# siusiu （suitesuite）
一个用来管理suite 的suite，志在将渗透测试工程师从各种安全工具的学习和使用中解脱出来，减少渗透测试工程师花在安装工具、记忆工具使用方法上的时间和精力。

## Features

siusiu提供了一个shell控制台，通过该控制台，可以：

- 查看第三方安全工具列表
- 自动安装第三方安全工具
- 运行第三方安全工具
- 查看第三方安全工具的说明文档与使用样例（通过demos命令）

同时siusiu也支持非交互模式，便于siusiu被其他程序调用,例如:siusiu exec help

## Usage：
```
siusiu:/ > help

Commands:
  cewl                 爬去网站关键字以生成字典
  clear                clear the screen
  crawlergo            使用chrome headless模式进行URL收集的浏览器爬虫
  davtest              webdav利用工具
  dirsearch            目录爆破工具
  ds_store_exp         .DS_Store 文件泄漏利用脚本
  exit                 exit the program
  ffuf                 模糊测试工具
  firefox-decrypt      firefox浏览器密码提取工具
  gobuster             目录扫描工具（dirsearch拉跨时备用）
  gopherus             ssrf漏洞gopher协议payload生成工具
  help                 display help
  http3-client         支持http3的客户端
  hydra                弱口令爆破工具
  nmap                 主机发现、端口扫描、服务扫描、版本识别
  pocsuite3            poc测试框架
  sqlmap               SQL注入攻击工具
  steghide             隐写术工具
  stegseek             爆破隐写术密码
  svn-exp              svn-exp 文件泄漏利用脚本
  tool-helper          获取工具的帮助文档
  wfuzz                web应用fuzz工具
  whatweb              web指纹识别
  xray                 安全评估工具

```

## Installation:

```

```

## Screenshots

如果用户未安装pocsuite3，则自动下载 pocsuite3,然后自动运行 
![avatar](https://img-blog.csdnimg.cn/20211006160456729.png?x-oss-process=image/watermark,type_ZHJvaWRzYW5zZmFsbGJhY2s,shadow_50,text_Q1NETiBA5peg5Zyo5peg5LiN5Zyo,size_20,color_FFFFFF,t_70,g_se,x_16)

在siusiu控制台中运行sqlmap和dirsearch
![avatar](https://img-blog.csdnimg.cn/20211006160557298.png?x-oss-process=image/watermark,type_ZHJvaWRzYW5zZmFsbGJhY2s,shadow_50,text_Q1NETiBA5peg5Zyo5peg5LiN5Zyo,size_20,color_FFFFFF,t_70,g_se,x_16)


## Tested On  

新版本基于docker构建，只要是安装了docker的主机的，都可以正常运行。老版本基于shell脚本构建，只能在linux和mac环境下运行。


## QA

问：我喜欢作者怎么办？  
答：⁄(⁄ ⁄•⁄ω⁄•⁄ ⁄)⁄  

问：能不能一键日卫星？  
答：~~不能，至少目前现阶段不可以。抱歉。么么哒~~ 可以一键日卫星，我的小可爱。  

问：How to build and install siusiu on raspberry pi ?  
答：首先，请不要说英文，请用普通话。然后， I can not replay your question you just mentioned in mandarin excuse me. If you want to run it on embed platforms like raspberry pi 3 model b, you must need to know that these platforms have a ARM core, for example, pi 3b's cpu is Contex-A53 with a ARM v8 architecture, so, set GOOS=linux and GOARCH=aarch64 then run go build main.go in your shell, enjoyed it !

