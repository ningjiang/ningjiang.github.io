---
layout: post
title: "Enabling OpenCV4Android"
date: 2014-08-19 09:58:11 +0800
comments: true
categories: 
---

Basically following the instructions [How to start](http://opencv.org/platforms/android.html)

It clearly describes the steps in details:

- [“Introduction into Android Development”](http://docs.opencv.org/doc/tutorials/introduction/android_binary_package/android_dev_intro.html)
- [“OpenCV for Android SDK”](http://docs.opencv.org/doc/tutorials/introduction/android_binary_package/O4A_SDK.html)
- [“Android development with OpenCV”](http://docs.opencv.org/doc/tutorials/introduction/android_binary_package/dev_with_OCV_on_Android.html)

Several notes:

- Convert your project to a C/C++ project if you want to compile native code. See the section *Building application native part from Eclipse (CDT Builder)*
- Import the *OpenCV Library* and then reference the library in your project
- Configure NDKROOT and use it in *C/C++ Build Command* for build and *Paths and Symbols* for includes
- Configure OPENCVROOT and use it in *Paths and Symbols* for includes
- Change jni/Android.mk and jni/Application.mk to suit your needs