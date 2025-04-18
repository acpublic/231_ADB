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
### APKインストール
```
adb install <APKファイル>
```

### APKアンインストール
```
adb uninstall <パッケージ名>
```
### APK起動
```
adb shell am start -n [アプリ名]/[アクティビティ名]
```
### 画面キャプチャ
```
adb shell screencap -p /sdcard/screenshot.png
```
### 画面録画
```
adb shell screenrecord /sdcard/record.mp4
```
### 仮想的キー入力
- https://developer.android.com/reference/android/view/KeyEvent
```
adb shell input keyevent <キーコード>
```
### APKファイルの保存場所
```
adb shell pm list packages -f
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
