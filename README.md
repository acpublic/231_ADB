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
