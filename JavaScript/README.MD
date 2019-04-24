## JavaScript


#### 基础语法

声明对象 

var person={name:"Bill",id:1}

通过new关键字声明对象
var carname=new String;
var x=      new Number;
var y=      new Boolean;
var cars=   new Array;
var person= new Object;


函数

function functionName(val1,val2...valn){
   变量声明和函数功能代码
}


#### JS对象

内建对象
String  Array   Date

对象构造器

``` JavaScript

function person(firstname,lastname,age,eyecolor)
{
this.firstname=firstname;
this.lastname=lastname;
this.age=age;
this.eyecolor=eyecolor;

this.changeName=changeName;
function changeName(name){
  this.lastname = name;
}
}

<!-- 创建对象 -->

var father=new person("Bill","Gates","blue"}

```

#### DOM Document Object Model


html网页可以看成树形结构，每个标签都是一个节点

document对象代表网页本身
document.body是网页里能被看到的部分，也就是<body></body>元素的内容

	//可以切换元素的style
	document.getElementById("name").className="";

由由于DOM即网页对象，所以其可以控制HTML，CSS以及JS

删除html节点（标签元素），必须先获取其父元素

	改变节点文本的三个步骤：
	1.移除所有子节点 removeChild()
	2.创建新内容文本createTextNode()
	3.新创建的文本附加在结点上

	var node=document.getElementById("name");
	while(node.firstChild)
		node.removeChild(node.firstChild);
		node.appendChild(document.createTextNode("ok,maybe you are alone."));

#### BOM Browser Object Model

浏览器对象模型