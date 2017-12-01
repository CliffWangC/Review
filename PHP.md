//========PHP===========

Magic Method:<br>
__construct()，类的构造函数<br>
__destruct()，类的析构函数<br>
__call()，在对象中调用一个不可访问方法时调用<br>
__callStatic()，用静态方式中调用一个不可访问方法时调用<br>
__get()，获得一个类的成员变量时调用<br>
__set()，设置一个类的成员变量时调用<br>
__isset()，当对不可访问属性调用isset()或empty()时调用<br>
__unset()，当对不可访问属性调用unset()时被调用。<br>
__sleep()，执行serialize()时，先会调用这个函数<br>
__wakeup()，执行unserialize()时，先会调用这个函数<br>
__toString()，类被当成字符串时的回应方法<br>
__invoke()，调用函数的方式调用一个对象时的回应方法<br>
__set_state()，调用var_export()导出类时，此静态方法会被调用。<br>
__clone()，当对象复制完成时调用<br>
__autoload()，尝试加载未定义的类<br>
__debugInfo()，打印所需调试信息<br>
