# 基本语法 Basic Syntax

#### 编码
默认情况下，Python 3 源码文件以 UTF-8 编码，所有字符串都是 unicode 字符串。

#### 标识符
* 第一个字符必须是字母或下划线
* 标识符的其他的部分由字母、数字和下划线组成
* 标识符对大小写敏感

#### 保留字
```python
>>> import keyword
>>> keyword.kwlist
['False', 'None', 'True', 'and', 'as', 'assert', 'async', 'await', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']
```


#### 注释
* 单行注释以 # 开头
* 多行注释可以用多个 # 号，还有 ''' 和 """

```python
#!/usr/bin/python3

# 第一个注释
# 第二个注释

'''
第三注释
第四注释
'''

"""
第五注释
第六注释
"""
print ("Hello, Python!")
```
#### 行与缩进
python最具特色的就是使用缩进来表示代码块，缩进的空格数是可变的，但是同一个代码块的语句必须包含相同的缩进空格数。

#### 多行语句
* 通常是一行写完一条语句，但如果语句很长，我们可以使用反斜杠( \ )来实现多行语句
* 在 [], {}, 或 () 中的多行语句，不需要使用反斜杠( \ )

#### 空行
函数之间或类的方法之间用空行分隔，表示一段新的代码的开始。类和函数入口之间也用一行空行分隔，以突出函数入口的开始。** 记住：空行也是程序代码的一部分。**

#### 同一行显示多条语句
同一行中使用多条语句，语句之间使用分号(;)分割

#### 多个语句构成代码组
缩进相同的一组语句构成一个代码块，我们称之代码组。像if、while、def和class这样的复合语句，首行以关键字开始，以冒号( : )结束，该行之后的一行或多行代码构成代码组。

我们将首行及后面的代码组称为一个子句(clause)。

#### import 与 from...import
* 在 python 用 import 或者 from...import 来导入相应的模块。
* 将整个模块(somemodule)导入，格式为： import somemodule
* 从某个模块中导入某个函数,格式为： from somemodule import somefunction
* 从某个模块中导入多个函数,格式为： from somemodule import firstfunc, secondfunc, thirdfunc
* 将某个模块中的全部函数导入，格式为： from somemodule import *

#### 命令行参数
Python可以使用-h参数查看各参数帮助信息
```
$ python -h
usage: python [option] ... [-c cmd | -m mod | file | -] [arg] ...
Options and arguments (and corresponding environment variables):
-b     : issue warnings about str(bytes_instance), str(bytearray_instance)
         and comparing bytes/bytearray with str. (-bb: issue errors)
-B     : don't write .pyc files on import; also PYTHONDONTWRITEBYTECODE=x
-c cmd : program passed in as string (terminates option list)
...
```
