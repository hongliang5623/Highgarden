> * 创建一个项目
  python django-admin.py startproject mysite
> * 启动该项目
python manage.py runserver 10.0.0.110:8001
坑是，默认8000端口，然后使用IP怎么都无法访问，这样`指定`端口、IP也是醉了！
* python圈很小，看点API就敢说自己精通，最近看到厂里面招人，各种问我根本不会，压力山大呀！

### ubuntu使用django框架
```python
django-admin.py startproject mysite
Actually, if you use Ubuntu, it's just django-admin not django-admin.py 感觉好坑
```
> * 1.查看django版本：
python -c "import django; print(django.get_version())"
> * 2.__init__.py: 
一个空文件，告诉 Python 该目录是一个 Python 包
> * 3.安装ipython:
sudo apt-get install ipython
> * 4.安装pip: 
sudo apt-get install python-pip
> * 5.安装django： sudo pip install django 卸载sudo pip uninstall django
或者源码安装 https://github.com/django/django.git python install setup.py
> * 6 shell： Python manager.py shell 可以调试程序
