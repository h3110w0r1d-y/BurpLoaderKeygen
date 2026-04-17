# BurpLoaderKeygen <img src="https://img.shields.io/static/v1?label=JAVA&message=v8%2b&color=blue"> <img src="https://img.shields.io/static/v1?label=BurpSuitePro&message=1.7%2b&color=blue"> <img src="https://img.shields.io/static/v1?label=System&message=Windows%20|%20Linux%20|%20macOS&color=blue"> <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/h3110w0r1d-y/BurpLoaderKeygen?style=social">

[How to Use (English)](./how-to-use.md)

Burp Suite Pro 加载器 & 注册机（适用于 Burp v1.7+）

## 本项目整合自以下项目
- https://github.com/x-Ai/BurpSuiteLoader
- BurpSuitePro Loader & Keygen By surferxyz
- https://github.com/googleweb/loader

### 说明
核心的 patch 代码和算号逻辑并非本人编写，本项目 1.9 版本之后的破解方案来自 @googleweb，本项目只是对各位作者的 Loader 和 Keygen 进行了整合，并增加了一些便捷功能。

## ⚠️ 声明
本项目仅供学习与交流使用，商业用途请购买正版软件：
https://portswigger.net/burp

---

## 特性
- 检测 Burp 更新（可勾选 `Ignore Update` 关闭）
- 自动启动 Burp（勾选 `Auto Run`）
- 支持指定 Java 版本（将 Java 放到同目录即可自动调用）
- 支持 Java 8+
- 支持 BurpSuite v1.7+
- 支持 BurpBounty

---

## 使用方法

### 命令行
```bash
java -jar Burploaderkeygen.jar [-a|-auto [0|1]] [-i|-ignore [0|1]] [-n|-name <UserName>]
```

---

### Mac 使用方法

1. 安装 Mac 版 Burp
2. 将注册机放到：
```
/Applications/Burp Suite Professional.app/Contents/Resources/app
```

3. 执行：
```bash
cd "/Applications/Burp Suite Professional.app/Contents/Resources/app"
"/Applications/Burp Suite Professional.app/Contents/Resources/jre.bundle/Contents/Home/bin/java" -jar BurpLoaderKeygen.jar
```

4. 点击 Run 启动 Burp，激活后关闭注册机

5. 修改：
```
/Applications/Burp Suite Professional.app/Contents/vmoptions.txt
```

添加：
```
--add-opens=java.base/java.lang=ALL-UNNAMED
--add-opens=java.base/java.lang=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm.Opcodes=ALL-UNNAMED
-javaagent:BurpLoaderKeygen.jar
-noverify
```

如果出现权限错误：
```bash
sudo xattr -r -d com.apple.quarantine /Applications/Burp\ Suite\ Professional.app
```

---

### 其他系统使用方法

目录结构：
```
custom_dir/
├── jdk/ 或 jre/
│ ├── bin/
│ │ ├── java.exe 或 java
│ │ └── ...
├── BurpLoaderKeygen.jar
└── burpsuite_pro_v20**.*.jar
```

或：
```
custom_dir/
├── bin/
│ ├── java.exe 或 java
│ └── ...
├── BurpLoaderKeygen.jar
└── burpsuite_pro_v20**.*.jar
```

步骤：

1. 双击 `BurpLoaderKeygen.jar` 或执行：
```bash
java -jar BurpLoaderKeygen.jar
```

2. 点击 `Run`，输入许可证，选择手动激活

3. 激活后勾选 `Auto Run`：
   - 启动时不会显示注册机界面
   - 后台自动检测更新
   - 若检测到更新会弹出界面

可勾选 `Ignore Update` 禁止检测更新
