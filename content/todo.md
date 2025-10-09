---
title: Todo
---

- 鸿蒙OS
  - 为什么之前用粗粒度锁 简单改成细粒度就好了吗
- 如何让llm严格生成markdown

## QD

### 一面
	
- 问项目
- inline 有什么用处？
- inline 和普通函数有啥区别？
- Cpp 新功能？
- 用过模板吗？
- 有多线程编程经历吗？
- C/Cpp 怎么创建线程？
- malloc/new 有啥区别？
- 为什么选量化？
	
**coding** 实现一个 latency 的平均值和标准差统计，需要多线程吗（先不用），但是要求 on-line（新增和过期时）地更新
	
### 二面
	
- 编译流程？
- 智能指针区别？
- lambda 传值方式、缺点？
- 多线程了解吗？
- 金融知识了解多少？
- 有做过金融项目吗？
	
**场景题**
	
- 10w x 10w 的矩阵，并发访问（QPS 不大），如何建立线程模型？
- 一个 core dump 的程序，如何 debug？
- 如何定位并解决运行慢的问题？
- 给定一段时间的电梯运行和人流量数据，建立根据电梯行为进行人流量预测的模型。
- 大文件小内存求 unique 数量
	
### 线下终面
	
**一轮**
	
- static
- inline
- move 和 vector 拷贝构造移动构造，`A a = f()` vs `A a; a = f();`
- vector 扩容机制
- 堆栈区别，优劣
- array 怎么弄在堆上
- linux 死机 debug
- 怎么判断系统是大端还是小端
- 多线程、含参初始化 的 单例 的 实现：static 函数 + 计数器 + 指针
- 实现`vector<A>`的多线程析构
	
**二轮**
	
算法题
	
- 实现 itos，要求尽可能快
- n 个数 m 个划分，使 minmax 差值最小
	
**三轮**
	
工程题
	
- csv parser
- 斗地主模拟器

John has always dreamed of taking a vacation on Hawaii. He has decided to make his dream come true during the next holiday period, and he would like to spend as much time there as possible.
The problem is that there is only one plane per week connecting Hawaii with the city where John lives. The plane departs every Monday and arrives every Sunday. There is no other way to get to Hawaii and back. It means that John can spend only whole weeks in Hawaii.
John knows in which month his vacation starts and in which month it ends. His vacation period starts on the first day of the beginning month and ends on the last day of the ending month. John also knows the year in which his vacation takes place.
For example, if John's vacation lasts from July to September in 2008, then it starts on 1st July 2008 and ends on 30th September 2008.
Your task is to calculate how many weeks John will spend in Hawaii, given:
the month when the vacation begins;
the month when the vacation ends;
the year when the vacation takes place;
the day of the week for 1st January in the vacation year (for convenience).
The names of the days of the week are:
Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday
content_copy
. The names of the months are:
January, February, March, April, May, June, July, August, September, October, November, December
content_copy
. The lengths of the months are, respectively:
31, 28 (or 29 in a leap year), 31, 30, 31, 30, 31, 31, 30, 31, 30, 31
content_copy
days.
Pay attention to leap years; you should also consider them. The year of the vacation will be a number between 2001 and 2099, inclusive, and you can tell that the year is a leap year if it's divisible by 4.
Write a function:
int solution(int Y, string &A, string &B, string &W);
content_copy
that, given an integer Y and three non-empty strings A, B and W, denoting the year of the vacation, the beginning month, the ending month and the day of the week for 1st January of that year, returns the maximum number of weeks that John can spend in Hawaii.
For example, given Y = 2014, A = "April
content_copy
", B = "May
content_copy
" and W = "Wednesday
content_copy
", the function should return 7, since John can leave his city on April 7th and come back on May 25th, so he will spend 7 weeks on Hawaii (the weeks beginning, respectively, on April 7th, 14th, 21st, 28th and May 5th, 12th, 19th).
此处跟日历图
Assume that:
Y is an integer within the range [2,001..2,099];
A and B are valid month names;
month B does not preceed month A;
W is a valid weekday name;
W is the correct weekday for January 1st of year Y in the actual calendar.
In your solution, focus on correctness. The performance of your solution will not be the focus of the assessment.