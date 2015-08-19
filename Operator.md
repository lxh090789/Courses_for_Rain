# [运算符](https://msdn.microsoft.com/zh-cn/library/ms174986.aspx)


<style>
    table {
        border-collapse:collapse;
    }
    table td, table th {
        border:1px solid #000000;
        padding:3px;
    }
        table th {
            background-color:#87c2f3;
        
        }
</style>


### 1.[算术运算符](https://msdn.microsoft.com/zh-cn/library/ms187716.aspx)



<table>
    <tbody>
        <tr>
            <th>运算符</th>
            <th>作用</th>
        </tr>
        <tr>
            <td>+</td>
            <td>加法运算(数值相加，字符串串联 时间类型也可以相加)</td>
        </tr>
        <tr>
            <td>-</td>
            <td>减法运算</td>
        </tr>
        <tr>
            <td>*</td>
            <td>乘法运算</td>
        </tr>
        <tr>
            <td>/</td>
            <td>除法运算，返回商</td>
        </tr>
                <tr>
            <td>%</td>
            <td>取模</td>
        </tr>
    </tbody>
</table>

> _/ (两个整形变量相除只返回商的整数部分,小数部分全部舍去)_

### 2.[逻辑运算符](https://msdn.microsoft.com/zh-cn/library/ms189773.aspx)

<table>
    <tbody>
        <tr>
            <th>运算符</th>
            <th>作用</th>
        </tr>

        <tr>
            <td>ALL</td>
            <td>如果一组的比较都为 TRUE，那么就为 TRUE。</td>
        </tr>
        <tr>
            <td>AND </td>
            <td>如果两个布尔表达式都为 TRUE，那么就为 TRUE。</td>
        </tr>
        <tr>
            <td>ANY </td>
            <td>如果一组的比较中任何一个为 TRUE，那么就为 TRUE</td>
        </tr>

        <tr>
            <td>BETWEEN  </td>
            <td>如果操作数在某个范围之内，那么就为 TRUE。 </td>
        </tr>

        <tr>
            <td>EXISTS </td>
            <td>如果子查询包含一些行，那么就为 TRUE。 </td>
        </tr>
        <tr>
            <td>IN  </td>
            <td>如果操作数等于表达式列表中的一个，那么就为 TRUE。</td>
        </tr>
        <tr>
            <td>LIKE  </td>
            <td>如果操作数与一种模式相匹配，那么就为 TRUE。</td>
        </tr>
        <tr>
            <td>NOT  </td>
            <td>对任何其他布尔运算符的值取反。  </td>
        </tr>
        <tr>
            <td>OR  </td>
            <td>如果两个布尔表达式中的一个为 TRUE，那么就为 TRUE。  </td>
        </tr>
        <tr>
            <td>SOME </td>
            <td>如果在一组比较中，有些为 TRUE，那么就为 TRUE。 (等同于Any) </td>
        </tr>
    </tbody>
</table>

### 3.[赋值运算符](https://msdn.microsoft.com/zh-cn/library/ms188343.aspx

### 4.[作用域解析运算符](https://msdn.microsoft.com/zh-cn/library/dd206995.aspx)

### 5.[按位运算符](https://msdn.microsoft.com/zh-cn/library/ms176122.aspx)

### 6.[集运算符](https://msdn.microsoft.com/zh-cn/library/ff848745.aspx)

> EXCEPT 从左侧输入查询返回非由右侧输入查询输出的非重复行。(差集)
> INTERSECT 返回由 INTERSECT 运算符左侧和右侧的查询都返回的所有非重复值。 (交集)
>  UNION 指定合并多个结果集并将其作为单个结果集返回。 （并集）如果没有指定ALL则会删除重复的行
>  

### 7.[比较运算符](https://msdn.microsoft.com/zh-cn/library/ms188074.aspx)

![比较运算符](/sql/1.png)