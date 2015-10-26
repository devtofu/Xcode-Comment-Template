# XcodeCommentDesign
![image](https://github.com/devtofu/XcodeCommentDesign/blob/master/images/screenshot.jpg?raw=true)

Xcode 注释设计。
# Overview

最近看到群里的 @神父 ，@Jasper 相继发了 Linux 的 欢迎图，觉得很有意思，请教他们之后，为了方便创建文件自动添加图案注释，做了一个 Xcode 模版，队友看到了也问我怎么弄的，所以就写一下总结吧。

# Description
这个东西叫做 ASCII 文字拼图，可以将文字、图片转换成 ASCII 图案。

# How to do?

### 一、设计注释图案
- [这里有一个在线设计网站](http://www.ascii-art-generator.org/) 

- 进入网站会看到编辑区域,有三种转换方式选择

![step1](https://github.com/devtofu/XcodeCommentDesign/blob/master/images/step1.png?raw=true)


- 一共有以下几种字体样式，[这里截了样式预览图](https://github.com/devtofu/XcodeCommentDesign/tree/master/Preview)

![step2](https://github.com/devtofu/XcodeCommentDesign/blob/master/images/step2.png?raw=true)

- 这里只展示第三种文字图案方式，在 **Banner Text** 中输入想要的英文，点击 **Start** 就出现了你想要的图案了。

### 二、制作模版
制作时使用的是 Xcode 7.0，其他版本路径可能会有所不同。

- 依次进入路径
	- `Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/Library/Xcode/Templates/File Templates/Source/`
	- 复制 `Cocoa Touch Class.xctemplate` 模版，重命名 `Tofu Cocoa Touch Class.xctemplate`
	- 进入 `Tofu Cocoa Touch Class.xctemplate`,里面是 Swift 和 OC 的类，打开文件将上面设计好的注释粘贴到头部即可
		![step3](https://github.com/devtofu/XcodeCommentDesign/blob/master/images/step3.png?raw=true)
		![step4](https://github.com/devtofu/XcodeCommentDesign/blob/master/images/step4.png?raw=true)
	- 这里制作的是文件模版，制作工程模版步骤相同

- 接下来打开Xcode,选择 `File -> New -> File` 或使用快捷键 `⌘ + N`，选择刚刚创建的 Source 模版，到此就全部完成了。

	![step5](https://github.com/devtofu/XcodeCommentDesign/blob/master/images/step5.png?raw=true)


# License
MIT