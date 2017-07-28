# 流行框架
## ssh方式上传代码
1. 生成公钥和私钥
    * ssh-keygen -t rsa -C "youxinag"
2. 在用户目录下.ssh 中复制..pub文件内容，在GitHub中用户下找settings找ssh and g.. 点击新秘钥

## 下载
1. git pull ssh地址 master

## 处理冲突
   本地与服务器端的代码发生冲突时，根据需要删除不需要的代码

## 提交数据时先pull再push
    先pull时，如果服务器版本和本地不同，我们可以吧冲突先解决，然后把最新的版本push到服务器
