# About

This is a clone of https://github.com/immichFrame/ImmichFrame\_Android

This code does not use a webview component.
This workaround is useful if your tablet has a broken webview component or classes.dex.



## Install App
```
adb install ImmichFrame.apk
```


## Uninstall APP
```
adb uninstall com.immichframe.immichframe
```


## Start App
```
adb.exe shell am start com.immichframe.immichframe/.MainActivity
```


## Run settings
```
adb shell am start -a android.settings.SETTINGS
```




## Disable Frameo app:
```
adb shell su

pm disable net.frameo.frame

exit
```


## Enable Frameo app:
```
adb shell am start net.frameo.frame
```


If you did broke WebView.apk or you lost backup of original apk on your Frameo device. Read this: 

If you break it, the solution is to buy a new Frameo board or send it to the factory for firmware repair.

Or you can install this apk from this Android project which does not use webview component and just works :)







