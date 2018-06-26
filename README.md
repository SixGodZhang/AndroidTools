# AndroidTools
(测试软件:麦库记事)
##编译步骤:
1.将APK用APK Tool反编译成得到文件夹
 apktool d webmknote_default_4.2.0.apk

2.将smali文件编译成dex文件

    java -jar smali.jar assemble com\ -o test.dex

3.将dex文件编译成jar包,借助ApkToolkit工具

4.用jd-gui查看jar包,即可看见java源码

## 工具包:
**APKToolKit: **dex文件=======>jar包

**apkool.bat/apktool_2.3.2.jar:**========>编译与反编译APK

**jd-gui:**查看Jar包中Java源代码

**smali.jar:**将smali文件编译成dex文件

参考资料:


- https://blog.csdn.net/u013233097/article/details/51256992 smali文件编译步骤
- https://github.com/JesusFreke/smali/tree/master/baksmali baksmali 开源项目地址,可以获取jar包,中第二步骤命令
- https://blog.csdn.net/llzkkk12/article/details/78526377 Android 反编译的一些工具