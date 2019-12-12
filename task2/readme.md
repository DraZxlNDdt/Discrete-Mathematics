# 编程任务2

由已知的真值表列写命题公式。

## 输入格式

在可执行文件所在目录下创建一个a.in文件,将输入数据写入a.in.

第一行 两个 正整数n 表示变元的个数

第二行 输入n个字符串，通过空格隔开，第i+1行表示第i个变元 的名称

接下来 2^n 行，每行1个数，通过空格隔开。对于第i+3行,考虑i的二进制形式，令此时i的第j位表示第j个变元的值，该行第j个数表示在这种情况下公式j的值。

## 输出格式

参考输出样例

## 输入样例

````
3
P Q R
1 0 0 1 1 0 1 1
````



## 输出样例

````
by True:
(┐P∧┐Q∧┐R)∨(P∧Q∧┐R)∨(┐P∧┐Q∧R)∨(┐P∧Q∧R)∨(P∧Q∧R)
by False:
(┐P∨Q∨R)∧(P∨┐Q∨R)∧(┐P∨Q∨┐R)

````



## 支持的数据范围

时间复杂度$O(2^n \times n)$
