
# 问题 #
给定一个非负整数 num，反复将各个位上的数字相加，直到结果为一位数。。
# 代码 #
```C++

class Solution {
public:
    int addDigits(int num) {
   return 1 + (num - 1) % 9;
    }      
   
};
```
# 总结 #
0～9的结果就是0～9

10～19的结果是1、2、3 …… 9、1

20～29的结果是1、2、3 …… 9、1

可以发现，0属于特殊情况，后面每9个数字就一次循环，1～9一直循环下去，
结果=(num-1)%9 + 1