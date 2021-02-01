输出hello world

```
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }
}
```

1. # Java中的关键字

![img](http://img.mukewang.com/53588ce900019bee05190178.jpg)

​		Java 关键字是**区分大小写**的！所以 void 是关键字，但 Void 就不是了

# 2.标识符

**标识符就是用于给 Java 程序中变量、类、方法等命名的符号**。

![img](http://img.mukewang.com/5358910f00018c2c07320199.jpg)

标识符**可以由字母、数字、下划线（_）、美元符（$)组成**，但**不能包含@，%，空格等其他的特殊符号**，**不能以数字开头**。

标识符不能用Java的关键字和保留字，但可以包含关键字和保留字。

标识符严格区分大小写。

标识符最好能反应其作用，做到见名知意。

# 3.变量

简单的说，我们可以把变量看作是个盒子，可以将钥匙、手机、饮料等物品存放在这个盒子中，也可以在需要的时候换成我们想存放的新物品。

在 Java 中，我们通过三个元素描述变量：**变量类型、变量名**以及**变量值**。

在 Java 程序中，我们可以根据所需要保存的数据的格式，将其保存在指定类型的变量空间中，并且通过变量名快速定位！（类比于客人住房间）

![img](http://img.mukewang.com/535a6c6000015cda02910139.jpg)



![img](http://img.mukewang.com/5358cb3400019b5606390263.jpg)



注意哦： **Java 中的标点符号是英文的**。譬如语句结束的分号，是英文符号的分号，千万别写成中文！

## 3.1 变量命名

如同酒店会给每个房间起个性化的名字一样，程序中的变量也需要用合理的名字进行管理---变量名！

在给变量起名字时，必须**符合一定的规则**

![img](http://img.mukewang.com/535a3ad60001057407870199.jpg)

错误分析

![img](http://img.mukewang.com/536887ea0001bf2004800148.jpg)

**优秀攻城师的习惯**：

1、变量名由多单词组成时，**第一个单词的首字母小写**，**其后单词的首字母大写**，俗称**骆驼式命名法**（也称驼峰命名法），如 myAge

2、变量命名时，尽量简短且能清楚的表达变量的作用，做到**见名知意**。如：定义变量名 stuName 保存“学生姓名”信息

PS： Java 变量名的**长度没有限制**，但 Java 语言**是区分大小写**的，所以 price 和 Price 是两个完全不同的变量哦！

## 3.2 Java中的数据类型

为了方便物品的存储，我们会规定每个盒子可以存放的物品种类，就好比在“放臭袜子的盒子”里我们是不会放“面包”的！同理，变量的存储也讲究“分门别类”！

 Java 中存储的数据都是有类型的，而且必须在编译时就确定其类型。 Java 中有两类数据类型：

![img](http://img.mukewang.com/535a6fc10001b8f604930247.jpg)

在 Java 的领域里**，基本数据类型变量**存的是**数据本身**，而**引用类型变量**存的是保存**数据的空间地址**。说白了，基本数据类型变量里存储的是直接放在抽屉里的东西，而引用数据类型变量里存储的是这个抽屉的钥匙，钥匙和抽屉一一对应。

常用的基本数据类型有：

![img](http://img.mukewang.com/540d468d000167bd07000130.jpg)

单精度浮点数（float）与双精度浮点数（double）的区别如下：

（1）在内存中占有的字节数不同

•单精度浮点数在机内占4个字节

•双精度浮点数在机内占8个字节

（2）有效数字位数不同

•单精度浮点数有效数字8位

•双精度浮点数有效数字16位

（3）在程序中处理速度不同

一般来说，CPU处理单精度浮点数的速度比处理双精度浮点数快

 ***特殊****

![img](http://img.mukewang.com/536888bb0001b9f803900106.jpg)

**String** 是一种常见的**引用数据类型**，用来表示字符串。在程序开发中，很多操作都要使用字符串来完成，例如系统中的用户名、密码、电子邮箱等。

## 3.3 JAVA中变量的使用规则

1、Java 中的变量需要先声明后使用

2、变量使用时，可以声明变量的同时进行初始化

[![img](http://img.mukewang.com/5358cc640001c54f01800024.jpg)](http://img.mukewang.com/5358cc640001c54f01800024.jpg)，

也可以先声明后赋值

[![img](http://img.mukewang.com/5358cc220001e08901720044.jpg)](http://img.mukewang.com/5358cbdb00012a5401910048.jpg)

3、变量中每次只能赋一个值，但可以修改多次

[![img](http://img.mukewang.com/536889b300012af004300053.jpg)](http://img.mukewang.com/536889b300012af004300053.jpg)

4、main 方法中定义的变量必须先赋值，然后才能输出

[![img](http://img.mukewang.com/536889c000019eb805080079.jpg)](http://img.mukewang.com/536889c000019eb805080079.jpg)

5、虽然语法中没有提示错误，但**在实际开发中，变量名不建议使用中文**，容易产生安全隐患，譬如后期跨平台操作时出现乱码等等

[![img](http://img.mukewang.com/5450a3ed000137a604590122.jpg)](http://img.mukewang.com/5450a3ed000137a604590122.jpg)

**关于 String ：表示变量中存储的数据的类型为字符串**

## 3.4 JAVA中的自动类型转换

在 Java 程序中，不同的基本数据类型的数据之间经常需要进行相互转换。例如：

[![img](http://img.mukewang.com/5359d0c70001ffe202530066.jpg)](http://img.mukewang.com/5359d0c70001ffe202530066.jpg)，

代码中 int 型变量 score1 可以直接为 double 型变量 score2 完成赋值操作，运行结果为： **82.0** 

这种转换称为**自动类型转换**。

当然自动类型转换是需要**满足特定的条件**的：

\1.  **目标类型能与源类型兼容，如 double 型兼容 int 型，但是 char 型不能兼容 int 型**

[![img](http://img.mukewang.com/53688a3200014fc803800109.jpg)](http://img.mukewang.com/53688a3200014fc803800109.jpg)

\2.  **目标类型大于源类型，如 double 类型长度为 8 字节， int 类型为 4 字节，因此 double 类型的变量里直接可以存放 int 类型的数据，但反过来就不可以了**

[![img](http://img.mukewang.com/53688a460001539403740086.jpg)](http://img.mukewang.com/53688a460001539403740086.jpg)

**特殊**

float是4个字节保存，int也是4个字节保存，**把float转换为int可能会损失精度，需要强转。**

例如：int x = (int)10.0f;

```
默认为直接舍掉小数部分，取整数值。实例：

        int a = (int) 10.5f;   //a = 10;
```

```
如何实现按四舍五入转换呢？转换前先加上 0.5f。实例：

        float f = 10.5f;

        int a = (int) (f + 0.5f);
```

## 3.5 Java中的强制类型转换

尽管自动类型转换是很方便的，但并不能满足所有的编程需要。  

例如，当程序中需要将 double 型变量的值赋给一个 int 型变量，该如何实现呢？

显然，这种转换是不会自动进行的！因为 int 型的存储范围比 double 型的小。此时就需要通过**强制类型转换**来实现了。

语法：

**( 数据类型 ) 数值**

[![img](http://img.mukewang.com/53688a9a0001f73404330109.jpg)](http://img.mukewang.com/53688a9a0001f73404330109.jpg)

运行结果：

[![img](http://img.mukewang.com/5359d73a00016cde00500033.jpg)](http://img.mukewang.com/5359d73a00016cde00500033.jpg)

可以看到，通过强制类型转换将 75.8 赋值给 int 型变量后，结果为 75，数值上并未进行四舍五入，而是直接将小数位截断。		

明白了吧，但**强制类型转换可能会造成数据的丢失**，需要慎重使用。

## 3.6 Java中常量的应用

所谓常量，我们可以理解为是一种特殊的变量，它的值被设定后，在**程序运行过程中不允许改变**。

语法：**final 常量名 = 值;**

[![img](http://img.mukewang.com/53689a880001620703990081.jpg)](http://img.mukewang.com/53689a880001620703990081.jpg)

程序中使用常量可以提高代码的**可维护性**。例如，在项目开发时，我们需要指定用户的性别，此时可以定义一个常量 SEX，赋值为 "男"，在需要指定用户性别的地方直接调用此常量即可，避免了由于用户的不规范赋值导致程序出错的情况。

**注意**：**常量名一般使用大写字符**



## 3.7 如何在Java中使用注释

在编写程序时，经常需要添加一些注释，**用以描述某段代码的作用**。

一般来说，对于一份规范的程序源代码而言，注释应该占到源代码的 1/3 以上。因此，注释是程序源代码的重要组成部分，一定要加以重视。

Java 中注释有三种类型：**单行注释、多行注释、文档注释**

[![img](http://img.mukewang.com/535ce105000118b504440337.jpg)](http://img.mukewang.com/535ce105000118b504440337.jpg)

运行结果： **Hello Imooc!**

看：**被注释的代码块在程序运行时是不会被执行的**

我们可以通过 **javadoc** 命令从文档注释中提取内容，生成程序的 API 帮助文档。

[![img](http://img.mukewang.com/53689f74000187be03800330.jpg)](http://img.mukewang.com/53689f74000187be03800330.jpg)

打开首页，查看下生成的 API 文档

[![img](http://img.mukewang.com/535ce323000141ff04670397.jpg)](http://img.mukewang.com/535ce323000141ff04670397.jpg)

PS：使用文档注释时还可以使用 **javadoc 标记**，生成更详细的文档信息：

​    @author 标明开发该类模块的作者

​    @version 标明该类模块的版本

​    @see 参考转向，也就是相关主题

​    @param 对方法中某参数的说明

​    @return 对方法返回值的说明

​    @exception 对方法可能抛出的异常进行说明。

# 4.运算符

运算符是一种“功能”符号，用以通知 Java 进行相关的运算。譬如，我们需要将变量 age 的值设置为 20 ，这时候就需要一个“=”，告诉程序需要进行赋值操作。

Java 语言中常用的运算符可分为如下几种：

Ø 算术运算符

Ø 赋值运算符

Ø 比较运算符

Ø 逻辑运算符

Ø 条件运算符

## 4.1 Java中的算术运算符

算术运算符主要用于进行基本的算术运算，如加法、减法、乘法、除法等。

Java 中常用的算术运算符：

[![img](http://img.mukewang.com/5368a1a10001da7603050148.jpg)](http://img.mukewang.com/5368a1a10001da7603050148.jpg)

 其中，**++** 和 **--** 既可以出现在操作数的左边，也可以出现在右边，但结果是不同滴

例1：

[![img](http://img.mukewang.com/5368a1f1000171c403980094.jpg)](http://img.mukewang.com/5368a1f1000171c403980094.jpg)

运行结果：

[![img](http://img.mukewang.com/535e6a9c000128ef00900039.jpg)](http://img.mukewang.com/535e6a9c000128ef00900039.jpg)

例2：

[![img](http://img.mukewang.com/5368a0ae00016f2603970091.jpg)](http://img.mukewang.com/5368a0ae00016f2603970091.jpg)

运行结果：

[![img](http://img.mukewang.com/535e6b040001403800890034.jpg)](http://img.mukewang.com/535e6b040001403800890034.jpg)

一定要注意哦！自增和自减运算符**只能用于操作变量**，**不能直接用于操作数值或常量**！例如 5++ 、 8-- 等写法都是错误滴！

PS：% 用来求余数，也称为”取模运算符“

## 4.2 Java中的赋值运算符

赋值运算符是指为变量或常量指定数值的符号。如可以使用 “=” 将右边的表达式结果赋给左边的操作数。

Java 支持的常用赋值运算符，如下表所示：

[![img](http://img.mukewang.com/5360ebdb0001401b04430144.jpg)](http://img.mukewang.com/5360ebdb0001401b04430144.jpg)

## 4.3 Java中的比较运算符

比较运算符用于判断两个数据的大小，例如：大于、等于、不等于。比较的结果是一个布尔值（ true 或 false ）。

Java 中常用的比较运算符如下表所示：

[![img](http://img.mukewang.com/536063f00001b7b904350145.jpg)](http://img.mukewang.com/536063f00001b7b904350145.jpg)

注意哦：

**1、  > 、 < 、 >= 、 <= 只支持左右两边操作数是数值类型**

**2、  == 、 != 两边的操作数既可以是数值类型，也可以是引用类型**

例子：

![image-20201212165106304](C:\Users\25902\AppData\Roaming\Typora\typora-user-images\image-20201212165106304.png)

![img](http://img.mukewang.com/535f56610001757b01980076.jpg)

## 4.4 Java中的逻辑运算符

逻辑运算符主要用于进行逻辑运算。Java 中常用的逻辑运算符如下表所示：

[![img](http://img.mukewang.com/5360ef9700017b9405870095.jpg)](http://img.mukewang.com/5360ef9700017b9405870095.jpg)

我们可以从“投票选举”的角度理解逻辑运算符：

1、 **与**：要求所有人都投票同意，才能通过某议题

2、 **或**：只要求一个人投票同意就可以通过某议题

3、 **非**：某人原本投票同意，通过非运算符，可以使其投票无效

4、 **异或**：**有且只能有**一个人投票同意，才可以通过某议题

当使用逻辑运算符时，我们会遇到一种很有趣的“**短路**”现象。（即只能运行一半）

譬如：( one > two ) && ( one < three ) 中，如果能确定左边 one > two 运行结果为 false , 则系统就认为已经没有必要执行右侧的 one < three 啦。

同理，在( one > two ) || ( one < three ) 中，如果能确定左边表达式的运行结果为 true , 则系统也同样会认为已经没有必要再进行右侧的 one < three 的执行啦！

![image-20201212171254413](C:\Users\25902\AppData\Roaming\Typora\typora-user-images\image-20201212171254413.png)

## 4.5 Java中的条件运算符

条件运算符（ ? : ）也称为 “三元运算符”。

语法形式：**布尔表达式 ？ 表达式1 ：表达式2**

运算过程：如果布尔表达式的值为 **true** ，则返回 **表达式1** 的值，否则返回 **表达式2** 的值

例如：

[![img](http://img.mukewang.com/535f7d130001a84f04340051.jpg)](http://img.mukewang.com/535f7d130001a84f04340051.jpg)

因为，表达式 8>5 的值为 true ，所以，返回： **8大于5**

## 4.6 Java中运算符的优先级

所谓优先级，就是在表达式中的运算顺序。Java 中常用的运算符的优先级如下表所示：

[![img](http://img.mukewang.com/5360ffb90001b4f002620224.jpg)](http://img.mukewang.com/5360ffb90001b4f002620224.jpg)

**级别为 1 的优先级最高，级别 11 的优先级最低**。譬如，x = 7 + 3 * 2  得到的结果是 13 “先乘后加”嘛!

PS：大家没必要去死记运算符的优先级顺序，实际开发中，一般会使用**小括号**辅助进行优先级管理。例如：

[![img](http://img.mukewang.com/5361000a000129a005060071.jpg)](http://img.mukewang.com/5361000a000129a005060071.jpg)

分析：小括号优先级最高，因此

1、 执行 a + 18 ，结果为 30

2、 执行( a + 18 ) % 4 取模，结果为 2

3、 执行 a * ( ( a + 18 ) % 4 )，结果为 24

**例子：**

请在编辑器中的第 **5** 行输入如下代码，

```
int x =（m*8/(n+2))%m
```

  相信结合运行结果，大家会对运算符的优先级会有更加清晰的理解！

**int  x = ( m \* 8 / ( n + 2 ) ) % m ;**

运行结果：

 [![img](http://img.mukewang.com/536101080001693000560061.jpg)](http://img.mukewang.com/536101080001693000560061.jpg)

![image-20201212172744164](C:\Users\25902\AppData\Roaming\Typora\typora-user-images\image-20201212172744164.png)

## 5.1 Java条件语句之 if

生活中，我们经常需要先做判断，然后才决定是否要做某件事情。例如，如果考试成绩大于 90 分，则奖励一个 IPHONE 5S 。对于这种“需要先判断条件，条件满足后才执行的情况”，就可以使用 **if 条件语句**实现。

语法：.

 [![img](http://img.mukewang.com/5364ef240001832c01830068.jpg)](http://img.mukewang.com/5364ef240001832c01830068.jpg)

执行过程：

 [![img](http://img.mukewang.com/53635a6b00011ebc01660184.jpg)](http://img.mukewang.com/53635a6b00011ebc01660184.jpg)

如：

[![img](http://img.mukewang.com/5364edff0001e2f004580095.jpg)](http://img.mukewang.com/5364edff0001e2f004580095.jpg)

注意哦：如果 if 条件成立时的**执行语句只有一条，是可以省略大括号**滴！但如果执行语句**有多条，那么大括号就是不可或缺的**。

## 5.2 Java条件语句之 if...else

**if...else** 语句的操作比 if 语句多了一步:  当条件成立时，则执行 if 部分的代码块； 条件不成立时，则进入 else 部分。例如，如果考试成绩大于 90 分，则奖励一个 IPHONE 5S ，否则罚做 500 个俯卧撑。

语法：

**[![img](http://img.mukewang.com/5364f0f300019c8c01880110.jpg)](http://img.mukewang.com/5364f0f300019c8c01880110.jpg)**

执行过程：

 **[![img](http://img.mukewang.com/536369030001ee7402510205.jpg)](http://img.mukewang.com/536369030001ee7402510205.jpg)**

如：

[![img](http://img.mukewang.com/5364f1e90001ed1304610132.jpg)](http://img.mukewang.com/5364f1e90001ed1304610132.jpg)

## 5.3 Java条件语句之多重 if

**多重 if 语句**，在条件 1 不满足的情况下，才会进行条件 2 的判断；当前面的条件均不成立时，才会执行 else 块内的代码。例如，如果考试成绩大于 90 分，则奖励一个 IPHONE 5S ，如果成绩介于 70 分至 90 分之间，则奖励一个红米，否则罚做 500 个俯卧撑。

语法：

 **[![img](http://img.mukewang.com/5364f177000198dd01660156.jpg)](http://img.mukewang.com/5364f177000198dd01660156.jpg)**

执行过程：

 **[![img](http://img.mukewang.com/5364a1db0001b6fb03790248.jpg)](http://img.mukewang.com/5364a1db0001b6fb03790248.jpg)**

如：

[![img](http://img.mukewang.com/5364f29c000137a804620178.jpg)](http://img.mukewang.com/5364f29c000137a804620178.jpg)

该段代码的含义是：如果 score 值大于90，则奖励一个 Iphone 5s ，当 score 值小于等于 90 时，先判断 score 是否大于 70 ，如果 score 是介于 70--90 之间，则奖励一个红米，如果成绩小于等于 70 ，则罚做 500 个俯卧撑

当需要判断的条件是连续的区间时，使用多重 if 语句是非常方便滴！

**例子：**

请在编辑器中应用多重 if 语句，补全代码实现如下功能：

假设年龄大于 60 岁，则提示“老年”；如果年龄介于 40 岁至 60 岁之间，则提示“中年”；如果年龄介于 18 岁至 40 岁之间，则提示“少年”； 18 岁以下则提示“童年”

运行结果为： **少年**

![image-20201212181725582](C:\Users\25902\AppData\Roaming\Typora\typora-user-images\image-20201212181725582.png)

## 5.4 Java条件语句之嵌套 if

**嵌套 if 语句**，只有当外层 if 的条件成立时，才会判断内层 if 的条件。例如，活动计划的安排，如果今天是工作日，则去上班，如果今天是周末，则外出游玩；同时，如果周末天气晴朗，则去室外游乐场游玩，否则去室内游乐场游玩。

语法：

 **[![img](http://img.mukewang.com/5364f3be000121bf01480198.jpg)](http://img.mukewang.com/5364f3be000121bf01480198.jpg)**

执行过程：

 **[![img](http://img.mukewang.com/5364bd8f0001c91e03690285.jpg)](http://img.mukewang.com/5364bd8f0001c91e03690285.jpg)**

例如：

[![img](http://img.mukewang.com/53703cb10001f78a06340312.jpg)](http://img.mukewang.com/53703cb10001f78a06340312.jpg)

运行结果为： **去室外游乐场游玩**

## 5.5 Java条件语句之 switch

当需要对选项进行等值判断时，使用 switch 语句更加简洁明了。例如：根据考试的名次，给予前 4 名不同的奖品。第一名，奖励笔记本一台；第二名，奖励 IPAD 2 一个；第三名，奖励移动电源一个；最后一名奖励 U 盘一个。

**语法：**

**[![img](http://img.mukewang.com/5364f4c800010b1f01620289.jpg)](http://img.mukewang.com/5364f4c800010b1f01620289.jpg)**

执行过程：**当 switch 后表达式的值和 case 语句后的值相同时，从该位置开始向下执行，直到遇到 break 语句或者 switch 语句块结束；如果没有匹配的 case 语句则执行 default 块的代码。**

如：

[![img](http://img.mukewang.com/5364f5e300010b6004790310.jpg)](http://img.mukewang.com/5364f5e300010b6004790310.jpg)

不得不说的几点小秘密：

1、 switch 后面小括号中表达式的值必须是**整型或字符型**

2、 case 后面的值**可以是常量数值**，如 1、2；也**可以是一个常量表达式**，如 2+2 ；但不能是变量或带有变量的表达式，如 a * 2。case后**可以跟字符，但必须是常量字符**，**常量字符就是用单引号引起来的字符**。

3、 case 匹配后，执行匹配块里的程序代码，如果没有遇见 **break** 会继续执行下一个的 case 块的内容，直到遇到 break 语句或者 switch 语句块结束 如

 [![img](http://img.mukewang.com/5364f6440001425d04810245.jpg)](http://img.mukewang.com/5364f6440001425d04810245.jpg)，

运行结果：

 [![img](http://img.mukewang.com/5364f74800013d9101330090.jpg)](http://img.mukewang.com/5364f74800013d9101330090.jpg)

4、 可以把功能相同的 case 语句合并起来，如

[![img](http://img.mukewang.com/5364f6950001a57604280064.jpg)](http://img.mukewang.com/5364f6950001a57604280064.jpg)

5、 default 块可以出现在**任意位置**，也**可以省略**

## 5.6 Java循环语句之 while

生活中，有些时候为了完成任务，需要重复的进行某些动作。如参加 10000 米长跑，需要绕 400 米的赛道反复的跑 25 圈。在 Java 中实现功能时，也经常需要重复执行某些代码，例如，我们为了表示“浓烈的爱”，希望输出 1000 行“我爱慕课网！”。显然，此时重复敲 1000 遍输出语句是不靠谱滴！！那么，有木有好的办法来解决呢？ 有，**循环语句**！

Java 常用的 3 种循环： **while 、 do...while 、 for**

本小节咱们先来聊聊 **while**

**语法：**

 [![img](http://img.mukewang.com/53699fb9000143d801590067.jpg)](http://img.mukewang.com/53699fb9000143d801590067.jpg)

执行过程：

< 1 >、 判断 while 后面的条件是否成立( true / false )

< 2 >、 当条件成立时，执行循环内的操作代码 ，然后重复执行< 1 >、< 2 >， 直到循环条件不成立为止

特点：**先判断，后执行**

如：

[![img](http://img.mukewang.com/5369a5910001ccb503750113.jpg)](http://img.mukewang.com/5369a5910001ccb503750113.jpg)

## 5.7 Java循环语句之 do...while

**do...while 循环**与 while 循环语法有些类似，但执行过程差别比较大。

语法：

 [![img](http://img.mukewang.com/536a018100011a0401720070.jpg)](http://img.mukewang.com/536a018100011a0401720070.jpg)

执行过程：

<1>、 先执行一遍循环操作，然后判断循环条件是否成立

<2>、 如果条件成立，继续执行< 1 > 、< 2 >，直到循环条件不成立为止

特点： **先执行，后判断**

由此可见，do...while 语句保证循环**至少被执行一次**！

例如，依然输出 1000 遍“我爱慕课网”，使用 do...while 的实现代码为：

[![img](http://img.mukewang.com/536a01150001976604830150.jpg)](http://img.mukewang.com/536a01150001976604830150.jpg)

## 5.8 Java循环语句之 for

Java 的循环结构中除了 while 和 do...while 外，还有 **for 循环**，三种循环可以相互替换。

语法： 

[![img](http://img.mukewang.com/536af1e60001f83604160073.jpg)](http://img.mukewang.com/536af1e60001f83604160073.jpg)

执行过程：

<1>、 执行循环变量初始化部分，设置循环的初始状态，此部分在整个循环中只执行一次

<2>、 进行循环条件的判断，如果条件为 true ，则执行循环体内代码；如果为 false ，则直接退出循环

<3>、 执行循环变量变化部分，改变循环变量的值，以便进行下一次条件判断

<4>、 依次重新执行< 2 >、< 3 >、< 4 >，直到退出循环

特点：相比 while 和 do...while 语句**结构更加简洁易读**

例如，输出 1000 遍“我爱慕课网”，使用 for 的实现代码为：

[![img](http://img.mukewang.com/536aea30000190eb04790088.jpg)](http://img.mukewang.com/536aea30000190eb04790088.jpg)

需要留心的几个小细节：

1、 for 关键字后面括号中的三个表达式必须用 “;” 隔开，三个表达式都可以省略，但 “;” 不能省略。

  a. 省略“循环变量初始化”，可以在 for 语句之前由赋值语句进行变量初始化操作，如:

[![img](http://img.mukewang.com/536c6cc80001c00505490117.jpg)](http://img.mukewang.com/536c6cc80001c00505490117.jpg)

  b. 省略“循环条件”，可能会造成循环将一直执行下去，也就是我们常说的“死循环”现象，如:

[![img](http://img.mukewang.com/536c6d060001fa4405310092.jpg)](http://img.mukewang.com/536c6d060001fa4405310092.jpg)

在编程过程中要避免“死循环”的出现，因此，对于上面的代码可以在循环体中使用 break 强制跳出循环（关于 break 的用法会在后面介绍）。

  c. 省略“循环变量变化”，可以在循环体中进行循环变量的变化，如：

[![img](http://img.mukewang.com/53704a7b0001217905270113.jpg)](http://img.mukewang.com/53704a7b0001217905270113.jpg)

2、 for 循环变量初始化和循环变量变化部分，可以是使用 “,” 同时初始化或改变多个循环变量的值，如：

[![img](http://img.mukewang.com/536c8b620001eb1005560086.jpg)](http://img.mukewang.com/536c8b620001eb1005560086.jpg)

代码中，初始化变量部分同时对两个变量 i 和 j 赋初值，循环变量变化部分也同时对两个变量进行变化，运行结果：

[![img](http://img.mukewang.com/536c8dc50001b60e00730112.jpg)](http://img.mukewang.com/536c8dc50001b60e00730112.jpg)

3、 循环条件部分可以使用逻辑运算符组合的表达式，表示复杂判断条件，但一定注意运算的优先级，如：

[![img](http://img.mukewang.com/536c8e120001306804240071.jpg)](http://img.mukewang.com/536c8e120001306804240071.jpg)

代码中，必须同时满足变量 i 小于 10 ，并且 i 不等于 5 时才会进行循环，输出变量 i 的值。

## 5.9 Java循环跳转语句之 break

生活中，我们经常会因为某些原因中断既定的任务安排。如在参加 10000 米长跑时，才跑了 500 米就由于体力不支，需要退出比赛。在 Java 中，我们可以使用 break 语句退出指定的循环，直接执行循环后面的代码。

**例如，**使用循环输出 1--10的数值，其中，如果数值大于 2 ，并且为 3 的倍数则停止输出。

**实现代码**：

[![img](http://img.mukewang.com/536b36a80001ed4b05420273.jpg)](http://img.mukewang.com/536b36a80001ed4b05420273.jpg)

运行结果：

[![img](http://img.mukewang.com/536b36d70001a8f200670071.jpg)](http://img.mukewang.com/536b36d70001a8f200670071.jpg)

## 5.10 Java循环跳转语句之 continue

**continue** 的作用是跳过循环体中剩余的语句执行下一次循环。

例如，打印 1--10 之间所有的偶数，使用 continue 语句实现代码为：

[![img](http://img.mukewang.com/536b50410001d1a706020200.jpg)](http://img.mukewang.com/536b50410001d1a706020200.jpg)

运行结果：

[![img](http://img.mukewang.com/536b50770001d42a00350109.jpg)](http://img.mukewang.com/536b50770001d42a00350109.jpg)

## 5.11 Java 循环语句之多重循环

循环体中包含循环语句的结构称为**多重循环**。三种循环语句可以自身嵌套，也可以相互嵌套，最常见的就是**二重循环**。在二重循环中，外层循环每执行一次，内层循环要执行一圈。

如下所示：

[![img](http://img.mukewang.com/549154470001ea5204920260.jpg)](http://img.mukewang.com/549154470001ea5204920260.jpg)

例如：使用 * 打印长方形：

[![img](http://img.mukewang.com/536c5253000181a900810058.jpg)](http://img.mukewang.com/536c5253000181a900810058.jpg)

实现代码为：

[![img](http://img.mukewang.com/536c549d0001381003560206.jpg)](http://img.mukewang.com/536c549d0001381003560206.jpg)

执行流程：当 i = 1 时，外层循环条件成立，进入内层循环，开始打印第一行内容。此时， j 从 1 开始，循环 8 次，内层循环结束后换行，实现第一行 8 个 * 的输出。接下来返回外层循环 i 变为 2 ，准备打印下一行，依此类推，直到完成长方形的打印。

## 6.1 编程优化

(1)使用 Scanner工具类接受用户输入信息。

固定格式为：

**String 变量=new Scanner(System.in).next();**

**或者**

**int 变量=new Scanner(System.in).nextInt();**

**或者**

```
//创建一个Scanner对象，去获取从键盘上输入的学生ID字符串
Scanner console=new Scanner(System.in);
//取得从键盘上输入的学生ID
            String stuID=console.next();
```

(2) print ——打印内容	

println——打印并换行

## 6.2 编程进阶

**psvm** 可以直接生成程序入口，即

```java
public static void main(String[] args){
```

**sout** 可以直接生成——

```java
System.out.println();
```

进阶练习：

![image-20201218140040061](C:\Users\25902\AppData\Roaming\Typora\typora-user-images\image-20201218140040061.png)



## 7.1 什么是数组

问：编写代码保存 4 名学生的考试成绩。

答：简单啊，定义 4 个变量呗

问：那“计算全年级 400 名学生的考试成绩”，肿么办

答： 。。。。。。。

**数组**，就可以帮助你妥妥的解决问题啦！！

数组可以理解为是一个巨大的“盒子”，里面可以按顺序存放多个类型相同的数据，比如可以定义 int 型的数组 scores 存储 4 名学生的成绩

**注意：括号里的数据是用"，"隔开的！而for语句括号中是用"；"隔开的！**

[![img](http://img.mukewang.com/537074a400017cd905290196.jpg)](http://img.mukewang.com/537074a400017cd905290196.jpg)

**数组中的元素都可以通过下标来访问，下标从 0 开始。例如，可以通过 scores[0] 获取数组中的第一个元素 76 ，scores[2] 就可以取到第三个元素 92 啦**！



## 7.2如何使用 Java 中的数组

Java 中操作数组只需要四个步骤：

**1、 声明数组**

语法： **数据类型[ ] 数组名；**

或者  **数据类型 数组名[ ]；**

其中，数组名可以是任意合法的变量名，如：

[![img](http://img.mukewang.com/5371e91d000147e903790167.jpg)](http://img.mukewang.com/5371e91d000147e903790167.jpg)

**2、 分配空间**

简单地说，就是指定数组中最多可存储多少个元素

语法： **数组名 = new  数据类型 [ 数组长度 ];**

其中，数组长度就是数组中能存放元素的个数，如：

[![img](http://img.mukewang.com/5371ecc10001c97804260171.jpg)](http://img.mukewang.com/5371ecc10001c97804260171.jpg)

话说，我们也可以将上面的两个步骤合并，在声明数组的同时为它分配空间，如：[![img](http://img.mukewang.com/5371ed4200012bee03590033.jpg)](http://img.mukewang.com/5371ed4200012bee03590033.jpg)

**3、 赋值**

分配空间后就可以向数组中放数据了，数组中元素都是通过下标来访问的，例如向 scores 数组中存放学生成绩

[![img](http://img.mukewang.com/5371ed9f0001accb02100053.jpg)](http://img.mukewang.com/5371ed9f0001accb02100053.jpg)

**4、 处理数组中数据**

我们可以对赋值后的数组进行操作和处理，如获取并输出数组中元素的值

[![img](http://img.mukewang.com/5371eec50001332707460043.jpg)](http://img.mukewang.com/5371eec50001332707460043.jpg)

在 Java 中还提供了另外一种直接创建数组的方式，它将声明数组、分配空间和赋值合并完成，如

[![img](http://img.mukewang.com/5371ee8b000101aa04540056.jpg)](http://img.mukewang.com/5371ee8b000101aa04540056.jpg)

它等价于：

[![img](http://img.mukewang.com/5371ef0f0001528c04830059.jpg)](http://img.mukewang.com/5371ef0f0001528c04830059.jpg)

## 7.3 使用循环操作 Java 中的数组

实际开发中我们经常使用循环控制数组成员的操作。如：

 [![img](http://img.mukewang.com/5372da76000146e908070159.jpg)](http://img.mukewang.com/5372da76000146e908070159.jpg)

运行结果：

 [![img](http://img.mukewang.com/5372da900001155a02500094.jpg)](http://img.mukewang.com/5372da900001155a02500094.jpg)

其中， **数组名.length 用于获取数组的长度**

需要注意的“小毛病”：

1、 **数组下标从 0 开始**。因此 scores[3] ，表示数组中的第 4 个元素，而并非第 3 个元素

2、 数组**下标的范围是 0 至 数组长度-1** ，如果越界访问，就会报错。如：

[![img](http://img.mukewang.com/5372db2c0001ee4303280058.jpg)](http://img.mukewang.com/5372db2c0001ee4303280058.jpg)

运行时会报如下错误： 

[![img](http://img.mukewang.com/5372db510001831408440046.jpg)](http://img.mukewang.com/5372db510001831408440046.jpg)

上面错误信息的意思是数组下标超过范围，即数组访问越界。在上面的代码中创建一个长度为 2 的数组，因此数组下标范围是 0 到 1 ，而程序中下标出现了 2 ，即 scores[2] ，超过了范围，造成数组访问越界。

**索引越界异常**：

输入的数字超过了代码中的范围。

用

```
try{

}

catch(ArrayIndexOutOfBoundsException e){

}
```

语法来解决。

**例：**

```java
import java.util.Scanner;

public class 练习 {
    public static void main(String[] args) {
        String[] contentList = new String[35];
        contentList[0] = "【第1周】环境搭建与语法入门";
        contentList[1] = "【第2周】Java语法之循环、数组与方法";
        contentList[2] = "【第3周】面向对象之封装与继承";
        contentList[3] = "【第4周】面向对象之单例模式与多态";
        contentList[4] = "【第5周】常用工具类（上）";
        contentList[5] = "【第6周】常用工具类（下）";
        contentList[6] = "【第7周】常用工具类（下）";
        contentList[7] = "【第8周】前端基础之HTML与CSS";
        contentList[8] = "【第9周】前端基础之JavaScript与综合案例";
        contentList[9] = "【第10周】Java Web基础";
        contentList[10] = "【第11周】Java Web基础";
        contentList[11] = "【第12周】常用功能与过滤器";
        contentList[12] = "【第13周】监听器与项目实战";
        contentList[13] = "【第14周】监听器与项目实战";
        contentList[14] = "【第15周】MySQL基础";
        contentList[15] = "【第16周】MySQL基础";
        contentList[16] = "【第17周】Java数据库开发基础";
        contentList[17] = "【第18周】框架前置知识";
        contentList[18] = "【第19周】MyBatis基础";
        contentList[19] = "【第20周】MyBatis实现OA系统项目实战";
        contentList[20] = "【第21周】MyBatis实现OA系统项目实战";
        contentList[21] = "【第22周】Linux环境搭建与Redis应用";
        contentList[22] = "【第23周】Spring基础";
        contentList[23] = "【第24周】Spring基础";
        contentList[24] = "【第25周】Spring基础";
        contentList[25] = "【第26周】SSM开发社交网站";
        contentList[26] = "【第27周】Spring Boot电商项目实战";
        contentList[27] = "【第28周】Spring Boot电商项目实战";
        contentList[28] = "【第29周】面试";
        contentList[29] = "【第30周】多线程与分布式";
        contentList[30] = "【第31周】多线程与分布式";
        contentList[31] = "【第32周】Spring Cloud基础";
        contentList[32] = "【第33周】Spring Cloud电商实战";
        contentList[33] = "【第34周】Spring Cloud电商实战";
        contentList[34] = "【第35周】Zookeeper+Dubbo应用与面试";

        //提示信息
        System.out.print("您要开始第几周学习啦,直接输入数字吧:");
        //设置变量存储接收到的数据
        int  a = new Scanner(System.in).nextInt();

        //计算今天是几月(1-月第一周、4-月第4周)
        int b=0;
        int c=0;
        if (a%4==0){
            b=a/4;
            c=4;
        }else {
            b=a/4+1;
            c=a%4;
        }
        //计算输入的周是这个月的第几周

        //提示信息
        System.out.println("以下是您本月的学习计划, √ 代表当周学习任务");
        System.out.println("=======================================");

        //利用for循环，找到数组中对应这个月的内容输出
        for(int i=(b-1)*4;i<b*4;i++){
            try {
                if (i+1==a){
                    System.out.println("√"+contentList[i]);
                }else {
                    System.out.println(contentList[i]);
                }
            }
            catch (ArrayIndexOutOfBoundsException e){
                System.out.println("未发现第"+(i+1)+"周学习记录");
            }

        }

    }
}
```

