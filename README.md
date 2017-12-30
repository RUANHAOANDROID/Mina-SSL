# Mina-SSL

[web https demo](https://github.com/RUANHAOANDROID/SpringBootDemo)

server demo

client demo

Android demo(跟进中...)


## 双向认证创建证书过程
1.创建服务端证书serverkey.jks

2.从服务端证书导出 server.cer

3.创建客户端jks clientkey.jks

4.从客户端导出cer client.cer

5.把server.cer 导入到clienttrust.jks

6.把client.cer 导入到servertrust.jks

### Android

7.把client.jks 转换为 aclient.bks

8.把clienttrust.jks转换为aclienttrust.bks

## BC库注意事项

/Library/Java/JavaVirtualMachines/jdk1.8.0_111.jdk/Contents/Home/jre/lib/security

该路径下配置Java.security文本 更改RSA 适配相应size、配置bc库



## 参考

[mina 官方文档](http://mina.apache.org/mina-project/userguide/ch2-basics/sample-tcp-client.html)

[Java Secure Socket Extension (JSSE) Reference Guide](https://docs.oracle.com/javase/8/docs/technotes/guides/security/jsse/JSSERefGuide.html#SSLContext)

[Netty使用JSSE实现SSLSocket通信](https://segmentfault.com/a/1190000010054860)

[Mina使用SSL结合android客户端SSL](http://blog.sina.com.cn/s/blog_49b531af0102v5g8.html)

[portecle使用文档](http://portecle.sourceforge.net/howtos.html)


[KEYTOOL和PORTECLE介绍](http://alanzhang.me/2014/12/31/KEYTOOL%E5%92%8CPORTECLE%E4%BB%8B%E7%BB%8D/)

[portecle使用教学视频](https://www.youtube.com/watch?v=nSqKv7VlMcg)

[openssl](https://www.openssl.org/docs/manmaster/man1/openssl.html)
