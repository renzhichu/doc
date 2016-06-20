1. 生成`ssh key`（windows系统使用git shell打开）：执行`ssh-keygen -t rsa -C "随便一个邮箱"`
2. 进入.ssh文件夹（linux在~/目录下，windows在C:\当前用户下）
3. 复制.ssh下面的id_ras.pub并重命名为你的名字全名，发送给我
4. 在.ssh文件夹下面建立一个config的文件（注意：没有后缀名），内容为
  ```
  Host 172.16.33.3
  HostName 172.16.33.3
  Port 9422
  User 你的名字
  IdentityFile ~/.ssh/id_rsa
  IdentitiesOnly yes
  ```
