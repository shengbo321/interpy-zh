# **kwargs 的用法

```**kwargs``` 允许你将不定长度的键值对, 作为参数传递给一个函数. 如果你想要在一个函数里处理已命名的参数, 你应该使用```**kwargs```. 这里是个让你上手的例子:

```python
def greet_me(**kwargs):
    for key, value in kwargs.items():
        print("{0} == {1}".format(key, value))


>>> greet_me(name="yasoob")
name == yasoob
```

那你可以看出我们怎样在一个函数里, 处理了一个键值对参数. 这就是```**kwargs```的基础, 而且你可以看出它有多么管用. 接下来让我们谈谈关于你如何使用```*args``` 和 ```**kwargs```来调用一个参数为列表或者字典的函数.