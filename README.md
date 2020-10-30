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

#### Which variable declaration is the first line not to compile?
```java
class Building {}
class House extends Building {}
public void convert() {
    Building b = new Building();
    House h = new House();
    Building bh = new House();
    Building p = (House) b;
    House q = (Building) h;
    Building r = (Building) bh;
    House s = (House) bh;
}
```
- [ ] `p`
- [ ] `q`
- [ ] `r`
- [ ] `s`

#### 关于 B+ 树表述正确的有？
- [ ] `只有叶子节点才能存储数据`
- [ ] `非叶子节点可以存储数据和索引`
- [ ] `叶子节点有双向链表关联`
- [ ] `非叶子节点的最大容量是固定的`

#### 下来哪些数据会出现在函数调用栈中？
- [ ] `函数入口地址`
- [ ] `函数出口地址`
- [ ] `局部变量`
- [ ] `当前执行的指令地址`

#### GC root 具体指以下哪些对象？
- [ ] `类成员变量`
- [ ] `函数内局部变量`
- [ ] `静态变量`
- [ ] `常量`

#### 以下哪些技术可以达到原子性操作？
- [ ] `volatile`
- [ ] `CAS`
- [ ] `lock`
- [ ] `synchronized`

#### 下列哪些引用类型是 java 中定义的？
- [ ] `强引用`
- [ ] `弱引用`
- [ ] `轻引用`
- [ ] `虚引用`

#### redis 支持以下哪些数据类型？
- [ ] `list`
- [ ] `hash`
- [ ] `map`
- [ ] `set`

#### 链表具有的特点是（）
- [ ] `不事先估计存储空间`
- [ ] `可随机访问任一元素`
- [ ] `插入删除不需要移动元素`
- [ ] `所需空间与线性表长度成正比`

#### 下面能让线程停止执行的有（）
- [ ] `sleep()`
- [ ] `stop()`
- [ ] `notify()`
- [ ] `synchronized()`
- [ ] `yield()`
- [ ] `wait()`

#### 关于以下程序的说明，正确的是（）
```java
public class Test {
    static int x = 10;
    static {
        x += 5;
    }
    public static void main(String[] args) {
        System.out.println("x=" + x);
    }
    static {
        x += 3;
    }
}
```
- [ ] `不能通过编译，因为缺少方法名和返回类型`
- [ ] `不能编译通过，因为只能有一个静态初始化块`
- [ ] `编译通过，执行结果为：x=18`
- [ ] `编译通过，执行结果为：x=15`

#### What is the output of the following?
```java
package reader;
import java.util.stream.*;

public class Books {
    public static void main(String[] args) {
        IntegerStream pages = IntegerStream.of(200, 300);
        IntegerSummaryStatistics stats = pages.summaryStatistics();
        long total = stats.getSum();
        long count = stats.getCount();
        System.out.println(total + "-" + count);
    }
}
```
- [ ] `500-0`
- [ ] `500-2`
- [ ] `The code does not compile`
- [ ] `The code compiles but throws an exception at runtime`

#### What does the following `paint()` method draw?
```java
public void paint(Graphics g) {
    g.drawString("Any question", 10, 0);
}
```
- [ ] `The string "Any question?", with its top-left corner at 10,0`
- [ ] `A little squiggle coming down from the top of the component`

#### 执行下面代码，下面描述正确的是：
```java
public class Person {
    static int arr[] = new int[10];
    public static void main(String a[]) {
        System.out.println(arr[1]);
    }
}
```
- [ ] `产生编译错误`
- [ ] `输出空`
- [ ] `编译正确，运行错误`
- [ ] `输出0`

#### 在 ord_user 表中查找 username 以 G 开头的 SQL 语句是（）
- [ ] `SELECT * FROM ord_user WHERE username like 'G%'`
- [ ] `SELECT * FROM ord_user WHERE username == 'G%'`
- [ ] `SELECT * FROM ord_user WHERE username in 'G%'`
- [ ] `SELECT * FROM ord_user WHERE username like 'G_'`

#### What could be the result of attempting to compile and run the following piece of code?
```java
public class Test {
    public static void main(String args[]) {
        int x[] = new int[10];
        System.out.println("Value is " + x[5]);
    }
}
```
- [ ] `The output "Value is 0" is printed`
- [ ] `An object of type NullPointerException is thrown`
- [ ] `An "illegal array declaration syntax" compiler error occurs`
- [ ] `A "possible reference before assignment" compiler error occurs`
- [ ] `An object of type ArrayIndexOutOfBoundsException is thrown`

#### What is the output of the following application?
```java
package holiday;
enum DaysOff {
    Thanksgiving, PresidentsDay, ValentinesDay
}
public class Vacation {
    public static void main(String... unused) {
        final DaysOff input = DaysOff.Thanksgiving;
        switch (input) {
            default:
            case DaysOff.ValentinesDay:
                System.out.println("1");
            case DaysOff.PresidentsDay:
                System.out.println("2");
        }
    }
}
```
- [ ] `1`
- [ ] `2`
- [ ] `10`

#### Which of these classes properly implement(s) the singleton pattern?
```java
class ExamAnswers {
    private static ExamAnswers instance = new ExamAnswers();
    private List<String> answers = new ArrayList<>();
    public static List<String> getAnswers() {
        return instance.answers;
    }
}
class TestAnswers {
    private static TestAnswers instance = new TestAnswers();
    private List<String> answers = new ArrayList<>();
    public static TestAnswers getTestAnswers() {
        return instance;
    }
    public List<String> getAnswers() {
        return answers;
    }
}
```
- [ ] `ExamAnswers`
- [ ] `TestAnswers`
- [ ] `Both classes`

#### 下列数据类型转换，必须进行强制类型转换的是：
- [ ] `byte -> int`
- [ ] `short -> long`
- [ ] `float -> double`
- [ ] `int -> char`

#### 编译运行以下程序后，关于输出结果正确的是（）
```java
public class Test {
    public static void main(String[] args) {
        int x = 4;
        System.out.println("value is " + ((x==4?9:99.9)));
    }
}
```
- [ ] `输出结果为：value is 99.99`
- [ ] `输出结果为：value is 9`
- [ ] `输出结果为：value is 9.0`
- [ ] `编译错误`

#### 执行完以下代码 `int[] x = new int[25]` 后，以下哪项说明是正确的（）：
- [ ] `x[24]为0`
- [ ] `x[24]未定义`
- [ ] `x[25]为0`
- [ ] `x[0]为空`

#### 下面关于变量及其范围的陈述哪些是不正确
- [ ] `实例变量是类的成员变量`
- [ ] `实例变量用关键字 static 声明`
- [ ] `在方法中定义的局部变量在该方法被执行时创建`
- [ ] `局部变量在使用前必须被初始化`

#### 执行下列代码后 `String[] s = new String[10]`，哪个结论是正确的（）
- [ ] `s[9]为null`
- [ ] `s[10]为""`
- [ ] `s[0]为未定义`
- [ ] `s.length为10`

#### 输出1000以内的素数
```java
public class Test {
    public static boolean sushu(int num) {
        for (int i=2; i<=Math.sqrt(num); i++) {
            if (num % i == 0) {
                return false;
            }
        }
        return true;
    }

    public static void main(String[] args) {
        for (int j=2; j<=1000; j++) {
            if (Test.sushu(j)) {
                System.out.println(j + " 是素数");
            }
        }
    }
}
```

#### 实现一个时间复杂度为 O(n) 的算法，在存储一系列整数的数组中找出最大最小的两个？
```java
public class Test {
    public static void main(String[] args) {
        int[] test = {4, 5, 8, 1, 2, 0, 10};
        int max = test[0];
        int min = test[0];
        for (int j=1; j<test.length; j++) {
            if (test[j] > max) {
                max = test[j];
            }
            if (test[j] < min) {
                min = test[j];
            }
        }
        System.out.println("max = " + max);
        System.out.println("min = " + min);
    }
}
```