# corivsky

假设盘子总数为奇数，目标从1移到3号柱。
奇数盘 移动顺序循环是 1->3 3->2 2->1
偶数盘                              1->2 2->3 3->1

第n步是几号盘第几次移动？
假设最上方1号盘，往下增大。

n%2=1  1号盘 第  n/2+1 次移动
n%2=0 （n/2）%2=1 2号盘 第（n/2/2）+1次移动
以此类推

根据奇数盘偶数盘以及移动次数对3取余，可以算出是几号柱子到几号柱子
————————————————
版权声明：本文为CSDN博主「逆向菜鸟」的原创文章，遵循 CC 4.0 BY-SA 版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/corivSky/article/details/101264712