## chrome无法访问github.com
##### 解决方案：
方案一：
1）访问https://github.com.ipaddress.com/www.github.com  获取github.com 的IP地址
2）复制 如：123.82.112.4   github.com 到 C:\Windows\System32\drivers\etc中的 host文件中（以防出错，拷贝到其他路径下进行修改）
3）cmd运行ipconfig/flushdns刷新DNS网络配置。

    P.S. host文件位置：
    windows系统的hosts文件的位置如下：C:\Windows\System32\drivers\etc\hosts
    mac/linux系统的hosts文件的位置如下：/etc/hosts

方案二:
拷贝一下内容到host文件：
151.101.184.133    assets-cdn.github.com
151.101.184.133    raw.githubusercontent.com
151.101.184.133    gist.githubusercontent.com
151.101.184.133    cloud.githubusercontent.com
151.101.184.133    camo.githubusercontent.com
151.101.184.133    avatars0.githubusercontent.com
199.232.68.133     avatars0.githubusercontent.com
199.232.28.133     avatars1.githubusercontent.com
151.101.184.133    avatars1.githubusercontent.com
151.101.184.133    avatars2.githubusercontent.com
199.232.28.133     avatars2.githubusercontent.com
151.101.184.133    avatars3.githubusercontent.com
199.232.68.133     avatars3.githubusercontent.com
151.101.184.133    avatars4.githubusercontent.com
199.232.68.133     avatars4.githubusercontent.com
151.101.184.133    avatars5.githubusercontent.com
199.232.68.133     avatars5.githubusercontent.com
151.101.184.133    avatars6.githubusercontent.com
199.232.68.133     avatars6.githubusercontent.com
151.101.184.133    avatars7.githubusercontent.com
199.232.68.133     avatars7.githubusercontent.com
151.101.184.133    avatars8.githubusercontent.com
199.232.68.133     avatars8.githubusercontent.com

OR尝试下面内容：
151.101.44.249 github.global.ssl.fastly.net
192.30.253.113 github.com
103.245.222.133 assets-cdn.github.com
23.235.47.133 assets-cdn.github.com
203.208.39.104 assets-cdn.github.com
204.232.175.78 documentcloud.github.com
204.232.175.94 gist.github.com
107.21.116.220 help.github.com
207.97.227.252 nodeload.github.com
199.27.76.130 raw.github.com
107.22.3.110 status.github.com
204.232.175.78 training.github.com
207.97.227.243 www.github.com
185.31.16.184 github.global.ssl.fastly.net
185.31.18.133 avatars0.githubusercontent.com
185.31.19.133 avatars1.githubusercontent.com
192.30.253.120 codeload.github.com





## chrome访问github.com速度慢甚至直接挂掉
#### 解决方案：

方法一：下载chrome插件--Github加速插件 地址1：https://www.conwen.cn/zd/3170.html  地址2：https://github.com/fhefh2015/Fast-GitHub
        打开扩展程序，将后缀为 .crx拖进并生效，刷新github.com （亲测有效！）
方法二： 打开cmd，输入ping github.com查看是否出现丢包（丢失情况100%）
        否--正常；是--无法访问的原因---则配置HOST文件---获取github.com和github.global.ssl.fastly.net的IP地址，配置进文件中，ipconfig/flushdns生效，刷新。
        
        
        
        
        
        































