# React.js-Introduction-For-People-Who-Know-Just-Enough-jQuery-To-Get-By
写给熟悉 jQuery 者的 React.js 的入门指南

###目标受众：那些熟悉 jQuery 的人
首先，我要澄清一下我这本书的受众

Zed Shaw，"Learn Code the Hard Way" 系列的作者，最近写了篇博客叫做 " Early v.s. Beginning Coders"。在文章里，Zed 指出声明他们的编程教育材料是面向初学者的，但现实中最不能理解的总是初学者。

我不想犯相同的错误。有的人可能没用过 React;有的可能用过像 Backbone,Ember,Angular 这样的前端 JS 框架，也有的可能很熟悉 JS;也有的可能只知道 jQuery。一个教程对一个群体适合，对另外一个群体可能就不合适了。

这个教程，我只面向上面说的第三个受众群体，也就是：只知道 jQuery 的那些人。下面的几类人可能也适合这个教程：
- 有 HTML/CSS/jQuery 基础的 设计师
- 知道用 jQuery 插件的 wordpress 开发者
- 掌握 HTML/CSS/JS 基础训练的初级开发者
- 会用 bootstrap 和 jQuery 完成他们的前端需求的后端开发者

如果你觉得其他的 JS 框架像 Backbone/Ember/Angular 很适合你，那么这个教程可能不适合你。

如果你已经知道 React，你可能会非常不高兴，因为我大部分讲的都是关于 `States`而不是改变和优化。但是我发现先讲 `states`对那些 jQuery 开发者来说是最好的方式告诉他们为啥 REact 这么叼。

好了，让我们开始吧！

###时间估计： 1-2两个小时
如果你速度足够快，这个教程应该还不要1个小时，如果你学的慢，可能要超过两个小时。

### 概观： 我们将创建一个"推特发布框"
许多的 React.js 教程开始都是解释 React 是怎么工作的，怎么怎么叼，我这个教程不是。

相反的，我们会马上创建一个简单的界面，交替使用 jQuery 和 React 实现。解释这两种实现方式的不同之处。

我们将要创建的界面是和 twitter 的发布界面一样的。它可能不是完全一样，但还是十分像的。希望您能照着这个例子实践。
![推特发布框](http://reactfordesigners.com/images/labs/tweet-box.png)

###第一步：介绍 JSBin
后面的学习我们都将代码写在 JSBin 上面，一个HTML/CSS/JS 的在线编辑器，支持 jQuery 和 React.js。下面就是一个简单的例子：
<a class="jsbin-embed" href="http://jsbin.com/lijufi/embed?html,css,js,output">JS Bin on jsbin.com</a><script src="http://static.jsbin.com/js/embed.min.js?3.34.0"></script>
在左边修改 HTML 代码，右边就能看到修改后的代码

####创建 JSBin 帐号
如果你没有 JSBin 的帐号，去 jsbin.com 创建一个帐号。创建完之后，你可以克隆公共的 JSbin 代码去你的帐号，就是克隆公共的 Github 代码仓库
一样。

