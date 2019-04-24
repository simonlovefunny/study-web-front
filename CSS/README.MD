## CSS 层叠样式 Cascading Style Sheets

网页外观控制

html控制网页内容，css控制网页外观

#### CSS基础语法

引用CSS

``` css

<head></head>标签内

<style type="text/css">
样式代码...
</style>

```


p-选择器 font-size-属性名 :-声明 20px-属性值

p{font-size: 20px;color:blue;}

selector {property1: value1; property2: value2; ... propertyN: valueN }


派生选择器


链接

链接可以根据点击状态设置样式

a:link{color: red}   /** 未被访问的链接 */
a:visited(color: red)  /** 已被访问的链接 */
a:hover{color: red}  /** 鼠标指针移动到链接上 */
a:active{color: red} /** 正在点击的链接 */

a:hover 必须位于 a:link 和 a:visited 之后
a:active 必须位于 a:hover 之后

text-decoration:none;用于去掉链接的下划线
background-color:red; 用于设置链接的背景颜色

#### CSS使用方法

行内样式（内联样式）

在\<head>标签内添加style样式属性，如 p{font-size: 30px;color:blue;}


内部样式（嵌入样式）

\<head></head>标签内

\<style type="text/css">

样式代码...

\</style>

外部样式表
导入样式

#### CSS选择器

id 选择器

#red{color:red}

\<p id="red">这个段落颜色是红色</p>


类选择器

.center {text-align: center}

``` css
<h1 class="center">
This heading will be center-aligned
</h1>
```


属性选择器

为所有属性名为title的元素设置样式

``` css
    [title]
    {
    color:red;
    }
```

属性和值选择器

为所有属性名为title，值为Hello World的元素设置样式

``` css
[title=W3School]
{
border:5px solid blue;
}
```

匹配所有title值以hello开头，空格分隔的元素，设置样式

``` css

[title~=hello]
{
color:red;
} 


```


匹配所有以en开头，使用-分隔的元素，设置样式


#### CSS继承和层叠

#### CSS优先级

内联样式(元素内部声明样式)->内部样式表(<head>标签内声明样式)->外部样式表（引入样式)->浏览器缺省样式


#### CSS命名规范

#### CSS3

