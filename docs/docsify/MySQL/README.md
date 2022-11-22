### MySQL基础

#### <div class = "a">定义类型</div>

##### 1. `DECIMAL`

依赖于M（精度）和D（标度）的值，小数值（精确定点数）  
**例如：123.45（精度为5，标度为2)**

##### 2. 定义无符号数值类型
```sql
age TINYINT UNSIGNED
```
注：有符号为SIGNED

##### 3. `DOUBLE`类型
```sql
score DOUBLE(4,1)
```
注：4为总位数，1为小数位数

##### 4. `BLOB`类型
二进制形式的长文本数据（含TINY、MEDIUM、LONG类型）

##### 5. `TEXT`类型
长文本数据（含TINY、MEDIUM、LONG类型）

##### 6. `CHAR`类型
定长字符串，比如char(10)，使用时性能好

##### 7. `VARCHAR`类型
可自动适应长度存储字符串，性能较差

#### <div class = "a">字段操作</div>

##### 1. 添加字段
```sql
ALTER TABLE 表名 ADD 字段名 类型(长度)[COMMENT 注释][约束];
```
##### 2. 修改数据类型
```sql
ALTER TABLE 表名 MODIFY 字段名 新数据类型(长度);
```







