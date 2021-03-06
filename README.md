# react-native-ios-style-picker
[![npm version](http://img.shields.io/npm/v/react-native-ios-style-picker.svg?style=flat-square)](https://npmjs.org/package/react-native-ios-style-picker "View this project on npm")
[![npm version](http://img.shields.io/npm/dm/react-native-ios-style-picker.svg?style=flat-square)](https://npmjs.org/package/react-native-ios-style-picker "View this project on npm")

## Introduction
Cross platform Picker component based on React-native.

Since picker is originally supported by ios while Android only supports a ugly Spinner component. If you want to have the same user behaviour, you can use this.

The android component is based on https://github.com/AigeStudio/WheelPicker which runs super fast and smoothly. It also supports curved effect which make it exactly the same looking and feel as the ios picker.
![](https://raw.githubusercontent.com/lesliesam/react-native-ios-style-picker/master/demo.gif)
![](https://raw.githubusercontent.com/lesliesam/react-native-ios-style-picker/master/demo_android.gif)

## How to use

Run command

For apps using RN 0.32 or higher, please run
```
npm i react-native-ios-style-picker --save
```
For apps using RN 0.31 or less, please run
```
npm install --save --save-exact react-native-ios-style-picker
```
Add in settings.gradle
```
include ':react-native-ios-style-picker'
project(':react-native-ios-style-picker').projectDir = new File(settingsDir, '../node_modules/react-native-ios-style-picker/android')
```
Add in app/build.gradle
```
compile project(':react-native-ios-style-picker')
```
Modify MainActivity
```
    import com.zyu.ReactNativeWheelPickerPackage;
    ......

    protected List<ReactPackage> getPackages() {
        return Arrays.<ReactPackage>asList(
            new MainReactPackage(), new ReactNativeWheelPickerPackage()
        );
    }
```
