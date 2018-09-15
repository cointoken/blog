
Blog 基于flask(从Blog_mini派生而来)

python版本: 2.6-2.7 </br></br>
ubuntu部署</br>
</br>
一、虚拟环境部署(以pipenv为例)</br>
&nbsp;&nbsp;&nbsp;&nbsp;1、安装pip install pipenv </br>
&nbsp;&nbsp;&nbsp;&nbsp;2、pipenv shell</br></br>

二、安装包</br>
&nbsp;&nbsp;&nbsp;&nbsp;pip install -r requirements/common.txt</br></br>
   
三、安装python的mysql库</br>
&nbsp;&nbsp;&nbsp;&nbsp;apt-get install python-dev libmysqlclient-dev</br>
&nbsp;&nbsp;&nbsp;&nbsp;pip install MySQL-python</br></br>

四、创建mysql数据库</br>
&nbsp;&nbsp;&nbsp;&nbsp;mysql-u root -p</br>
&nbsp;&nbsp;&nbsp;&nbsp;create database blog_mini default character set utf8 collate utf8_general_ci;</br></br>

五、创建数据库环境变量</br>
&nbsp;&nbsp;&nbsp;&nbsp;export DATABASE_URL=mysql://root:123456@127.0.0.1/blog_mini</br></br>

六、初始化默认数据</br>
&nbsp;&nbsp;&nbsp;&nbsp;python manage.py deploy product </br>
