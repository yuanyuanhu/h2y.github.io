---
title: App界面交互设计规范之视觉
url: 515.html
id: 515
categories:
  - huhuの文章
date: 2017-04-12 23:44:15
tags:
---

上篇[《APP界面设计风格》](http://www.woshipm.com/ucd/193763.html "App界面设计风格") APP设计规范指对APP界面进行风格统一，对界面元素的样式、颜色和大小设定统一的规范和使用原则。与设计、前端约定好统一的设计规范很重要，约定设计规范可以减少产品、设计、前端的沟通成本；可以使界面设计整洁、统一，减少界面元素的重复设计；可以减少设计素材，控制安装包的大小。 APP设计规范主要包括对界面布局、背景色、字体颜色大小、界面元素间距、弹层、loading、图标、按钮常态点击态等进行统一的梳理和规范。

一、页面布局规范
--------

![244174-681062d1a410283b](http://image.woshipm.com/wp-files/2015/08/244174-681062d1a410283b.png) 页面布局 页面布局和交互规范上建议安卓、ios尽量统一，这样可以避免安卓和ios分别设计一套稿子。当然土豪公司可以忽略这个建议，安卓和ios分别做专门的设计当然更好。在中小型项目来看，设计资源紧张的话可以考虑安卓和ios用同一个稿子，分别做相应的微调后输出适用安卓和ios不同的尺寸要求就可以。 推荐使用mac矢量设计工具”sketch”。以ios平台的iPhone5的尺寸640*1136px作为标准尺寸设计。在界面设计完成后可以做相应的微调导出适用ios和安卓尺寸的稿子。这里可以首先统一设计稿输出规范：

*   安卓（720*1280px）：界面预览图、界面坐标图、标准界面的图标png文件
*   IOS（640*1136px）：界面预览图、界面坐标图、1-3倍图矢量图标pdf文件

PS：界面坐标图指在设计已定稿的界面预览图上标注：界面元素的间距、文字的颜色、文字的字号大小、图标的尺寸、按钮不同状态颜色、按钮的尺寸等等 ![244174-6a9f0032dce8c8af](http://image.woshipm.com/wp-files/2015/08/244174-6a9f0032dce8c8af.png) 界面坐标图实例

二、标准色规范
-------

![244174-dd76e93c198cce22](http://image.woshipm.com/wp-files/2015/08/244174-dd76e93c198cce22.png) 标准色规范 标准色规范：重要、一般、弱。标准色重要：重要颜色中一般不超过3种，这里的例子重要颜色之一红色需要小面积使用,用于特别需要强调和突出的文字、按钮和icon；而黑色用于重要级文字信息比如标题、正文等。 标准色一般都是相近的颜色，而且要比重要颜色弱，普遍用于普通级信息、引导词比如提示性文案或者次要的文字信息。标准色较弱：普遍用于背景色和不需要显眼的边角信息。 ![244174-64832b9214e30e9c](http://image.woshipm.com/wp-files/2015/08/244174-64832b9214e30e9c.png) 标准色实例

三、标准字规范
-------

![244174-53a10bf40b54e19b](http://image.woshipm.com/wp-files/2015/08/244174-53a10bf40b54e19b.png) 标准字规范 文字是APP主要信息的表现，尤其新闻阅读、社区APP等制定标准的设计规范和良好的排版方式，用户使用APP也觉得毫无疲劳感，这一点很重要。标准字规范重要、一般、弱。这里主要规范标准字的大小，标准字要注意跟上文的标准色进行组合突出APP重要的信息和弱化次要的信息。标准字重要：大字号普遍用于大标题、top导航，较小字号用在分割模块的标题上。标准字一般：主要用在大多数文字，比如正文。标准字弱：普遍与标准色较弱组合用于辅助性文字如一些次要的文案说明。 ![244174-5b6ff350de69686e](http://image.woshipm.com/wp-files/2015/08/244174-5b6ff350de69686e.png) 标准字实例

四、界面元素间距
--------

![244174-4fe880e3fc14accb](http://image.woshipm.com/wp-files/2015/08/244174-4fe880e3fc14accb.png) 界面元素间距 APP界面要给人简洁整齐，条理清晰感，依靠的就是界面元素的排版和间距设计。这里间距设计还要注意考虑适配不同的屏幕分辨率。一般解决方案有据屏幕等比放大缩小间距，或者固定某些界面元素的间距，让其他空间留空拉伸。为了满足屏幕分辨率较大的设备，有时甚至需要改变APP界面的页面布局。 ![244174-4af7348becd31f74](http://image.woshipm.com/wp-files/2015/08/244174-4af7348becd31f74.png) 微信iPad版vs微信iPhone版

五、弹层规范
------

![244174-5ac66478727d585e](http://image.woshipm.com/wp-files/2015/08/244174-5ac66478727d585e.png) 弹层规范 弹层规范要注意分别设计安卓和ios的弹层，比如ios大多操作弹层由底部弹出，而安卓直接显示操作再页面中央，这样的交互搞作应该遵循各自平台的设计要求。弹层需求根据不同的功用设计不同的样式。比如操作性弹层-右上角更多按钮触发；提示性弹层：弱提示性的应用系统的token飘字提示即可；需要强提示可以使用取消、确定的模块弹层；更强提示而且弹层需要承载一定操作的使用强引导弹层，右上角提供关闭操作或者可以点击非弹层区域关闭弹层。

六、Loading规范
-----------

![244174-446167c3ecd77e82](http://image.woshipm.com/wp-files/2015/08/244174-446167c3ecd77e82.png) Loading规范 页面loading动画是APP界面必不可少的元素，增加loading可以给用户明确的反馈功能正在加载，减少用户在等待功能响应引起的烦躁感。另外loading动画除了常规的菊花还可以考虑使用npc，让APP更生动、活泼；或者使用logo口号加强APP的品牌形象。 ![244174-8b97e8bd72060c67](http://image.woshipm.com/wp-files/2015/08/244174-8b97e8bd72060c67.png) 次元社、闺蜜圈loading截图

七、图标/按钮规范
---------

![244174-2b523bc2dc22badb](http://image.woshipm.com/wp-files/2015/08/244174-2b523bc2dc22badb.png) 图标按钮规范 图标规范要注意安卓和ios平台需求不同的大小和不同的文件格式：如安卓需要720\*1280px标准页面的png图标格式；ios需要3个尺寸320\*（1-3）倍图的图标pdf文件。图标还应该根据不同的功能需求设计不同的状态：如常态、选中态、点击态等。 按钮规范按状态分有：常态、点击态、不可点击态。按钮规范因不同功能和场景需要，设计不同的样式和颜色，在尺寸上也分有：长、中、短；而且按不同手机平台长中短尺寸也注意有所不同。

八、页面加载失败、页面为空展示
---------------

![244174-ef9853634ac600b1](http://image.woshipm.com/wp-files/2015/08/244174-ef9853634ac600b1.png) 加载失败、页面为空 页面加载失败、页面为空可以统一规范为NPC、文案、按钮。要注意根据不同的场景显示不同的NPC和文案。…… … 设计规范主要由设计童鞋来梳理，但必须要与前端开发、产品经理达成共识，严格遵守约定的规范，否则这个设计规范就毫无意义了。 在制定设计规范过程中，产品经理要积极主动充当桥梁角色组织设计师、前端开发一起制定设计规范，保证设计规范考虑的更切合实际、更全面、更完整。