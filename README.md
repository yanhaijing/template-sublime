# [template-sublime](https://github.com/yanhaijing/template-sublime)

[template.js](https://github.com/yanhaijing/template.js)的sublime插件，[点击这里查看](https://github.com/yanhaijing/template-sublime)

## How to install

Way 1: with [Package Control](http://wbond.net/sublime_packages/package_control):

1. Run "Package Control: Add repository" and add https://github.com/yanhaijing/template-sublime
2. Run "Package Control: Install Package" command, find and install `templatejs` plugin.
3. Restart ST2 editor (if required)

Way 2: download and copy

1. Clone or [download] git repo into your packages folder (in ST2, find Browse Packages... menu item to open this folder)
2. Restart ST2 editor (if required)


## Features

- 语法高亮

支持templatejs的模板语法高亮

下面示例如下

```
<h2>我的待办</h2>
<ul>
    <%list.forEach(function(item, index) {%>
        <li>
            <div class="row">
                <div class="col-5 <%=index % 2 ? 'text-secondary' : ''%>">
                    <%=item.text%>
                    <%:=item.text%>
                    <%abc:=item.text%>
                </div>
            </div>
        </li>
    <%})%>
</ul>
<a href="#" class="btn btn-dark add-todo">新增</a>
```

高亮后的效果

![](./img/demo.png)

## CHANGELOG
[CHANGELOG.md](https://github.com/yanhaijing/template-sublime/blob/master/CHANGELOG.md)

## TODO
[TODO.md](https://github.com/yanhaijing/template-sublime/blob/master/TODO.md)

## 参考文档

- [How To Make a Custom Syntax Highlighting for Sublime Text](http://ilkinulas.github.io/programming/2016/02/05/sublime-text-syntax-highlighting.html)
- [官网API](http://www.sublimetext.com/docs/3/syntax.html)
- [如何打包发布](https://packagecontrol.io/docs/submitting_a_package)