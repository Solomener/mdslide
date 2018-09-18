## MD & Reveal.js 简易指北

===

为什么要使用 Markdown 写幻灯片?

* 纯文本，专注写作。
* 版本控制 

Note: 这是**小技巧**页的笔记。

===

## 规范定义

* 水平方向使用 [`===`](javascript:) 分隔
* 竖直方向使用 [`---`](javascript:) 分隔
* 内容以[Note:](javascript:) 可作为幻灯片的演讲者备注

===

水平页 1 - 竖直页 1

---

水平页 1 - 竖直页 2

===

水平页 2 - 竖直页 1

---

水平页 2 - 竖直页 2

===

## 小技巧

* 按 [ESC](javascript:) 键可打开 大纲模式
* 按 [S](javascript:) 键打开 演讲笔记窗口
* 在 URL 后加入 **?print-pdf** 即可[打印](?print-pdf)
* 本页面加入查询参数url=filename.md  即可加载自定义 markdown 文件
* 现已集成 chalkboard 等插件，左下角按钮可以使用白板
* 其他插件具体请查看源码

Note: 这是**小技巧**页的笔记。

===

## Markdown语法测试

*斜体*  **粗体** ~~删除线~~ [链接](http://github.com)

> 文字引用

图片：![pic](https://www.baidu.com/img/bd_logo1.png)

> 图片请使用外链或者相对路径

---

行内代码块：`echo Hello NCUTEA!` (部分主题不明显)

多行 C 代码块：

```c
#include <stdio.h>
int main(void){
    printf("Hello World\n");
    return 0; 
}
```

四个缩进空格代码块：

    #include <stdio.h>
    int main(void){
        printf("Hello World\n");
        return 0; 
    }
    

---

* 无序列表 1
* 无序列表 2
* 无序列表 3

1. 有序列表 1
2. 有序列表 2
3. 有序列表 3

===

## 已知问题

`行内代码块`与**粗体**不明显

临时方案：使用 [无目标链接](javascript:)

BUG: 

*选择文件加载md时，不支持相对路径。*

*markdown 中的相对路径均为相对本页面，而非相对markdown文件*

因此，暂时使用绝对路径

===

## 功能扩展

请参考 revealjs 文档，在 Markdown 内嵌 HTML 代码

---

<section id="transitions">
	<h2>Transition Styles</h2>
	<p>
		You can select from different transitions, like: <br>
		<a href="?transition=none#/transitions">None</a> -
		<a href="?transition=fade#/transitions">Fade</a> -
		<a href="?transition=slide#/transitions">Slide</a> -
		<a href="?transition=convex#/transitions">Convex</a> -
		<a href="?transition=concave#/transitions">Concave</a> -
		<a href="?transition=zoom#/transitions">Zoom</a>
	</p>
</section>

<section data-background="#dddddd">
	<h2>Slide Backgrounds</h2>
	<p>
		Set <code>data-background="#dddddd"</code> on a slide to change the background color. All CSS color formats are supported.
	</p>
	<a href="#" class="navigate-down">
		<img width="256" height="256" data-src="https://ncutea.gitee.io/tutorials/_media/logo.png" alt="Down arrow">
	</a>
</section>
<section data-background="https://ncutea.gitee.io/tutorials/_media/logo.png">
	<h2>Image Backgrounds</h2>
	<pre><code class="hljs">&lt;section data-background="image.png"&gt;</code></pre>
</section>
<section data-background="https://ncutea.gitee.io/tutorials/_media/logo.png" data-background-repeat="repeat" data-background-size="100px">
	<h2>Tiled Backgrounds</h2>
	<pre><code class="hljs" style="word-wrap: break-word;">&lt;section data-background="image.png" data-background-repeat="repeat" data-background-size="100px"&gt;</code></pre>
</section>
<section data-background-video="http://www.runoob.com/try/demo_source/movie.ogg,http://www.runoob.com/try/demo_source/movie.webm" data-background-color="#000000">
	<div style="background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px;">
		<h2>Video Backgrounds</h2>
		<pre><code class="hljs" style="word-wrap: break-word;">&lt;section data-background-video="video.mp4,video.webm"&gt;</code></pre>
	</div>
</section>

<section data-background="http://p0.ifengimg.com/pmop/2017/0428/981698501B4582AF2FDA8CF7E08BAC2A1EE8D0D6_size419_w640_h437.gif">
	<h2 style="color:black;">... and GIFs!</h2>
</section>
