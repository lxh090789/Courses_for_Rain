# [流程控制](https://msdn.microsoft.com/zh-cn/library/ms174290(v=sql.120).aspx)

>用BEGIN END 包裹起来的语句称为语句跨。他们是同一级别的

>一个批处理段是由一个或者多个语句组成的一个批处理，之所以叫批处理是因为所有语句一次性被提交到一个SQL实例。在这个批处理范围内，局部变量是互相可见的。

>而想让多个语句分多次提交到SQL实例，则需要使用GO关键字。GO关键字本身并不是一个SQL语句，GO关键字可以看作是一个批处理结束的标识符，当遇到GO关键字时，当前GO之前的语句会作为一个批处理直接传到SQL实例执行。所以不在同一个批处理内局部变量不可见，也不可对跨批处理的语句使用流程控制语句.

![GO1](/img/4.png)

![GO2](/img/5.png)

### 1.顺序结构

>默认情况下语句是从往下依次顺序执行

### 2.分支结构（IF ELSE）

>IF (布尔表白式)
    语句块
>ELSE   （可缺省）
    语句块

![if](/img/3.png)

### 3.循环结构（WHILE /GOTO）

>由于sql 不像其他高级编程语言 。仅仅支持while 和goto

    <Code>
        while(表达式)
            语句块
    </Code>

>循环的break/CONTINUE/return 也可以使用

GOTO 标签

### 4.WAITFOR


>WaitFor delay 时间间隔
    语句段

WAITFOR DELAY 指定时间间隔后执行语句段


> WaitFor TIME 时间点
>   语句段

WaitFor TIME 指定的时间点后执行语句段
    