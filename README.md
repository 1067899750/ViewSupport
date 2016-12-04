# <img src="http://ww2.sinaimg.cn/large/005Xtdi2jw1f4v398j1v3j3074074t8w.jpg" width=32 /> ViewSupport

[![License](https://img.shields.io/badge/license-Apache%202-green.svg)](https://www.apache.org/licenses/LICENSE-2.0)
![](https://img.shields.io/badge/Support-7%2B-green.svg)
[![](https://jitpack.io/v/GcsSloop/ViewSupport.svg)](https://jitpack.io/#GcsSloop/ViewSupport)

![](https://raw.githubusercontent.com/GcsSloop/ViewSupport/res/img/ViewSupport.png)

该开源库主要作用为简化自定义View流程，例如，自定义View继承 `CustomView` 可以自动获取View大小和一个默认画笔。

同时，它也提供了一些辅助工具，例如，可以绘制一个辅助坐标系的 `CanvasAidUtils`，拥有测量距离，角度弧度转换等功能的 `MathUtils`。

总而言之，这个开源库到作用就是为了优雅快速的制作自定义View，更多信息可以查看下面表格。

如果你对此有什么比较好的建议，欢迎提交 Issues 来告诉我。

*****

## 主要功能

封装一些与视图相关的工具类和辅助工具类，让自定义View更加优雅便捷。

例如绘制一个辅助的坐标系帮助检查视图位置：

<img src="http://ww4.sinaimg.cn/large/005Xtdi2jw1f4i5aypzo9j30dw0nhmxt.jpg" width=300 />

## 工具列表

>
**PS: 点击工具名称查看源码，点击Wiki查看简介。**

工具            | Wiki |简介
----------------|------|----------------------------
[CustomView](https://github.com/GcsSloop/ViewSupport/blob/master/Library/src/main/java/com/gcssloop/view/CustomView.java)                | [查看](https://github.com/GcsSloop/ViewSupport/wiki/CustomView)     | 自定义View基类，帮助你节省部分代码
[CanvasAidUtils](https://github.com/GcsSloop/ViewSupport/blob/master/Library/src/main/java/com/gcssloop/view/utils/CanvasAidUtils.java)  | [查看](https://github.com/GcsSloop/ViewSupport/wiki/CanvasAidUtils) | Canvas辅助工具，你可以用它绘制坐标系来帮助你检查视图的位置，并在完成之后移除该坐标系。
[CanvasUtils](https://github.com/GcsSloop/ViewSupport/blob/master/Library/src/main/java/com/gcssloop/view/utils/CanvasUtils.java)        | [查看](https://github.com/GcsSloop/ViewSupport/wiki/CanvasUtils)    | Canvas绘图工具，封装了一些Canvas没有提供的方法，目前只能用来画一条线。
[DensityUtils](https://github.com/GcsSloop/ViewSupport/blob/master/Library/src/main/java/com/gcssloop/view/utils/DensityUtils.java)      | [查看](https://github.com/GcsSloop/ViewSupport/wiki/DensityUtils)   | 密度工具， 根据设备进行如下单位转换: sp -> px, px -> sp, dp -> px, px -> dp
[MathUtils](https://github.com/GcsSloop/ViewSupport/blob/master/Library/src/main/java/com/gcssloop/view/utils/MathUtils.java)            | [查看](https://github.com/GcsSloop/ViewSupport/wiki/MathUtils)      | 数学工具， 封装一些数学算法，例如: 获取两点之间的距离，获取线段上某一点的位置， 获取线段与水平线夹角 等
[ViewUtils](https://github.com/GcsSloop/ViewSupport/blob/master/Library/src/main/java/com/gcssloop/view/utils/ViewUtils.java)            | [查看](https://github.com/GcsSloop/ViewSupport/wiki/ViewUtils)      | 视图工具， 封装了一些与视图相关等内容，如 手动测量视图大小， 为视图动态设置margin 等

## 文档

* [点击这里查看文档](https://jitpack.io/com/github/GcsSloop/ViewSupport/v1.2.2/javadoc/)
* [点击这里查看Wiki](https://github.com/GcsSloop/ViewSupport/wiki)

## 如何添加该开源库

#### Gradle:

**Step 1. 添加JitPack仓库**

在当前项目等根目录下的 `build.gradle` 文件中添加如下内容:

``` gradle
	allprojects {
		repositories {
			...
			maven { url "https://jitpack.io" }
		}
	}
```

**Step 2. 添加项目依赖**

``` gradle
	dependencies {
	        compile 'com.github.GcsSloop:ViewSupport:v1.2.2'
	}
```

## About Me

### 微博: [@GcsSloop](http://weibo.com/GcsSloop)

<a href="https://github.com/GcsSloop/README/blob/master/README.md" target="_blank"> <img src="http://ww4.sinaimg.cn/large/005Xtdi2gw1f1qn89ihu3j315o0dwwjc.jpg" width=300 height=100 /> </a>

## License

```
Copyright (c) 2016 GcsSloop

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
