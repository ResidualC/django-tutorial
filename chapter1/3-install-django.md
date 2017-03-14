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

在**windows系统**下，可以在[https://www.python.org/download/](https://www.python.org/download/) 下载最新版本的Python。

# 安装pip

pip是一个Python包的工具，Python安装包的工具有easy\_install，setuptools，pip，distribute等，使用这些工具都能下载并安装django。pip是easy\_install的替代品，在CPython解释器，PyPy解释器中都可以很好地管理Python包。

具体的安装方法这里不再一一介绍，不了解的可以参考：[http://stackoverflow.com/questions/6587507/how-to-install-pip-with-python-3](http://stackoverflow.com/questions/6587507/how-to-install-pip-with-python-3)

# 使用virtualenv



```
virtualenv -p python3 blog
```



# 安装数据库

# 安装Django

### 稳定版

### 开发版

# 验证



