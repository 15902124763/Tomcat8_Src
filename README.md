tomcat官方网站给出的源码是需要ant编译的，用ant环境比较麻烦，这里给了maven编译，对应的tomcat的版本是8.5.41。  

第一步、从tomcat官网下载对应版本的源码地址：  

https://tomcat.apache.org/  

第二步、新建maven工程；  

第三步、添加maven依赖，具体的依赖可以从pom.xml中copy；  

第四步、从下载好的tomcat源码中拷贝文件夹到新建的maven工程中，需要拷贝的文件夹如下：  

1、bin、conf、modules、res、webapps、test以上这几个文件夹一定要放在工程的根目录下，其中java文件夹下的两个文件要copy到maven工程下的java路径下，这个一定要注意；  

2、比较特殊的是wabapps下的几个文件夹是tomcat给的demo可以只保留ROOT，其他几个可以删除，其他的文件如果不删除可能会报错但不影响tomcat的启动，报的错是类无法加载，因为缺少servlet的依赖。
