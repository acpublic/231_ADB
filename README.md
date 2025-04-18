# Android Debug Bridge（ADB）
## コマンド
### バージョン
```
adb 
Android Debug Bridge version 1.0.41
```
### 内部アクセス
```
adb shell
```
### 接続デバイス
```
adb devices
```
### ファイル外部転送
```
adb pull /sdcard/Download/temp.png .
```
### ファイル内部転送
```
adb push temp.png /sdcard/Download/
```
### ADBサーバ再起動
```
adb kill-server
adb start-server
```
### 端末再起動
```
adb reboot
```

## perfetto
### UI
https://ui.perfetto.dev/

### Systrace
```java
Trace.beginSection("TextViewSampleActivity")
...
Trace.endSection()
```

### 解像度変更
```
adb shell wm size
adb shell wm size 1920x1080
```
### DPI値変更
```
$ adb shell wm density
$ adb shell wm density 320
```
