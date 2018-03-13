# Java-Experience
java学习笔记

### 一、开发环境

1. 开发 Java 都需要 做 些什么
（1） JDK  (java的开发包，编译器 运行器 库 等)
（2） 配置 Java 开发环境 (任何目录都可以访问)
（3） Eclipse (开发大型程序)

2. 下载 JDK
下载地址
http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

3. 配置 Java  开发环境
认识一下 JDK 的文件夹
将 bin 目录设置到 PATH 环境变量中(属性 高级设置 系统环境)

4. 测试java环境

        public class Helloworld{
        		public static void main(String[] args)
        		{
        				System.out.println("Hello java");
        		}
        }

        javac Helloworld.java

        java  Heloworld



虚拟机：virtualbox
下载地址：https://www.virtualbox.org/wiki/Downloads

Java SDK
下载地址：http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

Android Studio下载: https://developer.android.com/studio/index.html
下面是Android SDK下载，选择自己的操作系统平台即可（可能需要翻墙）

###  二、包 package

- 多个java类协同工作

- 编写一个Java类放入package内

- 避免库和类名重合冲突

- 相当于windows系统里的目录

- 命名规则xxxx.xxxx.xxxx

- javac -d . Product.java 生成包目录结构
