原来的svn地址为外网ip，且是http，所以在配置方面一直没有出现过大问题，但这回应领导要求，改为https并且使用域名访问，

则出现了问题。

首先修改svn地址不难，具体如下：

![Alt text](https://raw.githubusercontent.com/hdlytoolazy/svn/master/raw/Screenshots/20171208103831.png)

修改完毕之后，svn上已存在的文件update和commit均无问题，但新文件的commit却始终报502。由于在变更地址前没有这种问题，

所以这里猜想是否与服务器https的配置有关。

功夫不负有心人，在运维同事小石头的努力下找到了问题所在（我只是抱着学习的态度把这个问题记录下来，解决人并不是我），

在nginx下增加这个配置就可以了：

![Alt text](https://raw.githubusercontent.com/hdlytoolazy/svn/master/raw/Screenshots/20171208105530.png)


原文地址：https://stackoverflow.com/questions/2479346/502-bad-gateway-with-nginx-apache-subversion-ssl-svn-copy