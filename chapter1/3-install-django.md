# 安装Python

Django运行依赖于Python环境，不同版本的Django对Python的版本要求不同，具体如下：

| Django版本 | Python版本 |
| :---: | :---: |
| 1.4 | 2.5，2.6，2.7 |
| 1.5 | 2.6，2.7 & 3.2，3.3 |
| 1.6 | 2.6，2.7 & 3.2，3.3 |
| 1.7 | 2.7 & 3.2，3.3，3.4 |
| 1.8 | 2.7 & 3.2（截止2016年底），3.3，3.4，3.5 |
| 1.9，1.10 | 2.7 & 3.4，3.5 |
| 1.11 | 2.7 & 3.4，3.5，3.6 |
| 2.0 | 3.5+ |

目前Django稳定版本已经到1.11，2.0版本就不再支持Python 2.x版本。本书基于Django 1.10版本，支持Python 2.7.x、3.4和3.5版本，教程中代码使用Python 3.4.3版本。

在**Linux系统**（Ubuntu、CentOS等）下，一般自带了Python环境，如果不是最新版本，你可以使用系统的包管理软件（apt-get、yum等）安装最新版本的Python。

在**windows系统**下，可以在[Python官网](https://www.python.org/download/)下载最新版本的Python。

在Python安装之后，可以通过下面的代码验证是否安装成功：

```
xianglong@ubuntu:~/blog$ python
Python 3.4.3 (default, Nov 17 2016, 01:08:31) 
[GCC 4.8.4] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

# 安装pip

pip是一个Python包的工具，Python安装包的工具有easy\_install，setuptools，pip，distribute等，使用这些工具都能下载并安装django。pip是easy\_install的替代品，在CPython解释器，PyPy解释器中都可以很好地管理Python包。

具体的安装方法这里不再一一介绍，不了解的可以参考：[pip安装方法](http://stackoverflow.com/questions/6587507/how-to-install-pip-with-python-3)

# 使用virtualenv

virtualenv是一个用来创建独立的Python开发环境的包。在实际项目开发中，不同项目可能使用不同版本的Python和Python Lib，使用virtualenv你可以非常容易地为每个项目建立地理的Python环境，然后安装项目所需的软件包到它们各自独立的环境中。

你可以使用pip安装virtualenv

```
sudo pip install virtualenv
```

安装之后，可以通过下面的命令来为你的项目创建独立的Python环境

```
virtualenv -p python3 blog
cd blog
. bin/activate    # 激活Python环境
```

# 安装数据库

Django支持许多不同的数据库服务器，目前主要有PostgreSQL，MySQL，SQLite和Oracle，除此之外Django还支持第三方的数据库Lib，比如MongoDB有mongokit。

为了使用数据库功能，需要安装其中一种数据库；不同的数据库需要不同的Python Lib支持：

| 数据库 | Python Lib |
| :---: | :---: |
| PostgreSQL | [psycopg2](https://pypi.python.org/pypi/psycopg2 "psycopg2") |
| MySQL | [python-mysqldb](http://stackoverflow.com/questions/4960048/python-3-and-mysql) |
| SQLite | Python自带 |
| Oracle | [cx\_Oracle](http://xianglong.me/article/ubuntu-install-python-cx-oracle-DistutilsSetupError/ "cx\_Oracle") |
| MongoDB | [mongokit](https://pypi.python.org/pypi/mongokit "mongokit") |

# 安装Django

### 稳定版

### 开发版

# 验证

Django安装之后，可以通过下面的代码验证，同时查看Django版本：

```
>>> import django
>>> print(django.VERSION)
(1, 10, 0, 'final', 1)
>>> 
```





