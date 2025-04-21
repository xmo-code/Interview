### 一、Object对象方法有哪些

1. getClass() - 获取运行时的 Class 对象，属于反射机制的一部分，可用于获取运行时的相关数据。
	```java
	Object obj = new String("example");
	Class<?> clazz = obj.getClass();
	System.out.println(clazz.getName()); 
	```
	- 注意点
		- 反射机制会带来一定的性能开销，因为它需要在运行时动态解析类的信息。
		- 使用反射时可能会破坏类的封装性，因为可以绕过访问修饰符直接访问和修改类的成员。
