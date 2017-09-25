# python  基础教程

Python是一种解释型，面向对象，动态数据类型的高级程序设计语言。

python (2.7)实例：

    #!/usr/bin/python
    
    print "Hello ,World!"

python (3.0)实例：
    
    #!/usr/bin/python3
    
    print ("Hello ,World")
    

python 简介：

Python是一个高层次的结合了解释型，编译型，互动性和面向对象的脚本语言。Python的设计具有很强的可读性，相比其他语言经常使用英文关键字，其他语言的一些标点符号，它具有比其他语言更有特色语法结构。

  ·Python是一种解释型语言：这就意味着开发过程中没有了编译这么环节
  
  ·Python是交互式语言：这就意味着，你可以在一个Python提示符，直接互动执行写你的程序。
  
  ·Python是面向对象的语言：这就意味着Python支持面向对象的风格或代码封装在对象的编程技术。
 
  ·Python是初学者语言：Python对初级程序员而言，是一种伟大的语言，它支持广泛的应用程序开发，从简单的文件处理到www浏览器到游戏。
  
python的特点：

  ·易于学习：Python有相对较少的关键字，结构简单，和一个明确定义的语法，学习起来较为简单。
  
  ·易于阅读：Python代码定义的更清晰。
  
  ·易于维护：Python的成功在于它的源代码是相当容易维护的。
  
  ·广泛的标准库:python的最大优势之一是丰富的库，跨平台的。
  
  ·互动模式：互动模式的支持，你可以从终端输入执行代码并获得结果的语言，互动的测试和调试代码片段。
  
  ·可移植：基于其开放源代码的特性，Python已经被移植到许多平台。
  
  ·可扩展：如果你需要一段运行很快的关键代码，或者是其想要编写一些不愿开放的算法，你可以使用C或者C++完成那部分程序，然后从你的Python程序中调用。
  
  ·数据库：Python提供所有主要的商业数据库接口。
  
  ·GUI编程：Python支持GUI可以创建和移植到许多系统调用。
  
Python中文编码：

  当我们使用英文输入：“hello world”的时候输出没有问题，但是如果输入中文字符“你好，世界”就有可能存在中文编码问题。
  
  #!/usr/bin/python
  
  print "你好，世界";
  
  以上执行输出结果为：
  
  File "test.py", line 2
  SyntaxError: Non-ASCII character '\xe4' in file test.py on line 2, but no encoding declared; see              http://www.python.org/peps/pep-0263.html for details
  
  python中默认的编码格式是ascll格式，在没有修改编码格式时无法正确打印汉字，所以在读取中文时会报错。
  
  解决办法就是在开头加入 # -*- coding: UTF-8 -*- 或者 #coding=utf-8 就行了
  
  python (2.7)
  
  #!/usr/bin/python
  
  # -*- coding: UTF-8 -*-
  
  print "你好，世界";
  
  输出结果为:
  
  你好，世界
  
第一个Python程序：

  交互式编程：
  
  交互式编程：交互式编程不需要创建脚本文件，是通过Python解释器的交互式模式进来编写代码，Linux上你只需要在命令行中输入Python命令即可启动交互式编程，提示窗口如下：
  
  $ python
  Python 2.7.6 (default, Sep  9 2014, 15:04:36)
  
  [GCC 4.2.1 Compatible Apple LLVM 6.0 (clang-600.0.39)] on darwin
  
  Type "help", "copyright", "credits" or "license" for more information.
  
  >>> 

  在Python提示符中输入以下文本信息，然后按enter键查看运行效果：
  
  print "Hello,python"
  
  输出结果如下:
  
  Hello,python
  
  脚本式编程：
  
  通过脚本参数调用解释器开始执行脚本，直到脚本执行完毕。当脚本执行完成后，解释器不再有效。
  
  书写一个简单的Python脚本程序，创建以.py为扩展名。将 print "Hello,python"写至py文件中。
  
  假设你已经设置了Python解释器Path变量，使用以下命令行运行程序：
  
  Python test.py
  
  输出的结果：
  
  Hello,python 
  
python 表示符：

  在Python里：标识符由字母，数字，下划线组成。
  
  在Python中，所有表示符可以包含英文，数字以及下划线，但不能以数字开头。Python中的标识符是区分大小写的。
  
  以下划线开头的标识符是有特殊意义的，以单下划线开头_foo的代表不能直接访问的类属性，需要通过类提供的接口进行访问。不能用from xxx import *而导入
  
  以双下划线开头的__foo代表类的私有成员；以双下划线开头和结尾的——foo——代表Python里特殊方法专用的标识，如_init_()代表类的构造函数。
  
  Python可以同一行显示多条语句，方法是用分好；分开，如：
  
  >>> print 'hello';print 'runoob';
  hello
  
  runoob
  
Python 保留字：

  and	exec	not
  
  assert	finally	or
  
  break	for	pass
  
  class	from	print
  
  continue	global	raise
  
  def	if	return
  
  del	import	try
  
  elif	in	while
  
  else	is	with
  
  except	lambda	yield
  
  
