![(jacklogo)](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/JackTemplates.xctemplate/TemplateIcon.png "杰克logo")
## AddJackTemplates
* 定制化UIKit模板，UIView xib一键生成和使用，定制头文件标题样式。
## Contents
* Getting Started
	* [支持的类【Support what kinds of controls to AddJackTemplates】](#Support_what_kinds_of_controls_to_AddJackTemplates)<br>
	* [使用【How to use AddJackTemplates】](#How_to_use_AddJackTemplates)<br>
	* [谁在使用【More than hundreds of Apps are using AddJackTemplates】](#More_than_hundreds_of_Apps_are_using_AddJackTemplates)<br>
	* [目录【The Class Structure Chart of AddJackTemplates】](#The_Class_Structure_Chart_of_AddJackTemplates)<br>
* Comment API
	* [AddJackTemplates.sh](#AddJackTemplates_Jack)
	* [JackTemplates](#JackTemplates_Jack)
	* [jackAddstep](#jackAddstep_Jack)
* Examples
	* [Reference](#Reference)<br>
	* [选择定制模板](#jackstep3)<br>
	* [选择定制Xib View](#jackstep7)<br>
	* [定制控制器样式](#jackcontroller)<br>
* [Hope](#Hope)
## <a id="Support_what_kinds_of_controls_to_AddJackTemplates"></a>Support what kinds of controls to AddJackTemplates
* `NSObject-Objective-C`、`NSObject-Swift`、`UIViewController-Objective-C`、`UIViewController-Swift`、`UIViewControllerXIB-Objective-C`、`UIViewControllerXIB-Swift`、`UIView-Objective-C`、`UIView-Swift`、`UIViewXIB-Objective-C`、`UICollectionReusableView-Objective-C`、`UICollectionReusableView-Swift`、`UICollectionReusableViewXIB-Objective-C`、`UICollectionReusableViewXIB-Swift`、`UICollectionViewCell-Objective-C`、`UICollectionViewCell-Swift`、`UICollectionViewCellXIB-Objective-C`、`UICollectionViewCellXIB-Swift`、`UICollectionViewController-Objective-C`、`UICollectionViewController-Swift`、`UICollectionViewControllerXIB-Objective-C`、`UICollectionViewControllerXIB-Swift`、`UITableViewCell-Objective-C`、`UITableViewCell-Swift`、`UITableViewCellXIB-Objective-C`、`UITableViewCellXIB-Swift`、`UITableViewController-Objective-C`、`UITableViewController-Swift`、`UITableViewControllerXIB-Objective-C`、`UITableViewControllerXIB-Swift`、`UIScrollView`、`UITableView`、`UICollectionView`
## <a id="How_to_use_AddJackTemplates"></a>How_to_use_AddJackTemplates

* 第一步确定你安装Xcode之后在应用程序中的绝对路径是什么?（可以用终端进入Xcode 中然后pwd下就有Xcode的绝对路径了）
如果你的电脑上安装了两个xcode ，要找到xcode的安装绝对路径 ，确保你找的xcode的绝对路径是对的
比如:xcode的绝对路径是/Applications/Xcode.app ，接下来打开AddJackTemplates.sh文件，把下面图中红色框内的路径改为/Applications/Xcode.app，如果和红色框内的路径一样那么就不用修改了。

![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack1.png "杰克定制模板")

![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack2.png "杰克定制模板") 

* 第二步打开终端，用指令cd 进入目录 AddJackTemplates-master（要找到你存放AddMissingTemplates-master的路径），然后运行里面的脚本AddJackTemplates.sh就ok了。怎么运行脚本呢和运行二进制程序是一样的, 命令行是这样的:. +空格+名称(AddJackTemplates.sh)。
![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack12.png "杰克定制模板") 

## <a id="More_than_hundreds_of_Apps_are_using_AddJackTemplates"></a>More than hundreds of Apps are using AddJackTemplates
<img src=https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack14.jpeg width="320" height="568">
	* More information of App can focus on:[神龙无敌大将](https://github.com/JackCoderForLove)

## <a id="The_Class_Structure_Chart_of_AddJackTemplates"></a>The Class Structure Chart of AddJackTemplates
![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack13.png "杰克定制模板")

## <a id="AddJackTemplates_Jack"></a>AddJackTemplates.sh
```sh
# !/bin/sh

SAVEIFS=$IFS
IFS=$(echo -en "\n\b")

FILE_TEMPLATES_PATH="/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/Library/Xcode/Templates/File Templates/Source"

JACK_APPLICATION_PATH="$PWD/JackTemplates.xctemplate"

cp -R $JACK_APPLICATION_PATH $FILE_TEMPLATES_PATH

IFS=$SAVEIFS

```
## <a id="#JackTemplates_Jack"></a>JackTemplates模板
* 存放定制模板的文件夹
## <a id="#jackAddstep_Jack"></a>xcode添加定制文件模板步骤
* 使用说明文档rtf格式
## <a id="#Reference"></a>Reference
* 近期更新
![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack4.png "杰克定制模板")

## <a id="#jackstep3"></a>选择定制模板
![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack3.png "杰克定制模板")

## <a id="#jackstep7"></a>选择定制Xib View
* xcode6之后创建UIView是不能勾选xib的，创建View如果想用xib，有两种方式
![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack7.png "杰克定制模板")
	* 创建空的，没有任何关联的xib模板，在控制器里边去加载
	* 创建xib模板，创建UIView组件，使xib文件和UIView组件关联起来，这时候相关的UI实现和逻辑，可以在UIView类里边去实现
* AddJackTemplates定制UIView
	* 选择定制模板，UIView为父类，并勾选创建xib
![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack8.png "杰克定制模板")
        * UIView的xib和.h和.m自动关联，并生成相应的模块代码
![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack11.png "杰克定制模板")
![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack9.png "杰克定制模板")
	* 如何使用创建的View
```objc
    JCTestView *testView = [JCTestView instanceJackNibView];
    testView.frame =  CGRectMake(0, 0, [UIScreen mainScreen].bounds.size.width, [UIScreen mainScreen].bounds.size.height);
    [self.view addSubview:testView];
```
![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack10.png "杰克定制模板")
  
## <a id="#jackcontroller"></a>定制控制器样式
* 往往我们创建控制器之后，里边的方法原本是按着顺序写的，可是方法多了之后，就写乱了，这时候需要写mark来区分，每个控制器都需要自己添加，定制化控制器自动生成常用的mark和常用的代码块，这样方便很多。
	* 选择定制化模板
  ![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack3.png "杰克定制模板")
  
	* 选择定制化控制器
  ![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack4.png "杰克定制模板")
  
 	* 定制化控制器样式
  ![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack5.png "杰克定制模板")
  ![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack6.png "杰克定制模板")
 

## <a id="Hope"></a>Hope
* If you find bug when used，Hope you can Issues me，Thank you or try to download the latest code of this framework to see the BUG has been fixed or not）
* If you find the function is not enough when used，Hope you can Issues me，I very much to add more useful function to this framework ，Thank you !
* If you want to contribute code for AddJackTemplates，please Pull Requests me
* If you use AddJackTemplates in your develop app，Hope you can send a email to me for your app，my email is 979900351@qq.com。
I Will install your app，and according to the usage of many app，to be a better design and improve to AddJackTemplates，Thank you !




