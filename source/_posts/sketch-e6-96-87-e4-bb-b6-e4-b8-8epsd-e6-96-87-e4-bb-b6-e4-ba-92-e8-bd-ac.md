---
title: sketch文件与PSD文件互转
url: 1954.html
id: 1954
categories:
  - huhuの文章
date: 2018-04-10 11:04:39
tags:
---

刚才遇到一个很棘手的问题。 前几天在做一套界面，交接给另外的设计师，然而，对方可能是Windows用户。这样，我的sketch文件就不能直接给他用了。 但是，还是有解决方法的。 Photopea，一款可以在线编辑Sketch和PSD源文件的工具，有一个神奇的功能就是在线转换sketch为PSD文件。（使用网址：https://www.photopea.com/） 打开页面，就能看到支持PSD、XCF、Sketch、Any格式。不过这个网站有个最大问题，就是打开图层是中文，都会显示 口口 格子（不要紧，有办法）。 大法开始： 1、打开Photopea网址，选择Open Frome Computer 打开你需要转换的sketch文件； 2、会发现一个页面里面中文全部变成口口 格子，可以不管他（如果有强迫症，后面告诉怎么样显示中文方法）； 3、选择左上角，点击File - 选择Save as PSD, 保存成PSD文件（如果发现没有所选项，有可能是因为浏览器自动翻译了网页导致；如果发现点击了，还是没有转换为PSD，应该是因为没有登录）； ![](http://h2y.net.cn/wp-content/uploads/2018/04/9C3E4C79-B843-4CE9-A764-79CB0769F7A7.jpg) 4、打开PSD文件。 保存后，Chrome浏览器会直接出现底部。（其他浏览器，看你默认下载位置吧）； 5、打开PSD文件，发现还是口口 格子（不要紧）； 6、选择批量替换文字。（注：Sketch的隐藏图层，都会被显示，建议转换前，先将隐藏图层删除。）使用文本图层过滤器，可以仅显示文本，方便替换。 经亲身试验，**除了文字可编辑，其他都变成了图片。** 以下是针对过程中强迫症处理方式！（口口去除） 1、在Photopea打开sketch文件之前，确定，自己设计稿的字体文件。 2、在Photopea打开，选择设计稿字体文件 （支持TTF/OTF字体格式） 提示已经导入。 然后再打开skethc文件，发现中文顺利显示出来。（如果还有口口，就是你的字体不对应） （当然，我们也可以用最原始的方式。我们都知道可以直接复制ai的元素，粘贴到sketch中，同理，也可以从sketch中拖出画板或元素到ai中，然后再转为PSD，这样的好处是，过程可控，放进AI的元素也可以最大程度保留其可编辑性。）   另外，怎么把PSD转换为sketch呢? 有个叫做Avocode的工具（官方下载：[https://avocode.com/convert-psd-to-sketch](https://avocode.com/convert-psd-to-sketch)）， 整个转换操作只要**3 个步骤**： **1、上传需要转换格式的psd源文件；** **2、填写自己的邮箱地址，接收转换成功的 Sketch 文件；** **3、登录自己的邮箱，查看收件箱里的新邮件。** ![](http://h2y.net.cn/wp-content/uploads/2018/04/DB47BBCE-B3FB-40D1-A3E5-2267CDFC41A0.jpg) 转换结果是：

*   **分组和图层——完整保存，基本没有发生变化（有些文字不出现了）。**
*   文件大小大幅缩小。
*   **智能对象**——原Status bar 为智能对象被转化为图片。同样，其他智能对象都被转为图像。
*   **形状和嵌套——保留，形状依旧可以在编辑。**
*   **文本**——保留，但会发生错位，会需要重新调整
*   **形状——保留，按照 Sketch 样式保留布尔运算。**