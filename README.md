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
