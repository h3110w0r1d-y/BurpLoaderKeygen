# BurpLoaderKeygen <img src="https://img.shields.io/static/v1?label=JAVA&message=v8%2b&color=blue"> <img src="https://img.shields.io/static/v1?label=BurpSuitePro&message=1.7%2b&color=blue"> <img src="https://img.shields.io/static/v1?label=System&message=Windows | Linux | macOS&color=blue"> <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/h3110w0r1d-y/BurpLoaderKeygen?style=social">

[使用说明（中文）](./how-to-use-zh.md)

Burp Suite Pro Loader & Keygen (for Burp v1.7+)

## Integrated Projects
- https://github.com/x-Ai/BurpSuiteLoader
- BurpSuitePro Loader & Keygen by surferxyz
- https://github.com/googleweb/loader

### Description
The core patch and key generation logic are not written by me.  
Since version 1.9, the cracking method comes from @googleweb.  
This project simply integrates existing loaders and keygens and adds some convenience features.

## ⚠️ Disclaimer
This project is for learning and research purposes only.  
For commercial use, please purchase a legitimate license:
https://portswigger.net/burp

---

## Features
- Detect Burp updates (disable via `Ignore Update`)
- Auto start Burp (enable `Auto Run`)
- Support custom Java versions (place Java in the same directory)
- Support Java 8+
- Support BurpSuite v1.7+
- Support BurpBounty

---

## Usage

### Command Line
```bash
java -jar Burploaderkeygen.jar [-a|-auto [0|1]] [-i|-ignore [0|1]] [-n|-name <UserName>]
```

---

### macOS Instructions

1. Install Burp for macOS
2. Place the keygen in:
```
/Applications/Burp Suite Professional.app/Contents/Resources/app
```

3. Run:
```bash
cd "/Applications/Burp Suite Professional.app/Contents/Resources/app"
"/Applications/Burp Suite Professional.app/Contents/Resources/jre.bundle/Contents/Home/bin/java" -jar BurpLoaderKeygen.jar
```

4. Click **Run**, activate Burp, then close the keygen

5. Edit:
```
/Applications/Burp Suite Professional.app/Contents/vmoptions.txt
```

Add:
```
--add-opens=java.base/java.lang=ALL-UNNAMED
--add-opens=java.base/java.lang=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm.Opcodes=ALL-UNNAMED
-javaagent:BurpLoaderKeygen.jar
-noverify
```

If permission error occurs:
```bash
sudo xattr -r -d com.apple.quarantine /Applications/Burp\ Suite\ Professional.app
```

---

### Other Systems

Directory structure:
```
custom_dir/
├── jdk/ or jre/
│ ├── bin/
│ │ ├── java.exe or java
│ │ └── ...
│ └── ...
├── BurpLoaderKeygen.jar
└── burpsuite_pro_v20**.*.jar
```

or:
```
custom_dir/
├── bin/
│ ├── java.exe or java
│ └── ...
├── BurpLoaderKeygen.jar
└── burpsuite_pro_v20**.*.jar
```

Steps:

1. Double-click `BurpLoaderKeygen.jar` or run:
```bash
java -jar BurpLoaderKeygen.jar
```

2. Click **Run**, enter license, choose **manual activation**

3. After activation:
   - Enable `Auto Run` to start Burp silently
   - The keygen runs in background
   - Update detection runs automatically

Use `Ignore Update` to disable update checks
