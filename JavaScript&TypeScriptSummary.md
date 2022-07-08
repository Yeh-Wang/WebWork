# JavaScript&TypeScript总结  

## **JavaScript**  

* `<Script></Script>` 标签  
需要在HTML中插入Js代码时，需要用此标签包裹。这表明JavaScript从哪里开始从哪里结束。  

* JavaScript中的变量  
（1）变量必须以字母开头
（2）变量也能以`$`和`_`符号开头
（3）变量名称对大小写敏感（y 和 Y 是不同的变量）  
  * 全局变量:在函数外声明的变量是全局变量,生命周期从被声明开始直到程序停止运行。

  * 局部变量:在 JavaScript 函数内部声明的变量（使用 `var`）是局部变量，所以只能在函数内部访问它。（该变量的作用域是局部的）函数执行结束后变量失效。

* JavaScript 数据类型  
  * 基本数据类型  
    * 字符串（String）、数字(Number)、布尔(Boolean)、空（Null）、未定义类型（Undefined）。
  * 对象数据类型
    * 对象(Object)、数组(Array)、函数(Function),日期（Date）。  

* JavaScript 函数
  * 语法:使用关键字`function`声明,包裹在花括号内（与高级语言的函数类似）。  
  * 可以传入参数，也可以有返回值。  

* JavaScript 事件  
可以对触发的HTML事件进行处理。  

* JavaScript 操作运算符  
  * 一元操作符 `++ --`  
  * 布尔操作符 `&& || ！`  
    * `&&`和`||`都属于 短路操作！  
  * 算术操作符 `+ - * / %`  
  * 关系操作符 `<> <=>= == ===(全等)  != !==`  

* JavaScript `if...Else` 语句  
  * `if` 语句 : 只有当指定条件为 true 时，使用该语句来执行代码
  * `if...else` 语句 : 当条件为 true 时执行代码，当条件为 false 时执行其他代码
  * `if...else if....else` 语句 : 使用该语句来选择多个代码块之一来执行
  * `switch` 语句 : 使用该语句来选择多个代码块之一来执行  

* JavaScript `for` 循环  
与高级语言的循环控制类似，决定所包裹的代码的执行次数。  

* `Array` 数组方法  
  * 元素联合  
  ![image.png](https://s2.loli.net/2022/07/08/IFHYVLkGO7oWP6z.png)
  ![image.png](https://s2.loli.net/2022/07/08/wH4rIvVjU2QdPTe.png)  
  * 堆栈方法  
  栈是一种 LIFO（Last-In-First-Out，后进先出）的数据结构，也就是最新添加的项最早被移除。而栈中项的插入（叫做推入）和移除（叫做弹出），只发生在一个位置——栈的顶部。
  ![image.png](https://s2.loli.net/2022/07/08/NiBr8dvCS6hyHkX.png)  
  ![image.png](https://s2.loli.net/2022/07/08/nkFscroiZhw75GC.png)  
  * 队列方法
栈数据结构的访问规则是 LIFO（后进先出），而队列数据结构的访问规则是 FIFO（First-In-First-Out，先进先出）。队列在列表的末端添加项，从列表的前端移除项。
由于 `push()` 是向数组末端添加项的方法，因此要模拟队列只需一个从数组前端取得项的方法。实现这一操作的数组方法就是`shift()`，它能够移除数组中的第一个项并返回该项，同时将数组长度减1。  
  ![image.png](https://s2.loli.net/2022/07/08/nmakt6CIfROVJgH.png)  
  ![image.png](https://s2.loli.net/2022/07/08/1lbJfXa7YRTug4j.png)  
  `push、pop`操作在数组末，而`unshift、shift`操作在数组头；`push、unshift`压入而`pop、shift`弹出。  
  * 反转数组项 
    * `reverse()`方法实现数组元素的逆序。  
  * `concat()` 链接方法  
  * splice方法:直接更改原数组  //------------------------------------------------------------------------
    * 删除：可以删除任意数量的项，只需指定 2 个参数：要删除的第一项的位置和要删除的项数。 例如，`splice(0,2)`会删除数组中的前两项。

    * 插入：可以向指定位置插入任意数量的项，只需提供 3 个参数：起始位置、0（要删除的项数） 和要插入的项。如果要插入多个项，可以再传入第四、第五，以至任意多个项。例如，`splice(2,0,'red','green')`会从当前数组的位置 2 开始插入字符串`'red'`和`'green'`。

    * 替换：可以向指定位置插入任意数量的项，且同时删除任意数量的项，只需指定 3 个参数：起 始位置、要删除的项数和要插入的任意数量的项。插入的项数不必与删除的项数相等。例如，`splice (2,1,'red','green')`会删除当前数组位置 2 的项，然后再从位置 2 开始插入字符串`'red' 和 'green'`。

## **TypeScript**  

* Typescript是什么  [TypeScript官网](https://ts.xcatliu.com/)
  * 静态类型
  * 弱类型  
* TypeScript变量声明改用`let`,`const`并加上类型说明，且作用域为块级即以{}为界。
`{这种语法更能让人接受适应前端的数据操作。}`  
* 结构  
![image.png](https://s2.loli.net/2022/07/08/uvi4LHSmCBExAh5.png)  
![image.png](https://s2.loli.net/2022/07/08/5OVDvspUt4lAyMG.png)  
* 函数  
使用完整函数类型定义。  
  * 箭头函数  
* 类Class的定义和使用  
类是属性（有些什么）和函数（能干什么）的集合，是生成对象（Object）或类实例的模板。  

  ```  
  //类的定义和使用
  class MyInfo { //class是关键字，类名默认全部大写首字母
    name: string; //属性
    weather: string; //属性
  
    constructor(name: string, weather: string){ //构造函数，一般用于初始化。如果没有，TS会自动生成一个，以备用new创建类实例时调用。
      this.name = name;
      this.weather = weather;
    }
    printInfo(): void { //其它函数，无返回值
      console.log(`Hello, ${this.name}.`);
      console.log(`Today is ${this.weather}.`);
    }
  }
  let myData = new MyInfo('QiGe', 'raining'); //使用new关键字生成对象，即该类的实例
  myData.printInfo();  
  ```  

* 数据类型  
原始数据类型和对象类型。
  * 原始数据类型:布尔值、数值、字符串、`null`、`undefined`以及 ES6 中的新类型`Symbol`和 ES10 中的新类型`BigInt`。
  * 对象类型: 接口  
    * 在面向对象语言中，接口（Interfaces）是一个很重要的概念，它是对行为的抽象，而具体如何行动需要由类（classes）去实现（implement）。
    TypeScript 中的接口是一个非常灵活的概念，除了可用于对类的一部分行为进行抽象以外，也常用于对「对象的形状（Shape）」进行描述。  
