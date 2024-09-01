### Step
```
1、编写代码：app文件夹里面编写好你的代码 
2、本地测试：本地你可以生成一些测试输入放到tcdata里面（tcdata文件夹和app文件夹同级），运行run.sh里面的run on my workstation可以正常生成output的内容 
3、构建docker：build.sh run.sh里面保留第七行和14行 
4、线下进入容器测试，容器就类似一个新机器（sudo docker run -it --platform linux/amd64 -v ./tcdata:/tcdata 镜像地址 bash ），容器内app文件夹下生成output.zip文件即可 
5、push确认无误的镜像 
6、线上提交 
