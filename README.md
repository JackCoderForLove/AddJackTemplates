第一步确定你安装Xcode之后在应用程序中的绝对路径是什么?（可以用终端进入Xcode 中然后pwd下就有Xcode的绝对路径了）

如果你的电脑上安装了两个xcode ，要找到xcode的安装绝对路径 ，确保你找的xcode的绝对路径是对的


比如:xcode的绝对路径是/Applications/Xcode.app ，接下来打开AddJackTemplates.sh文件，把下面图中红色框内的路径改为/Applications/Xcode.app，如果和红色框内的路径一样那么就不用修改了。
![jack](https://github.com/JackCoderForLove/AddJackTemplates/img/jack1.png "杰克定制模板") 

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
