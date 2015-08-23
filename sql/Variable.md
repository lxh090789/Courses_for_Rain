# Sql 变量
### 声明

<code>
    DECLARE @variable_name DataType
</code>

##### 其中 *DECLARE* 为固定语法, *@variable_name* 为局部变量名称,注意这里必须用 @ 开头 ,*DataType* 为数据类型


#### 示例:
<code>
    DECLARE @deptName nvarchar(50);<br />
    DECLARE @Age int; <br />
    DECLARE @nowDate datetime;
</code>

### 赋值

> 变量已经声明,必须对变量赋值才有意义，变量赋值分为两种情况：

1. set @variable_name = value
2. select @variable_name = value  

> 其中select 赋值方式 可以从表，视图中获取数据 例如:

<code>
    select @variable_name = 字段名 from 表名或者视图 
</code>

当然 select 的后面可以跟from/where/group by 等语句