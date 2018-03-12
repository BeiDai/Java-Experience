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

### 三、类和对象

1. 类的组成

 - 类名
 - 成员变量
 - 成员方法
 - 构造方法

         //类名
         [修饰符] class 类名
         {
           成员变量...
           成员方法...
           构造方法...
         }
         [修饰符] public,final,abstract,或省略

         //成员变量
         [修饰符] 类型 成员变量名 [ = 默认值]
         [修饰符] (public,protected,private)+(static,final)
         其中public,protected,private同时只能有一个

         //成员方法
         [修饰符]  方法返回值类型 方法名(形参列表)
         {
           方法体
         }
         [修饰符] (public,protected,private)+(static,(final+abstract))
         其中public,protected,private同时只能有一个
         final,abstract同时只能有一个
         final：方法不可以重写

         //构造方法
         [修饰符] 构造方法名(形参列表)
         {
           方法体
         }

         例子：
         //类名
         class MyClass
         {
           Private int mValue;  //成员变量

           public int getValue() //成员方法
           {
             return mValue;
           }

           public void setValue(int value) //成员方法
           {
             mValue = value;
           }

           public MyClass(int value) //构造方法
           {
             mValue = value;
           }
         }

### 三、创建和使用对象

    class Product
    {
      public String name；
      public Product(String name)
      {
        this.name = name;
      }
      public void print()
      {
        Systen.out.println(name);
      }
    }

    public class CreateAndUseObject
    {
      public static void main(String[] args)
      {
        Prduct product;
        product = new Product("iPhone 8");
        product.print();

        Prouct product1 = new Product("iPhone 9");
        product.name = "特斯拉"
        product1.print();

      }
    }
