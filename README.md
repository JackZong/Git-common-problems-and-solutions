# Git 常见问题与解决办法
（方便自己以后遇到同样问题的时候查阅）

### 1. packet_write_wait connection to xx.xx.xx.xx Broken pipe   
### s：
  找到git安装的目录/etc/ssh，打开ssh_config文件
  ```
  sudo vim /etc/ssh/ssh_config 
  ```
  在其中修改（或者添加）
  ```
  Host *
  ServerAliveInterval 120
  ```
