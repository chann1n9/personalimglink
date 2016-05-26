#Markdown与写作环境
* [前言](#qianyan)
* [Markdown](#markdown)
* [关于自己的工作环境](#gzhj)
	* [Mou](#mou)
	* [Markdown Here](#mh)
	* [利用Github挂载图片](#github)
	
<h2 id=qianyan>前言</h2>	
&emsp;&emsp;原本是没有打算写关于Markdown的文章的，虽然这个玩意很高大上，但是写的人太多了。从介绍这种“标记语言”到具体的教程用法，类似于“Markdown从入门到放弃”等等。各路大大都在写Markdown的文章上6的飞起。但是自从我开始用Markdown写文章后，各路评价颇高，要我介绍一下自己的方法。那么这篇文章重点在**工作环境**的介绍和搭建上，关于Markdown语法本身并不过多提及。为什么我又想说。。  
![qibumeizai](https://github.com/JackMcKing/personalimglink/blob/master/img/mackup/u=722202751,1489560279&fm=21&gp=0.jpg?raw=true)</br></br>
<h2 id=markdown>Markdown</h2>  
&emsp;&emsp;还是得简单介绍一下Markdown这个家伙。简单来说，它不是一门计算机语言，却假装是计算机语言的样子，但是行家里手一定看着类似于这样"\</>"的家伙们明白起来。这是一门**标记语言**啊。利用一些标记，就可以让文本变成自己想要的样子，有点类似于写app时的“layout”文件，也是用标记的形式告诉编译器我想要的UI的样子。</br></br>
&emsp;&emsp;为了直观感受，上一张此时此刻的截图  
![mou](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/mou.png?raw=true)  
<h2 id=gzhj>工作环境以及搭建</h2>  
<h3 id=mou>Mou</h3>
---
&emsp;&emsp;正如上面截图，我在MacBook上码字用的是Mou，最大的感受是轻便、美观，还有就是对新手很重要的实时预览功能。</br></br>
&emsp;&emsp;还是遵从国际惯例，想要了解一个电子产品或软件，首先打开它的设置。我们摁下command+逗号打开，是这样的：  
![shezhi](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/shezhi.png?raw=true)  
&emsp;&emsp;分别是一般设置、编写环境设置（左半边屏幕的字体字号设置，纯粹为了写的时候好看点，比如我不要脸的设置了娃娃体，14pt大小）、主题设置（其实就是左半边背景颜色）、css（重头戏）、tumblr分享以及Scriptogram。</br></br>
&emsp;&emsp;我们先来讲最后一个Scriptogram，为什么呢，因为这个东西已经：  
![script](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/script.png?raw=true)  
如果你觉得不明白，谷歌翻译来帮忙  
![script2](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/scipt2.png?raw=true)</br></br>
&emsp;&emsp;等一下！不要揍我，我们来切入真正的重头戏：**CSS**</br></br>
&emsp;&emsp;CSS经常和HTML、XML一起出现，那么也就显而易见，这是一门关于编写网页的语言：  
>层叠样式表（英语：Cascading Style Sheets，简写CSS），又称串样式列表、级联样式表、串接样式表、层叠样式表、階層式樣式表，一种用来为结构化文档（如HTML文档或XML应用）添加样式（字体、间距和颜色等）的计算机语言，由W3C定义和维护。目前最新版本是CSS2.1，为W3C的推荐标准。CSS3现在已被大部分现代浏览器支持，而下一版的CSS4仍在开发过程中。

&emsp;&emsp;所以可以粗略的认为CSS是为HTML打下手的，用来规定字体大小、样式、背景balabala的，那么也许你已经发现，和我们今天的主题正好相关：**利用CSS来配置Markdown样式**</br></br>
&emsp;&emsp;那么我们打开设置里CSS的标签  
![css](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/css.png?raw=true)  
发现非常简洁：就是一个选择配置文件一样的选择CSS文件，右边一个编辑，一个重载。我们点击Edit，就可以跳转到finder下Mou的CSS文件的路径  
![findercss](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/findercss.png?raw=true)  
如图他默认竟然是emacs打开，作为vim党，作为圣战的一份子，果断用command+option+c复制CSS文件夹路径，并在terminal中打开  
![vim](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/vim.png?raw=true)  
![vim2](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/vim2.png?raw=true)  
看起来和谐安康多了。主要注意的是路径当中的那个"Application Support"一定要加引号！或者中间空格前面加“\”，否则shell会把空格后面的当做命令，就会报错。</br></br>
&emsp;&emsp;那么文件打开了，我们是不是还需要学CSS才会读，才会写？我看着你们可求得大眼睛，露出一丝激动人心地笑说：  
>对啊

&emsp;&emsp;其实也不用很彻底的学，我们只需要一些浅显的东西，只要Google一下“CSS语法”，便会出来一堆速成的学习大纲，看个一两眼，再加上CSS本身可读性就很高。起码用个几分钟就可以在原来的CSS文件上改出像模像样的东东啦。</br></br>
&emsp;&emsp;如果微信支持的话，大家可能会看到我大标题改了样式，左边会有一节奇怪的颜色。因为第一次用，所以如果不支持请留言吐槽。在这里放上截图：  
![lizi](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/lizi.png?raw=true)  
如果支持的话那么我会认真的调个色出来，固定位我写的文章的主题色。那么先放上这个配置的源码：  
`h0{
  font-size: 1.4em;
  margin: 40px 10px 20px 0;
  padding-left: 9px;
  border-left: 6px solid #70C0D2;
  font-family: "sans serif";
  color:#4F5154;
}
`  
&emsp;&emsp;每个Markdown里的CSS文件里都是有h1到h6的，分别定义六个级别的标题，这里我定义了h0，是传说中的“McKing专用标题（beta）”，用的是和二级标题一样的大小1.4em。</br></br>
&emsp;&emsp;说到调色，还真得说说一个调色神器：基于Alfred2的workflow功能开发的“colors”，这里是网站：`http://www.packal.org/workflow/colors`,就是这货：  
![color](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/color.png?raw=true)  
我这个颜色就是这样用hsl的形式调出来，然后转换成“#70C0D2”的，当然，最神奇的是它还能用command+回车调处OSX的调色盘，可视化高多了，然后再转化，岂不更美哉~  
![color2](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/colorface.png?raw=true)  

<h3 id=mh>Markdown Here</h3>
---
&emsp;&emsp;这是一款chrome插件。功能是把markdown文本选中后，摁一下，就转化成富文本（rich text），也就是给大家看的样子。曾经以图表巨丑、抽出天际出名，后来可能大家给他集资找了个好的设计师搞了个还看得过去的图标，就这货：  
![mdhere](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/mdhere.png?raw=true)  
使用发发相当的简单，比如我在Mou里写好了markdown文本，然后用chrome打开微信公众号的编辑界面，把Mou里的文本粘贴进去，全选，一摁这个chrome右上角的小按钮，就变成了富文本的样子，供大家观瞻。</br></br>
&emsp;&emsp;那么它有没有CSS来配置它呢？当然有。右键这个小图标，打开选项，可以看到这样：  
![mdshezhi](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/mdshezhi.png?raw=true)  
![mdshezhi2](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/mdshezhi2.png?raw=true)  
基本就这个样子，那个“基本渲染CSS”就是配置文件，掌管着你摁下那个小按钮的时候它以什么样的姿势为你服务（误），咳咳！它以什么样的形式转化成富文本。而下面的预览则是你可以输入一段markdown试一试你的CSS生效没有，比如这样：  
![mdshezhi3](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/mdshezhi3.png?raw=true)  
这就是定义的七种标题形式。</br></br>
&emsp;&emsp;然而更神的是这货竟然支持数学公式转换！这就很神奇了，上面也有详细说明这个服务是谷歌的，理论基本上就是把你写的这个markdown发过去，它生成公式再以图片形式发过来。也就是说微信是没法用了，因为不支持外链图片，更与谷歌无缘。(容我吐槽一句，在中国的互联网生活，太痛苦了)  

<h3 id=github>利用Github挂载图片</h3>
---
&emsp;&emsp;众所周知Markdown在文中插入图片的方式就是利用连接。那么我们就需要找到一个挂载的地方。当然微信我就不吐槽了，只支持挂载在它自己上面。我需要一张一张上传上去，可能是方便审核吧。而大部分非国产平台都是支持外链图片的，这样也确实更方便，更省财力、人力。作者写着舒服，平台也不需要占用服务器资源和储存空间来存放这些图片。两全其美。</br></br>
&emsp;&emsp;比较知名的挂载图片的地方就是七牛了，很多网站的图片都挂载在上面，但是对于我这种受众两位数的小作者来说，还是有些奢侈了。所以我利用了github，反正访问量也不大，足够用了。</br></br>
&emsp;&emsp;具体方法就是把图片存放的目录以git形式push成为一个repository，然后在今后写作中不断push、commit，周而复始，把图片在github上的链接当做外链，完美解决。</br></br>
&emsp;&emsp;如果不喜欢命令行，Github Desktop可以很完美的解决。高可视化的线程显示模式虽然对我挂在图片没啥用，但是在真正的开源协作中乃是神兵利器：  
![desktop](https://github.com/JackMcKing/personalimglink/blob/master/img/markdown/desktop.png?raw=true)  

<h0>最后</h0>  
&emsp;&emsp;在这欢欣鼓舞的最后，希望我能帮到大家一些实用的东西，写出高颜值的文章。  
![zhifubao](https://github.com/JackMcKing/personalimglink/blob/master/img/mackup/IMG_1390.JPG?raw=true)
