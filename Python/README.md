# Example Code

### Class

```
class Animal(object):
    __localtion = 'Asia'
    def __init__(self, name, age):
        self.name = name
        self.age = age

    @classmethod
    def set_localtion(cls, localtion):
        cls.__localtion = localtion

    @classmethod
    def get_localtion(cls):
        return cls.__localtion

```

---
### 繼承class

```
class Person(object):
    def __init__(self,name,gender):
        self.name = name
        self.gender = gender

class Teacher(Person):
    def __init__(self, name, gender, course):
        super(Teacher,self).__init__(name, gender)
        self.course = course
        
        
teacher = Teacher("Tim","male","math")

print(teacher.gender)
```
---
### isinstance()

```
​s = 'this is a string.'
n = 10
isinstance(s, int) # ==> False
isinstance(n, str) # ==> False
```

isinstance() 也能來判斷class
```
isinstance(p, Person)
```
---

### getattr() 和 setattr()

* type()函數，可以獲得變量的類型。
* dir()方法，可以獲取變量的所有屬性

```
class Person(object):
    def __init__(self, name, gender):
        self.name = name
        self.gender = gender

class Student(Person):
    def __init__(self, name, gender, score):
        super(Student, self).__init__(name, gender)
        self.score = score  

p = Person('Alice', 'Female')

setattr(p, 'age', 10) # 设置新的age属性

print(getattr(p, 'age') )

print(getattr(p, 'age', 20))

getattr(s, 'age', 20) # 获取age属性，如果属性不存在，就返回默认值20：

```
---

### Class的特殊用法
```
__len__、__str__、__repr__
當使用str()時，實際調用的是__str__()方法，而直接輸入變量，調用的是__repr__()方法。
```
```
__add__、__sub__、__mul__、__truediv__(除法)、__floordiv__ (除法取整數)
```

```
>>> num = 5
>>> num.__truediv__(3)
1.6666666666666667
>>> num.__floordiv__(3)
1 # 向下取整
>>> num = 7
>>> num.__floordiv__(3)
2
```
```
__slots__ = ('name', 'gender', 'score') 限定Student類的屬性
class Student(object):
    __slots__ = ('name', 'gender', 'score')
    def __init__(self, name, gender, score):
        self.name = name
        self.gender = gender
        self.score = score
```
---

### \_\_call\_\_
```
class Person(object):
    def __init__(self, name, gender):
        self.name = name
        self.gender = gender

    def __call__(self, friend):
        print('My name is {}...'.format(self.name))
        print('My friend is {}...'.format(friend))
        

p = Person("Tim","male")
p("Jake")
```
---

## Python_section
* [python 需要避免的三件事](https://blog.chairco.me/posts/2017/07/3%20mistakes%20to%20avoid%20when%20learning%20to%20code%20in%20Python.html)
* [python 深淺複製](https://ithelp.ithome.com.tw/articles/10221255)

```
<	__LT__(SELF, OTHER)
>	__GT__(SELF, OTHER)
<=	__LE__(SELF, OTHER)
>=	__GE__(SELF, OTHER)
==	__EQ__(SELF, OTHER)
!=	__NE__(SELF, OTHER)
```
---

