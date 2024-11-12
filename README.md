## コマンド
### バージョン
$ adb  
Android Debug Bridge version 1.0.41

### ファイル転送
$ adb push temp.png /sdcard/Download/

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
$ adb shell wm size
$ adb shell wm size 1920x1080

### DPI値変更
$ adb shell wm density
$ adb shell wm density 320

