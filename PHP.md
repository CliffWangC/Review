<h1 id="1">PHP整理</h1>

* [目录](#1)
     * [Magic Method](#1.1)
     * [HashTable HashMap比较？](#1.2)
     * [PrepareStatment](#1.3)
     * [比较记忆体空间](#1.4)
     * [比较String](#1.5)
     * [比较线程安全](#1.6)
     
<h2 id="1.1">Magic Method:</h2>
<ul>
  <li>__construct()，类的构造函数</li>
  <li>__destruct()，类的析构函数</li>
  <li>__call()，在对象中调用一个不可访问方法时调用</li>
  <li>__callStatic()，用静态方式中调用一个不可访问方法时调用</li>
  <li>__get()，获得一个类的成员变量时调用</li>
  <li>__set()，设置一个类的成员变量时调用</li>
  <li>__isset()，当对不可访问属性调用isset()或empty()时调用</li>
  <li>__unset()，当对不可访问属性调用unset()时被调用。</li>
  <li>__sleep()，执行serialize()时，先会调用这个函数</li>
  <li>__wakeup()，执行unserialize()时，先会调用这个函数</li>
  <li>__toString()，类被当成字符串时的回应方法</li>
  <li>__invoke()，调用函数的方式调用一个对象时的回应方法</li>
  <li>__set_state()，调用var_export()导出类时，此静态方法会被调用。</li>
  <li>__clone()，当对象复制完成时调用</li>
  <li>__autoload()，尝试加载未定义的类</li>
  <li>__debugInfo()，打印所需调试信息</li>
</ul>
