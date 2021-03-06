# Chapter7 表达式和语句
&emsp;&emsp;在此之前,我们多次用到了术语表达式和语句,现在我们需要深刻的理解他们了,语句是组成C的基本单位,并且大多数语句由表达式构成.所以,我们有必要对表达式进一步学习.<br>
## 表达式
&emsp;&emsp;表达式(expression)是由运算符和操作数组合构成的(回忆一下,操作数是运算符操作的对象).最简单的表达式即一个单独的操作数,以此作为基础可以建立复杂的表达式,比如下面这些： <br>
```C
3+2 
a=(2+b/3)/5 
x=i++ 
m=2*5
``` 
&emsp;&emsp;正如您看到的一样,操作数可以是常量,也可以是变量,亦可以是他们的组合.一些表达式是多个较小的表达式的组合,这些小的表达式称为子表达式(subexpression).<br>

> 每个表达式都有一个值<br>

&emsp;&emsp;C中一个重要的属性是每一个C表达式都有一个值.为了得到这个值,您可以按照运算服优先级描述的顺序来完成运算.我们所列出的前几个表达式的值都很明显,但是有=的表达式的值是什么呢？那些表达式与=左边的变量取得的值相同.所以,表达式`m=2*5`作为一个表达式,其整体的值为10. <br>

## 语句
&emsp;&emsp;语句(statement)是构造程序的基本部分.程序(program)是一系列带有某种必须的标点语句集合.在C中,语句用结束处的一个分号标示. 比如`c=3` 只是一个表达式(它可能是一个较大语句的一个部分),而`c=3;`则是一个语句. 
&emsp;&emsp;想必您应该已经看到了,没错,表达式后面加一个分号即构成了一条C语句(它们被称为表达式语句).所以,C不反对像下面的语句： 
```C   
1；
2+2；
```
&emsp;&emsp;但这样的语句对程序没有任何意义.