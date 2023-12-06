# PublishTool
C#（.net 7）开发的一个自动化部署程序，相比jenkins部署更简单，使用更方便<br>

项目包含客户端和服务端<br>
服务端是一个webapi应用，通过windows服务或者控制台方式运行在服务器上，支持发布文件的上传，命令行执行，程序启动时会自动添加端口防火墙白名单<br>
客户端是一个控制台程序，支持传入参数，执行具体的发布命令，编译项目，然后调用webapi的上传和命令接口来完成自动化部署操作<br>
配合bat的命令行脚本，只要双击脚本，就能自动完成程序的编译，上传，服务端应用的重启等操作<br>

命令行脚本如下：<br>
cd ..<br>
PublishTool.Client.exe --Name=quntool --Host=http://10.168.10.143:9600<br>
Name为需要发布的应用名称，Host为服务器程序的Ip和端口

界面截图如下:<br>
客户端：<br>
![image](https://github.com/xlf8255565/PublishTool/assets/6311878/5f1fac00-954a-4e26-aadf-ada109847d1f)

服务端：<br>
![image](https://github.com/xlf8255565/PublishTool/assets/6311878/20a98036-0f04-42a4-9d74-8769c4b6e9c9)
