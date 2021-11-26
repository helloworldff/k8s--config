## 服务器信息收集和告警，已完成的功能比较简单，后期会继续优化。
### 简单的服务器监控：（基于python3.6和django2.1）
### 主要功能：
##### 1. 可以自主添加服务器，在服务器添加页面添加服务器的ip，端口，用户名，密码等信息。
##### 然后获取回去服务器的基础信息
##### 2. 获取服务器的基础信息显示在页面
##### 3. 告警页面,需要修改setting文件的邮箱配置，然后在告警设置页面
##### 写上接收邮件地址，告警设置.
### 运行：
##### 1. 拉取github代码:   git clone https://github.com/helloworldff/k8s--config
##### 2. 进入k8s目录，build镜像:    cd k8s && docker build --tag k8s-django -f k8s-dockerfile .
##### 3. 然后服务:  kubectl apply -f k8s-django.yaml
##### 4. 页面访问:  服务器IP+30800  即可