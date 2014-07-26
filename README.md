
总结备忘与索引
==============
## 从源码构建testng

```
cd ~/gnuhub/git/
git clone git@github.com:gnuhub/testng.git
cd testng
mkdir -p ~/.ant/lib/
cp ivy-2.1.0.jar ~/.ant/lib
ant
```
* 生成的jar `target/testng-6.8.8.jar`
* 将jar包加入classpath
```
# 配置testng classpath
export CLASSPATH=$HOME/gnuhub/git/testng/target/testng-6.8.8.jar:$CLASSPATH
```
## testng helloworld

```
exercises/hello_testng
cd exercises/hello_testng
javac TestNGSimpleTest.java
java org.testng.TestNG testng.xml
```
* 结果
```
[TestNG] Running:
  /Users/stallman/gnuhub/git/testng/exercises/hello_testng/testng.xml


===============================================
Suite1
Total tests run: 1, Failures: 0, Skips: 0
===============================================
```

## 笔记书籍文档索引

* [testng](http://localhost:8080/wiki/index.php?title=testng)

