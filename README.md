# mypUI

**快速开发nvue页面的组件库与工具集**

- nvue页面，兼容vue页面；
- 纯flex布局，符合weex规范；
- 规范与统一，确保代码质量和开发效率；
- 可配置主题；
- 细节开放到位，在好用和可灵活适配之间把握到位；
- request/router/share...各种工具集；

# 出发点
2019年下半年开始接触uni-app，从vue到nvue，然后到v3，经历了几次迭代，经历过几次提速。我也算是最先拥抱nvue，一路踩坑过来的。

自从有了nvue之后，虽然很多应用都不需要上线app端，我还是统一使用了nvue页面来进行开发（除开canvas页面依然使用的是vue）。

有些人可能纠结，也可能徘徊：到底使用vue页面还是nvue页面。

说说我的情况：

- 我多年前在用Objc/Swift做iOS原生开发，也用Python做后台开发，后来B站代码泄露，又搞了一下go。因为偶尔需要写后台管理页面，就使用Vue+elementUI+vue-element-admin写过js，期间看过几次flex布局和css动画的内容，有一个大概的css基础；
- 用flex做排版，个人感觉很舒服，很规范。其实我个人比较喜欢flex布局（实际上我对其它的一些css排版的规则也不太了解）；

那为什么使用nvue页面？

实际上我们对开发的要求主要有几点：

- 规范；
- 质量；
- 效率；

规范包含了好几个方面：

- 技术范围（使用哪些技术，哪些语法特性）；
- 代码的组织结构（项目内代码的结构）；
- 命名规则等（代码的可读性）；
- 复用与模块化（代码的复用）；
- 接口与字段的管理；
- ...

我们通过规范来尽量确保：

- 项目结构清晰，新人上手快（简单熟悉一下代码结构和目录就能接手项目，而且照着样同样写有规范保证的代码）；
- 代码可维护性好，可读性好，清晰且模块化，易于定位问题和解决问题，同样易于复用和修改；
- 协同成本低；
- 更少的bug；
- 更熟练的开发；

规则越少，越简单，上手越快，熟练越快，用起来得心应手，事半功倍。规范不仅对代码的质量有很大的影响，而且也能极大的促进效率。

在规范的基础上开发的代码，自然质量会有一定的保证。

而且功能以及组件的模块化，更易于不断迭代和优化代码，提升质量。各模块命名和字段的规范，使得复用更加方便快捷。

另外，对于效率，还有很重要的一点就是：减少差异化。

我们主要处理以下几点：

- 对外开放的属性以及事件的命名规范；
- 适当抹平各端差异，减少各端单独的配置；
- 尽量所有的页面都是一个模子刻下来，减少独立配置；

我们讲究拿来就用，平等对待，组件或者框架抹平差异，使用时不需要做特殊处理，字段意思明确，不需要重复查看使用手册或者文档。

为此，我们的项目都去除了系统自带的导航栏，tabbar，以及页面外层包裹的scroll。我们只利用uni编译，它与页面内容无关，所有的页面内容都由我们自己管理。

从而：

- 我们没有pages.json的各种配置，它不再不涉及页面的内容；
- 实现各种各样的导航栏，以及动画；
- 想要什么tabbar都可以；
- 灵活的scroll处理方式；
- 页面每一个地方都可以遮挡（当然，小程序自带的胶囊按钮不能被遮挡）；

# 说明

我当时写这套nvue页面的时候，还没有任何一款nvue页面组件在开放或者售卖。

第一版的时候，我其实是根据weex-ui改的。scroll是根据mescroll改的（当时mescroll还不是mixin的形式）。

本来是想着19年双十一就放出来的，只怪自己太懒，拖来拖去就迎来了最艰难的2020.

现在免费开放出来，希望更多的人一起来参与维护，一起开放更多的组件。

其实我的最终目的是搞一个设计软件，设计即uni-app代码，而且是nvue代码，减少大量的开发时间，甚至直接通过简短的几句描述就实现页面。

希望对你有用。

# 最后

劝你善良，内心平静，不刻意差评，不恶意差评。
