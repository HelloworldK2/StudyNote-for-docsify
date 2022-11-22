### Java基础

#### <div class = "a">命名规则</div>

##### 1. 小驼峰命名法：方法、变量
- 标识符是**一个单词**的时候全部小写，如：`name` 
- 标识符由**多个单词组成**的时候，第一个单词首字母小写，其他单词首字母大写，如：`firstName`

##### 2. 大驼峰命名法：类名
1.标识符是**一个单词**的时候，首字母大写，如：`Student`  
2.标识符由**多个单词组成**的时候，每个单词的首字母大写，如：`GoodStudent`

#### <div class = "a">强制转换</div>
把取值范围大的数赋值给取值范围小的变量。
```java
double a = 12.3;
int b =  (int) a
```
其中"+="、"-="、"*="、"/="、"%="的底层都隐藏了一个强制类型转换，如：
```java
short s = 1;
s += 1;
等于
s = (short)(s + 1);
```
**byte，short，char类型参与计算时会转换为int类型运算。**

#### <div class = "a">字符串</div>
在ASCII中，"a"为97，"A"为65。
字符串左右两边相加会输出字符串，字符与数字相加会使用相应的ASCII码相加，如：
```java
"123"+ 123 == 123123;
1+2+"123" == 3123;
'a'+ 3 == 100;
'a'+"abc" == aabc;
```
