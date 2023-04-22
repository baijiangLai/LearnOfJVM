ClassLoader是一个抽象类，所有的类加载器都继承自ClassLoader(不包含启动类加载器)

![classLoader方法.png](..%2Fimages%2F01-%E7%B1%BB%E5%8A%A0%E8%BD%BD%E5%AD%90%E7%B3%BB%E7%BB%9F%2FclassLoader%E6%96%B9%E6%B3%95.png)


## 获取ClassLoader的途径
1. 获取当前类的CLassLoader
```java
clazz.getCLassLoader()
```
2. 获取当前线程上下文的ClassLoader
```java
Thread.currentThread.getContextClassLoader()
```
3. 获取系统的ClassLoader
```java
ClassLoader.getSystemClassLoader()
```
4. 获取调用者的ClassLoader
```java
DriverManager.getCallerClassLoader()
```