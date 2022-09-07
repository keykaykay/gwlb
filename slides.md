---
titleTemplate: "%s - zk"
theme: seriph
background: https://source.unsplash.com/collection/94734566/1920x1080
class: "text-center"
highlighter: shiki
lineNumbers: false
drawings:
  persist: false
css: unocss
preload: false
---

# 前端开发

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    什么是前端开发呢？ <carbon:arrow-right class="inline"/>
  </span>
</div>

---

# 什么是前端开发呢？

前端开发, 就是使用 Web 技术(如：HTML,CSS,DOM 和 JavaScript)设计和开发网站应用. 网站应用, 或运行于 Web 平台 之上。

<v-clicks>

那么网页的组成和显示是怎样的呢？

网页显示的过程

1. 用户在浏览器输入一个网站；
2. 浏览器会找到对应的服务器地址，请求静态资源；
3. 服务器返回静态资源给浏览器；
4. 浏览器对静态资源进行解析和展示。

<img src="/public/image-20220712094728310.png" style="height: 200px;"/>

</v-clicks>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# 静态资源的来源

<v-clicks>

1. 使用 HTML 编写网页的结构。（HTML - 超文本标记语言, 通常被称为 HTML, 是被用于创建网页的标准标记语言. Web 浏览器能将 HTML 文件渲染成可见的或者可听到的. HTML 随着线索提示, 语义化地描述了网站的结构, 使它成为一种标记语言, 而不是编程语言.）
2. 使用 CSS 编写网页的样式。 （CSS - 层叠式样式表(CSS)是用于描述外观和格式化标记语言编写的文档的样式表语言. 尽管经常被用来改变用 HTML 和 XHTML 编写的网页和用户界面的样式, 但也可用于任何 XML 文档, 包括纯 XML, SVG 和 XUL. 跟 JavaScript 和 HTML 一样, CSS 是被大多数网站用于为 Web 应用程序创建富有吸引力的网页, 用户界面的一种基础技术, 也为许多移动应用程序创建用户界面.）
3. 使用 Javsscript 编写交互脚本。 （Javsscript - 是一种高级的, 动态的, 无类型的和解释型的编程语言, 它已经在 ECMAScript 语言规范中被标准化. 跟 HTML 和 CSS 一样, JavaScript 是 WWW 内容生成的第三种必不可少的技术; 大多数的网会使用 Javascript, 并且 Javascript 被所有现在 Web 浏览器支持. JavaScript 基于原型和函数优先的特点, 使它成为多范型的语言, 支持面向对象的, 命令式的, 和函数式编程风格. JavaScript 能提供 API 来处理文本, 数组, 日期和正则表达式, 但不包括任何 I/O, 如网络, 存储或图形工具, 对这些的依赖取决于宿主环境中嵌入了什么. ）
4. 开发项目（HTML/CSS/<span class="text-#ff6c44">Javsscript</span>[Vue、React]）
5. 打包、部署项目到服务器里面

</v-clicks>

---

# 世界上第一个网页

<v-clicks>

- 上世纪 90 年代，Berners-Lee 上线了世界上第一个网站：[World Wide Web](http://info.cern.ch/hypertext/WWW/TheProject.html)

<img src="/public/image-20220712095535678.png" style="height: 180px;"/>

- 现代的网页

<img src="/public/image-20220712095709869.png" style="height: 180px;"/>

</v-clicks>

---

# 网页的组成

<v-clicks>

- 阶段一： HTML 元素
- 阶段二： HTML 元素 + CSS 样式
- 阶段三： HTML 元素 + CSS 样式 + JavaScript 交互

<img src="/public/image-20220712095832216.png" style="height: 150px;"/>

- 例如：
  <img src="/public/image-20220712100021763.png" style="height: 150px;"/>

</v-clicks>

---

# 服务器

<v-clicks>

- 服务器本质上也是一台类似于电脑一样的主机；
- 这个主机有几个特点：
- 二十四小时不关机（稳定运行）
- 没有显示器
- 一般装的是 linux 操作系统（例如 Centos）
- 目前公司大部分使用的是云服务器（比如阿里云、腾讯云、华为云等）
  <img src="/public/image-20220712095323492.png" style="height: 150px;"/>

</v-clicks>

---

# 浏览器

一般而言，编写的 HTML,CSS,JavaScript 代码运行在 web 浏览器。

<v-clicks>

- 最常见的 web 浏览器有：
  - Chrome
  - Internet Explorer
  - Firefox
  - Safari
- 浏览器最核心的部分是渲染引擎（Rendering Engine），一般也称为”浏览器内核“
  - 负责解析网页语法，并渲染（显示）网页
- 常见的浏览器内核有
  - Trident（三叉戟）：IE、360 安全浏览器、搜狗高速浏览器、百度浏览器、UC 浏览器；
  - Gecko（壁虎）：Mozolla Firefox；
  - Presto（急板乐曲） --> Blink(眨眼)：Opera；
  - Webkit：Safari、360 极速浏览器、搜狗高速浏览器、移动端浏览器（Android、iOS）；
  - Webkit --> Blink：Google Chrome；
- 不同的浏览器内核有不同的解析、渲染规则，所以同一网页在不同内核的浏览器中的渲染效果也可能不同;

</v-clicks>

---

# JavaScript

JavaScript 是一门高级编程语言。

<v-clicks>

- 常见的编程语言

<div class="flex justify-around">
  <img src="/public/09.png" style="height: 300px;"/>
  <img src="/public/10.png" style="height: 300px;"/>
</div>
</v-clicks>

<style>
  h1 {
    color: #ff6c44 !important;
  }
</style>

---

# 编程语言的发展

<v-clicks>

- 阶段一: 机器语言
  - 计算机的存储单元只有 0 和 1 两种状态，因此一串代码要让计算机“读懂”，这串代码只能由数字 0 和 1 组成。
  - 像这种由数字 0 和 1 按照一定的规律组成的代码就叫机器码，也叫二进制编码。
  - 一定长度的机器码组成了机器指令，用这些机器指令所编写的程序就称为机器语言。
    <img src="/public/11.png" style="height: 90px;"/>
- 优点:
  - 代码能被计算机直接识别，不需要经过编译解析；
  - 直接对硬件产生作用，程序的执行效率非常高；
- 缺点:
  - 程序全是些 0 和 1 的指令代码，可读性差，还容易出错；
  - 不易编写

</v-clicks>

---

# 汇编语言

<v-clicks>

- 阶段二: 汇编语言
  - 为了解决机器语言的缺陷，人们发明了另外一种语言——汇编语言。
  - 这种语言用符号来代替冗长的、难以记忆的 0、1 代码。(mov/push 指令，经过汇编器，汇编代码再进一步转成 0101)
    <img src="/public/12.png" style="height: 90px;"/>
- 优点:
  - 像机器语言一样，可以直接访问、控制计算机的各种硬件设备；
  - 占用内存少，执行速度快；
- 缺点:
  - 第一，不同的机器有不同的汇编语言语法和编译器，代码缺乏可移植性，也就是说，一个程序只能在一种机器上运行，换到其他机器上可能就不能运行；
  - 第二，符号非常多、难记，即使是完成简单的功能也需要大量的汇编语言代码，很容易产生 BUG，难于调试；
- 应用场景
  - 操作系统内核、驱动程序、单片机程序；

</v-clicks>

---

# 高级语言

<v-clicks>

- 阶段三: 高级语言
  - 最好的编程语言应该是什么? 自然语言；
  - 而高级语言, 就是接近自然语言, 更符合人类的思维方式
  - 跟和人交流的方式很相似, 但是大多数编程语言都是国外发明的, 因为都是接近于英文的交流方式
    <img src="/public/13.png" style="height: 90px;"/>
- 优点:
  - 简单、易用、易于理解，语法和结构类似于普通英文；
  - 远离对硬件的直接操作，使得一般人经过学习之后都可以编程，而不用熟悉硬件知识；
  - 一个程序还可以在不同的机器上运行，具有可移植性；
- 缺点:
  - 程序不能直接被计算机识别，需要经编译器翻译成二进制指令后，才能运行到计算机上；
  - 种类繁多：JavaScript 、 C 语言、C++、C#、Java、Objective-C 、Python 等；

</v-clicks>

---

# 认识 JavaScript

<v-clicks>

- 维基百科对 JavaScript 的定义:
  - JavaScript（通常缩写为 JS）是一种高级的、解释型的编程语言；
  - JavaScript 是一门基于原型、头等函数的语言，是一门多范式的语言，它支持面向对象程序设计，指令式编程，以及函数式编程；
- 通俗的说法:JavaScript 是一门高级编程语言, 是前端开发的重要组成部分!
- HTML 和 CSS 也是前端开发的重要组成部分, 而 JavaScript 是前端开发的灵魂;

- ECMAScript 是 JavaScript 的标准，描述了该语言的语法和基本对象。

  - JavaScript 是 ECMAScript 的语言层面的实现;
  - 因为除了语言规范之外，JavaScript 还需要对页面和浏览器进行各种操作;
  - 除了基本实现之外，还包括 DOM 操作和 BOM 操作;

</v-clicks>

---

# JavaScript 的运行

<v-clicks>

- 不同的浏览器有不同的内核组成

- Gecko：早期被 Netscape 和 Mozilla Firefox 浏览器浏览器使用；
  - Trident：微软开发，被 IE4~IE11 浏览器使用，但是 Edge 浏览器已经转向 Blink；
  - Webkit：苹果基于 KHTML 开发、开源的，用于 Safari，Google Chrome 之前也在使用；
  - Blink：是 Webkit 的一个分支，Google 开发，目前应用于 Google Chrome、Edge、Opera 等；
  - 等等...
- 常说的浏览器内核指的是浏览器的排版引擎：排版引擎（layout engine），也称为浏览器引擎（browser engine）、页面渲染引擎（rendering engine）或样版引擎。
- JavaScript 代码由 JavaScript 引擎来执行。

</v-clicks>

---

# JavaScript 引擎

<v-clicks>

- 为什么需要 JavaScript 引擎呢？

  - 我们前面说过，高级的编程语言都是需要转成最终的机器指令来执行的；
  - 事实上我们编写的 JavaScript 无论你交给浏览器或者 Node 执行，最后都是需要被 CPU 执行的；
  - 但是 CPU 只认识自己的指令集，实际上是机器语言，才能被 CPU 所执行；
  - 所以我们需要 JavaScript 引擎帮助我们将 JavaScript 代码翻译成 CPU 指令来执行；

- 常见的 JavaScript 引擎有哪些呢？
  - SpiderMonkey：第一款 JavaScript 引擎，由 Brendan Eich 开发（也就是 JavaScript 作者）；
  - Chakra：微软开发，用于 IT 浏览器；
  - JavaScriptCore：WebKit 中的 JavaScript 引擎，Apple 公司开发；
  - V8：Google 开发的强大 JavaScript 引擎，也帮助 Chrome 从众多浏览器中脱颖而出；
  - 等等...

</v-clicks>

---

# 浏览器内核和 JavaScript 引擎的关系

<v-clicks>

- 以 WebKit 为例，WebKit 事实上由两部分组成的：

  - WebCore：负责 HTML 解析、布局、渲染等等相关的工作；
  - JavaScriptCore：解析、执行 JavaScript 代码；

- 小程序中也是这样的划分：
  - 在小程序中编写的 JavaScript 代码就是被 JSCore 执行的；

<img src="/public/14.png" style="height: 200px;"/>

</v-clicks>

---

# JavaScript 应用越来越广泛

<v-clicks>

- Stack Overflow 的创立者之一的 Jeff Atwood 在 2007 年提出了著名的 Atwood 定律：
  - Any application that can be written in JavaScript, will eventually be written in JavaScript.
  - 任何可以使用 JavaScript 来实现的应用都最终都会使用 JavaScript 实现。

<img src="/public/15.png" style="height: 300px;"/>

</v-clicks>

---

# 练习一

```js {monaco}
// 合并多个操作步骤
(function () {
  if (location.href.includes("http://www.network-science.de/ascii/")) {
    window.frames[0].document.querySelector("select[name=FONT]")
      .selectedIndex++;
    window.frames[0].document.querySelector("input[type=image]").click();
  }
})();
```

---

# 练习二

```js {monaco}
// 从百度图片批量下载
(function () {
  if (location.href.includes("https://image.baidu.com/search/")) {
    document.querySelectorAll(".main_img").forEach((img) => {
      const src = img.src;
      setTimeout(() => {
        fetch(src).then((res) => {
          res.blob().then((blob) => {
            const blobUrl = window.URL.createObjectURL(blob);
            const filename = `${new Date().getTime()}`;
            const a = document.createElement("a");
            a.href = blobUrl;
            a.download = filename;
            a.click();
            window.URL.revokeObjectURL(blobUrl);
          });
        });
      }, 2000);
    });
  }
})();
```

---

<div class="h-full w-full flex justify-center items-center">
  <h1 class="text-center text-6xl!">感谢大家</h1>
</div>
