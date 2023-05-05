---
marp: true
theme: zju
paginate: true
---

<!--
_paginate: false
_class: homePage
-->

![h:120px](../../images/zju/logo_blue.png)

# 这是一个浙大主题的学术PPT模板
## 毕业答辩
**zlt  2023-03-04**

---
<!--
_paginate: false 
_class: contents
-->

## 目录

- **01**Marp
- **02**标题和列表
- **03**代码
- **04**数学公式
- **05**表格
- **06**图片布局
- **07**参考

---
<!-- 
_header: Marp
_class: contentPage
-->

[Marp](https://marp.app/)(Markdown Presentation Ecosystem)是一款可以轻松将Markdown转换为HTML/PDF/PPTX的工具，能让我们专注于PPT的内容而不是排版。如果你是精通Markdown和css的程序员，那么用起来会更加顺手。

- 如果还不会熟练使用Markdown，可以查阅[Markdown中文教程](https://markdown.com.cn/)进行学习。
- 在VS Code中安装[Marp for VS Code](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode)插件。
- 新建Markdown文件（后缀名为`.md`），在头部插入以下代码，点击右上角预览按钮即可实时编辑。

---
<!--
_header: 标题和列表
_class: contentPage
-->

## 二级标题

### 三级标题

普通文字、**加粗文字**、*斜体文字*、~~删除线~~
Markdown一般是使用`-`和`1.`来展示列表，Marp支持使用`*`和`1)`实现逐条显示的动画效果（仅支持HTML，在PDF和PPT只是普通列表）。

1) 第一行
2) 第二行
3) 第三行

* 第一行
* 第二行
* 第三行



---
<!--
_header: 代码
_class: contentPage
-->

### 行内代码

行内代码 `"markdown.marp.mathTypesetting": "mathjax"`

### 代码块

```json
{
  "markdown.marp.breaks": "on", // 渲染换行符
  "markdown.marp.chromePath": "", // 浏览器路径
  "markdown.marp.enableHtml": true, // 启用所有HTML标签
  "markdown.marp.exportType": "pdf", // 默认的导出文件类型
  "markdown.marp.mathTypesetting": "mathjax", // 默认的数学渲染引擎
  "markdown.marp.outlineExtension": true, // 启用大纲视图
  "markdown.marp.pdf.noteAnnotations": true, // 将注释作为备注添加到导出的PDF中
  "markdown.marp.pdf.outlines": "headings", // 在导出的PDF中添加书签
  "markdown.marp.strictPathResolutionDuringExport": false, // 导出禁用严格的路径解析
  "markdown.marp.themes": [ // 声明主题样式文件
    "./themes/companyLightBlue.css",
  ],
}
```

---

<!--
_header: 数学公式
_class: contentPage
-->
Marp支持MathJax、KaTeX这两种主流数学渲染引擎，属性值分别为`mathjax`、`katex`，不同版本Marp默认引擎不一致，建议显式声明，更多信息请查阅[官方文档-Math typesetting](https://marp.app/docs/guide/math-typesetting)。

- 使用`$`符号包裹即可使用行内公式，例如`$ax^2+bc+c$`会渲染为$ax^2+bc+c$。
- 使用`$$`包裹就会渲染为公式块，如：

$$
f(x) =
  \int_{-\infty}^\infty
  \hat f(\xi)\,e^{2 \pi i \xi x}
  \,d\xi
$$

---
<!--
_header: 表格
_class: contentPage
-->

指令分为全局指令（控制所有幻灯片）和局部指令（控制特定幻灯片）。

名称|类型|描述
:---:|:---:|---
**marp**|全局|是否在VSCode中启用Marp。
**theme**|全局|指定样式主题。
**style**|全局|用于快捷调整整体主题的CSS。
**size**|全局|指定幻灯片尺寸比例，内置尺寸有`4:3`、`16:9`、`4K`。
**headingDivider**|全局|在指定级别标题前自动添加幻灯片分隔符。
**math**|全局|指定数学渲染引擎，支持`mathjax`、`katex`。
**paginate**|局部|设置为`true`，将在右下角显示页码。
**header**|局部|指定幻灯片页眉内容，支持内联Markdown。
**footer**|局部|指定幻灯片页脚内容，支持内联Markdown。
**class**|局部|为单页幻灯片外层元素`<section>`设置class属性。

---
<!--
_header: 图片布局
_class: contentPage horizontalImages
-->
`_class`加上`horizontalImages`类名，就可以使图片横向布局，方便插入更多图片。

![h:300px](../../images/zju/cover_bg_1.JPG)
![h:300px](../../images/zju/cover_bg_2.JPG)
![h:300px](../../images/zju/cover_bg_4.jpg)

---
<!--
_header: 参考
_class: contentPage
-->

> - [Marp官方文档](https://marpit.marp.app)
> - [Marp-theme](https://github.com/marp-team/marp-core/blob/main/themes)
> - [Marp-Theme-UCAS](https://github.com/BeWaterMyFriend7/Marp-Theme-UCAS)

---

<!--
_paginate: false
_class: thanksPage
-->

## 请各位老师批评指正

<br/>

**zlt 2023-03-04**
