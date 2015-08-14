网页设计:重置CSS样式表


第一种方式
* {margin:0px; padding:0px;}

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

第三种方式
彻底抹去浏览器影响

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
Yahoo的YUI提供的CSS重置文件

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
