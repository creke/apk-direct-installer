# apk-direct-installer

直接安装APK，完全不依赖系统安装器。在中国大陆的安卓系统尤其有用，因为各种魔改系统（MIUI、鸿蒙、ColorOS等）对于APK安装都很复杂，还有可能要求账号登录等，对开发者很麻烦。本项目专为此而生。

Direct install android APK WITHOUT system installer UI, especially useful when CN modified android apk installer is too complicated to use.

# Roadmap

- [x] 手把手教程（复杂）
- [ ] English Tutorial (Professional)
- [ ] APK直装应用（简单）

# 中文教程

## 安装Shizuku

Shizuku安装地址（选1个能下载的就行）：

* https://www.coolapk.com/apk/moe.shizuku.privileged.api （酷安）
* https://github.com/RikkaApps/Shizuku/releases （github）

## 配置Shizuku

然后前往 https://shizuku.rikka.app/zh-hans/guide/setup/ 把Shizuku配置起来，这步很重要！

## 安装sShell

前往 https://f-droid.org/zh_Hans/packages/in.sunilpaulmathew.ashell/ 下载并安装aShell

## 如何下载&直接安装APK

下载你的apk，建议下载到“下载”目录下，记住文件名，如 abc.apk

启动aShell（如果Shizuku要授权，则允许授权）

在aShell中粘贴命令（如果是其它路径或其它文件名，则视情况修改）：

```bash
export APK_PATH=/sdcard/Download/abc.apk && APK_SIZE=$(stat --printf="%s" ${APK_PATH}) && cat ${APK_PATH} | pm install -S ${APK_SIZE}
```

回车执行，如果最后展示

```bash
Success
```

恭喜，直接安装成功！

Via [https://creke.net/842.html](https://creke.net/842.html)


# English Tutorial

TBD
