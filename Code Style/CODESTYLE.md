# Python代码规范

## 一、编码

### 1. 如无特殊情况，文件一律使用UTF-8编码

### 2. 如无特殊情况, 文件头部必须加入#-*-coding:utf-8-*-标识


## 二、命名规范

### 1. 变量和函数名应使用小写字母，单词之间使用下划线分隔，例如：my_variable。

### 2. 类名应使用驼峰命名法，首字母大写，例如：MyClass。

### 3. 常量应全部使用大写字母，单词之间使用下划线分隔，例如：MY_CONSTANT。

示例代码

```
my_variable = 10

def my_function():
    pass

class MyClass:
    pass

MY_CONSTANT = 100
```


## 二、缩进和空格

### 1. 使用4个空格进行缩进，不要使用制表符。

### 2. 在运算符和逗号后面加一个空格，例如：x = y + z。

### 3. 在逗号和冒号前面不加空格，例如：x, y = 1, 2。

### 4. 在注释符号(#)后面加一个空格。


示例代码

```
if x > 0:
    y = x * 2

numbers = [1, 2, 3, 4]

for number in numbers:
    print(number)

# This is a comment
```


## 三、行长度和换行

### 1. 每行代码不应超过79个字符。

### 2. 如果一行代码过长，可以使用括号或者反斜杠进行换行。

示例代码:

```
result = (number1 + number2 +
          number3 - number4)

result = number1 + number2 + \
         number3 - number4
```


## 四、空行

### 1. 在不同的函数、类和方法之间应插入空行，以提高代码的可读性。

### 2. 在函数或方法内部的相关代码块之间也应插入空行。

示例代码:

```
def function1():
    pass


def function2():
    pass


class MyClass:
    def method1(self):
        pass

    def method2(self):
        pass
```


## 五、导入规范

### 1. 导入应放在文件开头，每个导入语句应独占一行。

### 2. 导入应按照标准库、第三方库和本地库的顺序排列。

### 3. 不推荐使用通配符导入，应明确导入需要的模块。

示例代码:

```
import os
import sys

from math import sqrt

import my_module
```


## 六、注释规范

### 1. 注释应以英文句点结尾。

### 2. 注释应清晰地解释代码的功能和用途。

### 3. 长的注释可以使用多行注释。

示例代码:

```
# This is a comment

def calculate_square_root(number):
    """
    This function calculates the square root of a number.
    """
    return sqrt(number)
```


## 七、函数规范

### 1. 函数应尽量短小，每个函数只完成一个具体的任务。

### 2. 函数的参数应尽量少，避免使用过多的全局变量。

### 3. 函数应有明确的返回值。

示例代码：

```
def calculate_square_root(number):
    return sqrt(number)
```


## 八、异常处理规范

### 1. 在代码中应适当添加异常处理语句，以防止程序出现错误时崩溃。

### 2. 异常处理语句应尽量具体，避免使用通用的Exception类。

### 3. 可以使用try-except语句来捕获异常，并在except块中处理异常情况。

示例代码：

```
try:
    result = x / y
except ZeroDivisionError:
    print("Error: Division by zero")
```

