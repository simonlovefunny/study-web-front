## HTML

元素=开始标记+内容+结束标记


知识点


id为元素标识符，id在页面中必须唯一，name可以不唯一


路径 由于html使用的默认路径是当前文件夹，因此返回上层路径需要在url中添加../,需要返回几级就添加几个../

嵌套 一个元素中放置另一个元素称为嵌套（想象俄罗斯套娃）

引用 

    <q></q> 短引用，使用双引号包裹内容

    <blockquote></blockquote> 

void 元素  在开始标记和结束标记之间没有任何内容的元素,没有实际内容

    <br> 换行

    <img src=""  alt=""  width="" height="" > 显示图像 src标签为图像的读取路径

alt为图像未能正确显示时的提示信息
 
width和height告诉浏览器图像的大小，单位为像素数

``` html

<html>
  <head>
    <!-- 设定页面使用的字符集 -->
    <metahttp-equiv="content-Type"content="text/html;charset=utf-8">  
    <!-- 如果IE9浏览器使用IE7兼容模式访问，仍然渲染成IE9样式 https://www.cnblogs.com/menyiin/p/6527339.html-->
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">

meta标签解析
https://www.cnblogs.com/yumo1627129/p/7198968.html
<!DOCTYPE html  文档类型声明

```

``` html
<a href="" title=""></a>链接元素 内容为可点击 title标签为鼠标移动到上面的提示信息

<a href="http://wickedlysmart.com/buzz/#Coffee"></a>  直接把可以把页面指到对应的id元素显示的内容

<a target="_blank"  href=""></a>  target="_blank" 会弹出一个新窗口而不是跳转
```

指定target="coffee" 如果多个链接指向同一名字的target，则会在同一个窗口打开，target="_blank"则是每次都创建一个新窗口

列表 

    <ol>列表项前有数字标识  ordered list
	<ul> 列表项前有“·”  unordered list


表格
  
	<table>表格元素
	<tr>表格的一行
	<th>表格头的一个单元格
	<td>表格中的一个单元格

``` html
  <table>   <!-- 表格开始 -->
    <tr>    <!-- tr行标签  -->
        <td>....</td>
        ....
    </tr>
    <tr>    <!-- tr行标签  -->
        <td>....</td>
        ....
    </tr>
    .....
  </table>

``` 

表格优化标签（可以按照thread，tbody，tfoot分步进行加载）

thread 表格头（表格标题）

tbody 表格的主体（数据主体）

tfoot 表格的脚（表格的脚注）  

table 可选属性

| 属性    | 值      | 描述    |
| ------  | ------ | ------ |
| align | left，center，right | 规定表格相对周围元素的对齐方式|
| bgcolor | rgb(x,x,x)，#xxxxxx，colorname | 规定表格的背景颜色 |
| border  | pixels|规定表格边框的宽度 |
|cellpadding |pixels，% |规定单元边沿与其内容之间的空白 |
|cellspacing| pixels，% | 规定单元格之间的空白|
|frame | void，above，below，hsides，lhs，rhs，vsides，box，border |规定外侧边框的哪个部分是可见的|
|rules |none，groups，rows，cols，all |规定内侧边框的哪个部分是可见的|
|summary |text |规定表格的摘要 |
|width | %，pixels | 规定表格的宽度 |


表单

\<form> 标签用于为用户输入创建 HTML 表单


    <input type="类型属性" name="名称" .../>

input type
    
| type | 描述    |
| ------  | ------ | 
| text |  文字域|
| password  | 密码域 |
| file | 文件域 | 
| checkbox | 复选域 | 
| radio | 单选域| 
| Button | 按钮| 
| Submit | 提交按钮 | 
| Reset | 重置按钮 | 
| Hidden | 隐藏域 | 
| image | 图像域 | 


工具

http://validator.w3.org W3C的HTML页面检测工具

前端特殊符号 https://blog.csdn.net/qq_33559304/article/details/53147577