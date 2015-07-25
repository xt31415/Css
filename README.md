网页设计:重置CSS样式表

网页设计，让人最头疼的莫过于让页面兼容各大浏览器，准确些是兼容它们“默认”的CSS样式表。这样，“抹掉”这些默认样式表成了首要问题，也就有了CSS样式表重置一说，目前用的最多的，也是自己现在正在用的方法是，添加以下代码：

第一种方式
* {margin:0px; padding:0px;}
    
现在众多的设计师发现，这行代码虽然简单，但却让网页解析太慢，呵呵，当然了，自己是业余的，不用太在意。
于是出现了几种CSS重置方法：

第二种方式
NETTUTS上的 Jeffrey Way写了篇文章Weekend Quick Tip: Create Your Own Simple Reset.css File
释出自己用来重置CSS样式表的方法

body, html, div, blockquote, img, label, p, h1, h2, h3, h4, h5, h6, pre, ul, ol,
li, dl, dt, dd, form, a, fieldset, input, th, td
{margin: 0; padding: 0; border: 0; outline: none;}
body{line-height: 1;font-size: 88% /* Decide for yourself if you want to include this. */;}
h1, h2, h3, h4, h5, h6{font-size: 100%;padding: .6em 0;margin: 0 15px;}
ul, ol{list-style: none;}
a{color: black;text-decoration: none;}
a:hover
{text-decoration: underline;}
.floatLeft{float: left;padding: .5em .5em .5em 0;}
.floatRight{float: right;padding: .5em 0 .5em .5em;}
    
这个方法适用于大多数的网页设计。

第三种方式
一部分人追求彻底抹去浏览器影响

html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, font, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td {
        margin: 0;
        padding: 0;
        border: 0;
        outline: 0;
        font-size: 100%;
        vertical-align: baseline;
        background: transparent;
}
body {line-height: 1;}
ol, ul {list-style: none;}
blockquote, q {quotes: none;}
blockquote:before, blockquote:after,
q:before, q:after {content: '';content: none;}

/* remember to define focus styles! */
:focus {outline: 0;}

/* remember to highlight inserts somehow! */
ins {text-decoration: none;}
del {	text-decoration: line-through;}

/* tables still need 'cellspacing="0"' in the markup */
table {border-collapse: collapse;border-spacing: 0;}
第四种方式
还有今天sofish提到的Yahoo的YUI提供的CSS重置文件

body,div,dl,dt,dd,ul,ol,li,h1,h2,h3,h4,h5,h6,pre,form,fieldset,input,textarea,p,blockquote,th,td {
        margin:0;
        padding:0;
}
table {border-collapse:collapse;border-spacing:0;}
fieldset,img { border:0;}
address,caption,cite,code,dfn,em,strong,th,var {font-style:normal;
font-weight:normal;}
ol,ul {list-style:none;}
caption,th {text-align:left;}
h1,h2,h3,h4,h5,h6 {font-size:100%;font-weight:normal;}
q:before,q:after {content:'';}
abbr,acronym { border:0;}
这些，没有谁好谁坏一分，大多数设计师并不推荐第一种方法，因为我国的抄袭美德，现在搜索到的CSS网页设计技巧，第一位却一定是这个。






html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed, 
figure, figcaption, footer, header, hgroup, 
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
	margin: 0;
	padding: 0;
	border: 0;
	font-size: 100%;
	font: inherit;
	vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article, aside, details, figcaption, figure, 
footer, header, hgroup, menu, nav, section {
	display: block;
}
body {
	line-height: 1;
}
ol, ul {
	list-style: none;
}
blockquote, q {
	quotes: none;
}
blockquote:before, blockquote:after,
q:before, q:after {
	content: '';
	content: none;
}
table {
	border-collapse: collapse;
	border-spacing: 0;
}
