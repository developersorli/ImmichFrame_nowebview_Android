# About

This is a clone of https://github.com/immichFrame/ImmichFrame\_Android

This code does not use a webview component.
This workaround is useful if your tablet has a broken webview component or classes.dex.



\## Install App

adb install ImmichFrame.apk



\## Uninstall APP

adb uninstall com.immichframe.immichframe



\## Start App

adb.exe shell am start com.immichframe.immichframe/.MainActivity



\## Run settings

adb shell am start -a android.settings.SETTINGS





\## Disable Frameo app:

adb shell su

pm disable net.frameo.frame

exit



\## Enable Frameo app:

adb shell am start net.frameo.frame



If you did not brick webview on your frameo. Read this carfuly: 



\# ⚠️ Why You Should Avoid `mount -o rw,remount /system \&\& rm-rf /system/app/webview/oat` on Android



This command may seem like a quick fix, but it introduces serious risks to system stability and WebView functionality.





🚫 Why This Is Dangerous

1\. WebView May Break Completely

\- The oat/ directory contains optimized .odex files used by Android's runtime.

\- Removing these files without proper regeneration can cause WebView to crash or fail to load.

\- Affected components include:

\- Browsers

\- Apps using embedded HTML

\- System services relying on WebView

2\. No Safety Net

\- rm -rf deletes everything instantly, with no checks.

\- If the APK or DEX files are invalid or missing, the system cannot regenerate the oat files.

\- This can lead to boot-time errors or runtime crashes.

3\. System Partition Risks

\- On many devices (especially Android 6.0.1), /system is read-only unless rooted.

\- Even with root, remounting and modifying /system can break SELinux contexts.

\- This may result in:

\- Boot loops

\- Inaccessible system apps

\- Failed OTA updates



If you break it. The solution is to buy a new Frameo board or send it to the factory to be repaired.

Or you can use this apk which does not use webview component.







