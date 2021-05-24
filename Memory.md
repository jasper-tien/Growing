## AutoreleasePool
[黑幕背后的Autorelease](http://blog.sunnyxx.com/2014/10/15/behind-autorelease/)  
[自动释放池的前世今生 ---- 深入解析 autoreleasepool](https://draveness.me/autoreleasepool)  
[autorelease的使用场景](https://blog.csdn.net/fly1183989782/article/details/71325701)  
[引用计数带来的一次讨论](https://www.jianshu.com/p/e3690f3e4675)  


## 引用计数
[iOS内存管理的那些事儿-原理及实现](https://juejin.im/post/5c0744f6e51d45598b76f481)  
[iOS内存管理（MRC、ARC）深入浅出](https://www.jianshu.com/p/f03a4d32dc41)  

## ARC下dealloc过程
[ARC下dealloc过程及.cxx_destruct的探究](http://blog.sunnyxx.com/2014/04/02/objc_dig_arc_dealloc/)
1、父类的dealloc是在子类dealloc执行完以后，自动调用的
2、根类（一般是指NSObject）的dealloc会做：移除有关联关系的对象；释放所有的实例变量；清空引用计数表并清除弱引用表，将所有weak引用指nil；

