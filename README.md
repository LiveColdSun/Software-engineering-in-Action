软件工程项目实践
====

预备知识 - -# 水平有限，仅供参考

### TOC

* [目录](#toc)
* [前端相关](#前端相关)
* [后端相关](#后端相关)
    * [参考资料](#参考资料)
    * [环境配置](#环境配置)
        * [windows](#windows)
        * [Linux & Mac OS X](#linux--mac-os-x)

===

### 前端相关

**HTML, CSS, Javascript** 是前端必须要掌握的知识。

HTML 是网页的基础， CSS 是网页的布局，首先要熟悉 HTML 标签和 CSS 属性，不断尝试练习各种不同的排版，总结技巧，必须要有规范。

HTML & CSS 熟悉之后可以学习 Javascript，从基本的 DOM 结构开始，然后就是各种 function，尝试自己去实现一些酷炫的效果。

**[w3schools](http://www.w3school.com.cn/)**  提供了许多学习材料。

**[Web Fundamentals](http://www.codecademy.com/tracks/web)** & **[Web Projects](http://www.codecademy.com/tracks/projects)** 提供了许多练习。

当你的 HTML/CSS/JS 掌握的差不多之后可以开始尝试下面的一些技术：

* **[Bootstrap 3](http://v3.bootcss.com/)**，Twitter 推出的一个开源的 HTML/CSS 框架，提供了优雅的 HTML/CSS 规范以及丰富的 Web 组件，可以极快的搭建一个酷炫的网页。

    Bootstrap 3 偏向扁平化的设计，[Bootstrap 2](http://v2.bootcss.com/) 偏向拟物化设计。
    
* **[JQuery](http://jquery.com/)**，很流行的 JS 框架，极大的简化了 DOM 操作，为网站提供了更方便的 Ajax 交互。

    [Codecademy JQuery](http://www.codecademy.com/tracks/jquery) 提供了基础的教程。

*  **[Ajax](http://en.wikipedia.org/wiki/Ajax_(programming\))**，一种支持异步请求的技术，用于创建更好更快以及交互性更强的 Web 应用的技术。

我觉得以上就是足够让我短时间内搭建一个还不错的 web 应用最快的方法。

浏览器的兼容性是前端开发者必须要重视的问题，同样的代码在 Chrome, FireFox, Safari, IE 下可能会有不同的表现。不过这个问题这次可以先不去考虑，以上提到的这些技术对传统的 IE ( 低于 IE 9 ) 并不能很好的支持，调试最好使用 Chrome/FireFox/Safari 或者 搜狗/360浏览器的 极速 模式。

**掌握 Chrome/FireFox 的调试方法能极大的提高开发效率。**

> 怎样成长为一个优秀的 Web 前端开发工程师？ \- [via 知乎](http://www.zhihu.com/question/19554845) 

> * 多写。很多问题都是积累得来的。写了，遇到了，才能去真正理解解决方案，才会随着自己的不断成长而有进步。别人问我为什么知道那么多 CSS 兼容解决方案，为什么一看就出的时候，我只能告诉他，我写了 20 几个 Wordpress 主题。-，-

> * 看书。看 BLOG 或者一些网上的教程，都很难让你全面理解一个东西的。坚持看书，至少前端相关的语言都看一本。

> * 读 BLOG。最后你会发现，很多东西大家都会。但只有某些人才解决得了某些细节性的东西，这些人就是我们所谓的高手。很大牛在 BLOG 不会写一些简单的 List, 而是针对某个问题深入研究。这时看 BLOG 对于进阶非常有帮助。

> * 去学一门后端语言。怎么说呢，实际用到会很少。但会很有利于一些问题的理解。比如 Ajax。还有 HTML5 中像 Web sockets、post message 之类的 API。

> * 去用很多产品，至少去爱一个产品。你不止是一个前端，你还应该是一个设计者，去用很多产品，你才会发现技术为什么有用，去爱一个产品，你才会把技术用得更好。

>   ...

===

### 后端相关

后端暂定使用 python 2.7.x + django 1.5.x

数据库暂定使用 mysql

#### 参考资料

* **[Google's Python Class](https://developers.google.com/edu/python/)** 两天速成 python，语法真的很简单。

* **[Django Book 中文版](http://djangobook.py3k.cn/2.0/)**  
* **[Django Book 英文版](http://www.djangobook.com/en/2.0/index.html)**

只需要前十章看完（或者只需要前七章）就足够可以完成本次的任务了。
当然 Django Book 只介绍了web开发最基础的部分，如果使用中有什么问题可以联系[我](mailto:xindervella@gmail.com)或者[姚育华](mailto:goclisyyh@gmail.com)，或者在 [Django 主页](https://www.djangoproject.com/) 查相关文档。


#### 环境配置

python 使用 2.7.5 ( 2.6.x 以上版本均可，不要尝试使用 python 3.x， 目前 django 还不支持 python 3.x)

##### windows 

* [Python 2.7.5 Windows Installer](http://www.python.org/ftp/python/2.7.5/python-2.7.5.msi) (Windows binary -- does not include source)
* [Python 2.7.5 Windows X86-64 Installer](http://www.python.org/ftp/python/2.7.5/python-2.7.5.amd64.msi) (Windows AMD64 / Intel 64 / X86-64 binary -- does not include source)


下载完成后打开CMD 输入 python 后显示类似如下即安装完成。

```python
Python 2.7.5 (default, Sep 18 2013, 13:30:00) 
[GCC 4.2.1 Compatible Apple LLVM 4.2 (clang-425.0.28)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```

然后安装 django

* [Django-1.5.5.tar.gz](https://www.djangoproject.com/download/1.5.5/tarball/)

下载完成后解压缩，CMD 切换到文件夹下：

`c:\django-1.5.5> python setup.py install`

完成后打开 CMD，看到如下输入不报错即完成

```python
C:\>python
Python 2.7.5 (default, Sep 18 2013, 13:30:00) 
[GCC 4.2.1 Compatible Apple LLVM 4.2 (clang-425.0.28)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> import django
>>> django.VERSION
(1, 5, 5, 'final', 0)
>>> 
```

##### Linux & Mac OS X

* Linux 和 Mac OS X 已经预装了 python 环境不需要再次安装。

使用 pip 安装 django

* `~$ sudo pip install django`
* 如果提示 pip 未安装 请使用 `~$ sudo easy_install pip` 安装完成后再使用 pip 安装 django

完成后打开 terminal，看到如下输入不报错即完成

```python
~: python
Python 2.7.5 (default, Sep 18 2013, 13:30:00) 
[GCC 4.2.1 Compatible Apple LLVM 4.2 (clang-425.0.28)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> import django
>>> django.VERSION
(1, 5, 5, 'final', 0)
>>> 
```

===

\- -# 今天就先写到这里，关于前后端的数据交互和web开发的相关概念我会慢慢补充上来。

