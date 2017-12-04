![(jacklogo)](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/JackTemplates.xctemplate/TemplateIcon.png "杰克logo")
## AddJackTemplates
* 定制化UIKit模板，UIView xib一键生成和使用，定制头文件标题样式。
## Contents
* Getting Started<br>
    * [支持的类【Support what kinds of controls to AddJackTemplates】](#Support_what_kinds_of_controls_to_AddJackTemplates)<br>
    * [使用【How to use AddJackTemplates】](#How_to_use_AddJackTemplates)<br>
    * [谁在使用【More than hundreds of Apps are using AddJackTemplates】](#More_than_hundreds_of_Apps_are_using_AddJackTemplates)<br>
    * [目录【The Class Structure Chart of AddJackTemplates】](#The_Class_Structure_Chart_of_AddJackTemplates)<br>
* Comment API
	* [AddJackTemplates.sh](#AddJackTemplates.sh)<br>
	* [JackTemplates.xctemplate](#JackTemplates.xctemplate)<br>
	* [xcode添加定制文件模板步骤](#jackaddsetp)<br>
* Examples
    * [Reference](#Reference)<br>
    * [选择定制模板](#jackstep3)<br>
    * [选择定制Xib View](#jackstep7)<br>
    * [定制控制器样式](#jackstepController)<br>
    * [定制View样式](#jackstepView)<br>
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
![jack](https://github.com/JackCoderForLove/AddJackTemplates/blob/master/img/jack14.jpeg width:320 height:568 "杰克定制模板")
* More information of App can focus on:[神龙无敌大将](https://github.com/JackCoderForLove)

Add OC Customization templates to Xcode ，pls modify PROJECT_TEMPLATES_PATH and FILE_TEMPLATES_PATH as your need.

```sh
# !/bin/sh

SAVEIFS=$IFS
IFS=$(echo -en "\n\b")

FILE_TEMPLATES_PATH="/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/Library/Xcode/Templates/File Templates/Source"

JACK_APPLICATION_PATH="$PWD/JackTemplates.xctemplate"

cp -R $JACK_APPLICATION_PATH $FILE_TEMPLATES_PATH

IFS=$SAVEIFS

```
