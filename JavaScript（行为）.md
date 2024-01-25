#                                      JavaScript（行为）

### JavaScript引入方式

- 内部脚本：将JS代码定义在HTML页面中
- 外部脚本：将JS代码定义在外部JS文件中，然后引入到HTML页面中



### JavaScript基础语法

- 书写语法
  - 区分大小写
  - 每行结尾分号可有可无
  - 注释：
    - 单行：//
    - 多行：/*     */
- 输出语句
  - window.alert( )写入警告框
  - document.write( )写入HTML输出
  - console.log( )写入浏览器控制台
- 变量
  - 用var关键字声明变量
  - javascript是一弱类型语言，变量可以存放不同类型的值
  - 数字不能开头，建议使用驼峰命名
  - let声明的变量作用域在代码块中 ，不允许重复声明

- 数据类型
  - 原始类型
    - number
    - string：字符、字符串，单双引号皆可
    - boolean
    - null
    - undefined：当声明变量未初始化时，默认是undefined

- 函数
  - 定义：通过function关键词进行定义
  - 形式参数和返回类型都不需要定义类型
  - 调用：函数名称（实际参数）





### Javascript对象

- Array对象

  - 定义：
    - var arr = new Array(1,2,3);
    - var arr = [1,2,3];

  - 访问：
    - arr[索引] = 值；

- String对象

  - 定义：
    - var str = new String("hello");
    - var str = "hello"或‘hello’

- 自定义对象

  - 格式：

    var 对象名称 = {

    ​                       属性名称1：属性值1，

    ​                       属性名称2：属性值2，

    ​                       函数名称：function（形参列表）{}

    }；

### BOM（浏览器对象吗，模型）

- Window：浏览器对象

- History：历史记录对象





### DOM（文档对象模型）

- 获取Element对象

 

- 事件监听
  - 可以在事件被侦测时执行代码