# BurpLoaderKeygen <img src="https://img.shields.io/static/v1?label=JAVA&message=v8%2b&color=blue"> <img src="https://img.shields.io/static/v1?label=BurpSuitePro&message=1.7%2b&color=blue"> <img src="https://img.shields.io/static/v1?label=System&message=Windows | Linux | macOS&color=blue"> <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/h3110w0r1d-y/BurpLoaderKeygen?style=social">
Burp Suite Pro Loader &amp; Keygen ( burp v1.7+ )

## 本项目由以下项目整合而成 / This project is integrated by the following projects
- https://github.com/x-Ai/BurpSuiteLoader
- BurpSuitePro Loader&Keygen By surferxyz
- https://github.com/googleweb/loader

### 核心的patch代码和算号代码并不是我写的，本项目1.9版本后的破解方案来自这位大佬 @googleweb ，我只是把各位大佬的Loader和Keygen整合到一块加了点小功能方便使用

## **项目仅供学习和交流使用，商业使用请购买正版软件！链接:https://portswigger.net/burp**
## **This project is only for learning and communication. For commercial use, please buy genuine software! Link:https://portswigger.net/burp**

### 特性 / Features
- 检测Burp更新，如果不需要检测请勾选`Ignore Update`
- 不用编写脚本，自动启动burp，只需要勾选`Auto Run`
- 支持指定Java版本，只需要把指定版本的Java放到同目录下，注册机会自动调用
- 支持Java8+
- 支持BurpSuite v1.7+
- 支持BurpBounty

- Detect burp updates. If you don't need, please check `Ignore Update` 
- Auto start burp without write command manually, just check `Auto Run`
- Support for specifying java versions, just put java files in same path
- Support Java 8+
- Support BurpSuite v1.7+
- Support BurpBounty

### **Jar包未混淆，欢迎dalao们改进！**
## 食用方法
### 命令行
```
java -jar Burploaderkeygen.jar [-a|-auto [0|1]] [-i|-ignore [0|1]] [-n|-name <UserName>]
```
### Mac版食用方法
0. 安装Mac版Burp
1. 将注册机放置到`/Applications/Burp Suite Professional.app/Contents/Resources/app`目录下
2. 执行以下命令启动注册机
```
cd "/Applications/Burp Suite Professional.app/Contents/Resources/app"
"/Applications/Burp Suite Professional.app/Contents/Resources/jre.bundle/Contents/Home/bin/java" -jar BurpLoaderKeygen.jar
```
点击run启动Burp, 激活后关闭注册机

3. 修改`/Applications/Burp Suite Professional.app/Contents/vmoptions.txt`, 增加以下参数
```
--add-opens=java.base/java.lang=ALL-UNNAMED
--add-opens=java.base/java.lang=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm.Opcodes=ALL-UNNAMED
-javaagent:BurpLoaderKeygen.jar
-noverify
```
之后便可以正常启动了

如果出现以下错误
<img width="367" alt="image" src="https://user-images.githubusercontent.com/52311174/197393162-cdd3be46-6e33-42e2-8c62-773a991ba59d.png">
```
sudo xattr -r -d com.apple.quarantine /Applications/Burp\ Suite\ Professional.app
```

### 其他系统食用方法

0. 将BurpLoaderKeygen.jar、burpsuite_pro_v20**.*.jar 放到同一目录下(也可将指定版本的Java放到目录中，注册机会自动调用)
![image](https://user-images.githubusercontent.com/52311174/136488232-bae027a6-8f9a-45eb-9d6c-e0b150084170.png)

1. 直接双击 BurpLoaderKeygen.jar 或者 `java -jar BurpLoaderKeygen.jar`

2. 点击`Run`，输入许可证然后选择**手动激活**即可

3. 激活后勾选`Auto Run`，打开BurpLoaderKeygen.jar即可自动启动BurpSuite，不显示注册机窗口，但会在后台自动检测Burp更新，当检测到更新时将显示注册机，你可以勾选`Ignore Update` 来禁止检测更新，启动Burp后注册机直接退出。
