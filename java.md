<h1 id="1">java整理</h1>

[目录](#1)
<ol>
     <li>[Collection](#1.1)</li>
     <li>[HashTable HashMap比较？](#1.2)</li>
     <li>[PrepareStatment](#1.3)</li>
     <li>[比较记忆体空间](#1.4)</li>
     <li>[比较String](#1.5)</li>
     <li>[比较线程安全](#1.6)</li>
</ol>

字节流 - 以byte为单位<br>
字符流 - 以16位unicode为单位

super 调用父类的constructor 如果没有则采用预设的constructor

<h2 id="1.1">Collection</h2>

集合中只能存放对象 不可以使用基本的数据类型<br>
HashMap 适用在map中 插入 删除和定位元素<br>
TreeMap 适用于自然排序的情况<br>
HashMap较TreeMap快速

ArrayList 数组实现 查询快 增删慢 线程不安全(轻量)<br>
LinkList  链表实现 查询慢 增删快 线程不安全(轻量)<br>
Vector 数组实现 线程安全(重量)

<h2 id="1.2">HashTable HashMap比较？</h2>
<table>
     <tr>
         <th></th>
         <th>HashTable</th>
         <th>HashMap</th>
     </tr>
     <tr>
         <th></th>
         <th>AbstractMap</th>
         <th>Dictionary</th>         
     </tr>
     <tr>
         <th>是否同步</th>
         <th>是</th>
         <th>否</th>
     </tr>
     <tr>
         <th>k,v可否null</th>
         <th>否</th>
         <th>是</th>
     </tr>
 </table>

<h2 id="1.3">PrepareStatment</h2>

使用PrepareStatment的优缺点？
<ol>
     <li>简化代码</li>
     <li>提高访问数据库的性能</li>
     <li>PrepareStatment执行预准备的SQL语句 数据库只需编译一次SQL语句就可以多次执行故提高效率</li>
</ol>     

<h2 id="1.4">比较记忆体空间</h2>

== 比较记忆体空间<br>
equals 比较值<br>
String a = "test";
String b = new String("test");
String a = "te" + "st";
<br>if(a == b) //==>false
<br>if(a == c) //==>true
<br>if(a.equals(b)) //==>true


<h2 id="1.5">比较String</h2>

String StringBuffer StringBuilder比较？<br>
<ol>
     <li>String 不可变 StringBuilder可变</li>
     <li>StringBuilder 速度快但线程不安全</li>
     <li>StringBuilder 之所以可以使用链形式是因为 他在函式中返回的是自己的对象(return this)<br>
         ex. stringBuilder.append().append();</li>
     <li>另外StringBuilder如果容量不足会自动扩充</li>
     <li>StrigBuffer 速度慢但线程安全</li>
</ol>    


<h2 id="1.6">比较线程安全</h2>

线程安全<br>
synchronize<br>
volatile 强迫去主记忆体中获取东西<br>

