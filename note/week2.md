# nomal
## 超連結
```html
<a href="https://www.w3schools.com">Visit W3Schools</a>
```
## 圖片
### 放置圖片
```html
<img src="img_girl.jpg">
<img src="https://www.w3schools.com/images/img_girl.jpg"width="500" height="600">
<img src="https://www.w3schools.com/images/img_girl.jpg"style="width:500px;height:600px;>
```
第二種寫法使用超連結，並調整大小
第三種寫法第二種寫法好
*個人覺得第三種的大小寫法和css較相似
### 點擊圖片到達超連結
```html
<a href="default.asp">
  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a>
```
### alt(萬一圖片跑不出來時的替代文字)
## area
https://www.w3schools.com/html/html_images_imagemap.asp
## style
色碼(#000000)為兩個兩個一組(由左至右分別為R、G、B)，是以16進位的方式寫的
```html
<p style="color:red;">This is a red paragraph.</p>
```
*最好的方法是用css寫(之後會說)
## 語言
```html
<!DOCTYPE html>
<html lang="en">
<body>
...
</body>
</html>
```
## title&tooltip
```html
<h2 title="I'm a header">The title Attribute</h2>

<p title="I'm a tooltip">Mouse over this paragraph, to display the title attribute as a tooltip.</p>

```
游標放在內文或標題處會有附加框框
eg:https://www.w3schools.com/html/tryit.asp?filename=tryhtml_attributes_title
# 各種特別字體
## 字體大小
```html
<h1 style="font-size:60px;">Heading 1</h1>
<h1 style="font-size:300%;">This is a heading</h1>
<p style="font-size:160%;">This is a paragraph.</p>
```
## 空白
&nbsp或中文全行的空白
## 分隔線
```html
<hr/>
```
## 強制換行
```html
<br>
```
## pre取消格式化
```html
<pre>
Text in a pre element
is displayed in a fixed-width
font, and it preserves
both      spaces and
line breaks
</pre>
```
## 置中
```html
<h1 style="text-align:center;">Centered Heading</h1>
<h1 style="text-align:left;">left</h1>
<h1 style="text-align:right;">right</h1>
```

## 特別字體
```html
<p><b>HTML</b>
            <strong>contains</strong>
            <i>several </i>
            <em>elements</em>
            <mark> for</mark> 
            <small>text </small>  
            <del>with </del>
            <ins>aaaaaa</ins>
            <sub>special</sub>
            <sup> meaning.</sup></p>
```
https://www.w3schools.com/html/html_formatting.asp

## 引用
```html
<p>Here is a quote from WWF's website:</p>
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 50 years, WWF has been protecting the future of nature.
The world's leading conservation organization,
WWF works in 100 countries and is supported by
1.2 million members in the United States and
close to 5 million globally.
```

## 短引號
```html
<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>
```

## 有底線的引用
```html
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
```
## 地址(斜體)
```html
<address>
Written by John Doe.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>
```
## 斜體的標題
```html
<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
```

## 反方向顯示文字
```html
<bdo dir="rtl">This text will be written from right to left</bdo>
```
## 附註
```html
<!-- This is a comment -->
<p>This is a paragraph.</p>
```

## 外框顏色
```html
<h1 style="border:2px Tomato solid;">Hello World</h1>
<h1 style="border:15px Violet solid;">Hello World</h1>
<h1 style="border: 12px skyblue dashed;">Hello World</h1>
```
# CSS使用以大量變更格式
https://www.w3schools.com/html/html_css.asp

# CSS排版
https://www.w3schools.com/css/css_boxmodel.asp
# Html Link
## _target 
### self(可以在該頁面中抵達連結的網址)
```html
<a href="https://www.w3schools.com/" target="_self">Visit W3Schools!</a> 
```
### _blank(在新分頁中開啟連結)
```html
<a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a> 
```
### _parent(在副頁籤中打開網址)
```html
<a href="https://www.w3schools.com/" target="_parent">Visit W3Schools!</a> 
``` 
### _top(在最頂層的視窗打開網址)
```html
<a href="https://www.w3schools.com/" target="_top">Visit W3Schools!</a> 
```
## 相對路徑
```html
<p><a href="/css/default.asp">CSS Tutorial</a></p>
```
```html
<p><a href="/css/cd../default.asp">CSS Tutorial</a></p>
```
* cd..可以返回上一步
* 上下兩種兩者相同(主要是了解cd..的用法)
* 補充:https://www.itread01.com/p/632662.html
* 主要是架網頁上為了便捷，因此相對路徑相當重要
# 表格(table)<<用table 包住表格
## html
http://www.pcnet.idv.tw/pcnet/html/11.htm
### 列
```html
<tr>            </tr>
```
### 欄
<td>            </td>
## css
```html
table {
  font-family: arial, sans-serif; <!--字體-->
  border-collapse: collapse;  <!--讓框線變成一條，而不是兩條-->
  width: 100%;  <!--寬度-->
}

td, th {
  border: 1px solid #dddddd;  <!--線框  線的實虛(可見文字邊框處)  邊框顏色-->
  text-align: left;  <!--文字置左(預設置中)-->
  padding: 8px;  <!--表格格寬-->
}

tr:nth-child(even) {  <!--偶數列-->
  background-color: #dddddd;  <!--表格背景色-->
}
```
# list
## 清單
```html
<li>
```
## ul(無序的)
```html
<ul>                        </ul>
```
## ol(有序的....阿拉伯數字)
```html
<ol>                        </ol>
```
*更詳細:http://www.pcnet.idv.tw/pcnet/html/06.htm
# 表單
```html
<label for="fname">First name:</label><br>
```