# 安装python
```
windows： 去python官网下载
mac:      自带2.7版本
```

# 安装django
```
通过pip安装 pip install Django==1.10.2
或者通过下载源代码安装，进行源代码目录输入 python setup.py install
```

# 创建项目
```
django-admin startproject xxx项目名称
!!! 由于项目创建成功之后，项目中的一些配置项会默认使用项目名称做为一些配置，所以项目名称最好不要在进行修改
```

# 项目目录
```
wsgi.py (python服务器网关接口)
python应用与web服务器之间的接口

urls.py (url配置文件)
django项目中所以页面地址(页面)都需要自己去配置其url

settings.py (项目的总配置文件)
包含了数据库、web应用、时间等各种配置

__init__.py (声明模块的文件)
```

# 启动项目
1. 进入manage.py同级目录
2. python manage.py runserver [端口号] 默认8000

# 创建应用
1. 进入项目中manage.py同级目录
2. 输入 python manage.py startapp xxx应用名称
3. 添加应用名到settings.py中的INSTALLED_APPS里

# 应用目录
```
|
├──migrations                     数据迁移模块
|
├──__init__.py
|
├──admin.py                       当前应用的管理系统配置
|
├──apps.py                        该应用的一些配置
|
├──modules.py                     数据模块 使用ORM框架
|
├──tests.py                       自动化测试模块
|
├──views.py                       执行响应代码模块
```

# django 函数
```
Django url() 可以接收四个参数，分别是两个必选参数：regex、view 和两个可选参数：kwargs、name，接下来详细介绍这四个参数。
regex: 正则表达式，与之匹配的 URL 会执行对应的第二个参数 view。
view: 用于执行与正则表达式匹配的 URL 请求。
kwargs: 视图使用的字典类型的参数。
name: 用来反向获取 URL。
```

# templates
```
使用了Django模板语言（Django Template Language, DTL）
可以使用第三方模板（如Jinja2）
```
