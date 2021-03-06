ColorView
========

抛弃Selector文件，直接在布局文件中实现，文字颜色，背景颜色，边框圆角，背景图片，前景图片的配置。

![](https://github.com/uccmawei/ColorView/raw/master/demo.jpg)


**1. Gradle 添加引用**

    compile 'com.wei.android.lib:colorview:1.2.0'

**2. 拓展的View**

    ColorButton
    ColorEditText
    ColorImageView
    ColorLinearLayout
    ColorRelativeLayout
    ColorTextView
    ColorView

**3. 拓展的属性**

    app:textColorNormal="#FFFFFF"
    app:textColorPressed="#FFFFFF"
    app:textColorSelected="#FFFFFF"
    app:textColorChecked="#FFFFFF"
    app:textColorUnable="#FFFFFF"

    app:backgroiundColorNormal="#FFFFFF"
    app:backgroiundColorPressed="#FFFFFF"
    app:backgroiundColorSelected="#FFFFFF"
    app:backgroiundColorChecked="#FFFFFF"
    app:backgroiundColorUnable="#FFFFFF"

    app:backgroundDrawableNormal="@drawable/pic_test"
    app:backgroundDrawablePressed="@drawable/pic_test"
    app:backgroundDrawableSelected="@drawable/pic_test"
    app:backgroundDrawableChecked="@drawable/pic_test"
    app:backgroundDrawableUnable="@drawable/pic_test"

    app:srcDrawableNormal="@drawable/pic_test"
    app:srcDrawablePressed="@drawable/pic_test"
    app:srcDrawableSelected="@drawable/pic_test"
    app:srcDrawableChecked="@drawable/pic_test"
    app:srcDrawableUnable="@drawable/pic_test"

    app:borderColorNormal="#FFFFFF"
    app:borderColorPressed="#FFFFFF"
    app:borderColorSelected="#FFFFFF"
    app:borderColorChecked="#FFFFFF"
    app:borderColorUnable="#FFFFFF"

    app:borderWidth="2dp"
    app:borderDashWidth="10dp"
    app:borderDashGap="10dp"

    app:cornerRadius="10dp"
    app:cornerRadiusTopLeft="10dp"
    app:cornerRadiusTopRight="10dp"
    app:cornerRadiusBottomRight="10dp"
    app:cornerRadiusBottomLeft="10dp"

**3. 属性介绍**

    1. xxxNormal属性具有通用性，设置了Normal后其他4个属性的值都默认都是跟随Normal
    
    2. 背景图片的和背景颜色一起设定时，背景图片会覆盖背景颜色。

    3. 需要更新某个属性则调用：view.getXXHelper().setXXX();

**4. 开发笔记**

[1. 加粗边框时需要重新构建背景对象，否则背景边框绘制不正确。](https://issuetracker.google.com/issues/70444558 "Google Issue")

**5. 本库小瑕疵**

[1. 当四个圆角的值不一样时，背景绘制的效果有些不准确，圆角值越大越明显，Selector也有一样的问题。](https://issuetracker.google.com/issues/70461762 "Google Issue")

**6. 版本记录**

**v1.2.0**　`2017.12.12`　发布1.2.0版本

## License ##

Licensed under the MIT License, see the [LICENSE](https://github.com/uccmawei/ColorView/blob/master/LICENSE) for copying permission.
