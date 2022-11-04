#python django在线考试系统

#1，问题
没有账户信息：去找找model.py中的用户表代码
#2，运行
1，在pycharm中打开python django源码文件
2，编辑配置manage中，形参中输入：runserver 8000
3，在Navicat Premium15中创建数据库：djangoexam 字符集使用-utf-8mb4 排序规则默认
4，并运行sql导入数据库脚本djangoexam.sql也可以使用数据迁移命令
5，修改密码： DjangoExam文件夹下面的settings.py文件的84行修改'PASSWORD': 'eq10324'
6，调试manage.py文件，看看有没有需要安装的pyton模块。
7，在PyCharm中运行manage.py文件，浏览器打开地址：http://127.0.0.1:8000/即可
8，不迁移数据库，直接导入djangoexam.sql文件也可以


#3，测试账户信息
  学生id：20220727  密码：eq10324
  
#4，创建管理员后台账户
  管理员后台账户信息admin 123456

创建超级管理员命令：
    1.创建一个超级管理员，在控制台或者命令窗口输入如下命令:
     先cd进入程序目录 如 cd /d 目录
    python manage.py createsuperuser
    
    2.输入打算使用的登录名：
    username:admin
    
    3.输入email（这里输不输都不影响，直接回车也可以）：
    Email address:
    
    4.输入密码，需要输入两次，输入过程中密码不显示，密码要记住：
    Password:123456
    
    Password (again):
    
    5.当两次密码都相同的时候，就会提示superuser创建成功。:
    Superuser created successfully
    
    6.修改密码：
    python manage.py changepassword username
    
    7.运行服务：
    python manage.py runserver 127.0.0.1:8000 
    
    在浏览器打开：http://127.0.0.1:8000/admin/
