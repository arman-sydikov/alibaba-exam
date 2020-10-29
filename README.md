## 阿里巴巴在线考试
-------------------

#### 下面关于缺省构造方法的描述中正确的是？
- [ ] `当类中没有定义任何构造方法时，Java 编译器将为这个类创建缺省构造方法`
- [ ] `缺省构造方法可以初始化其他方法中定义的变量`
- [ ] `Java编译器会为所有的类创建缺省构造方法`
- [ ] `如果在一个类中定义的构造方法都声明了参数，Java 编译器将为这个类创建一个缺省构造方法`

#### 当要将一文本文件当作一个数据库访问，读完一个纪录后，跳到另一个纪录，它们在文件的不同地方时，一般使用___类访问：
- [ ] `FileOutputStream`
- [ ] `RandomAccessFile`
- [ ] `PipedOutputStream`
- [ ] `BufferedOutputStream`

#### What is the output of the following?
```java
Stream<String> s = Stream.of("speak", "bark", "meow", "growl");
BinaryOperator<String> merge = (a, b) -> a;
Map<Integer, String> map = s.collect(toMap(String::length, k -> k, merge));
System.out.println(map.size() + " " + map.get(4));
```
- [ ] `2 bark`
- [ ] `2 meow`
- [ ] `4 bark`
- [ ] `None of the above`