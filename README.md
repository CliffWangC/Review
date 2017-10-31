# java整理

super 调用父类的constructor 如果没有则采用预设的constructor

集合中只能存放对象 不可以使用基本的数据类型
HashMap 适用在map中 插入 删除和定位元素
TreeMap 适用于自然排序的情况
HashMap较TreeMap快速

ArrayList 数组实现 查询快 增删慢 线程不安全(轻量)
LinkList  链表实现 查询慢 增删快 线程不安全(轻量)
Vector 数组实现 线程安全(重量)

HashTable HashMap比较？
                 HashTable     HashMap
父类            AbstractMap    Dictionary
是否同步            是              否
k,v可否null         否              是

使用PrepareStatment的优缺点？
1. 简化代码
2. 提高访问数据库的性能
3. PrepareStatment执行预准备的SQL语句 数据库只需编译一次SQL语句就可以多次执行故提高效率


== 比较记忆体空间
equals 比较值
String a = "test";
String b = new String("test");
String a = "te" + "st";
if(a == b) //==>false
if(a == c) //==>true
if(a.equals(b)) //==>true

String StringBuffer StringBuilder比较？
1. String 不可变 StringBuilder可变
2. StringBuilder 速度快但线程不安全
3. StringBuilder 之所以可以使用链形式是因为 他在函式中返回的是自己的对象(return this)
   ex. stringBuilder.append().append();
4. 另外StringBuilder如果容量不足会自动扩充
5. StrigBuffer 速度慢但线程安全

线程安全
synchronize
volatile 强迫去主记忆体中获取东西
