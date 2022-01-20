# Introduction to Object Oriented Programming

### Classes and Objects
A **class** is a template for an object, whereas an **object** is an instance of a class. A class may contain only data, or only code, or both. 

Thus, the class is a blueprint from which objects are created. 

```
Person P = new Person()
```

*NOTE: In Java, all concepts must be encapsulated within a class.*


```
class class_name() {
	data_type instance_var1;
	data_type instace_var2;

	data_type method() {//}
}
```


##### A Demo
```
class rect {
	int l;
	int b;
}

public class demo {
	public static void main(String args[]) {
		rect r = new rect();

		// We have not initialized rect.
		System.out.println(r.l);
		System.out.println(r.b);

		// In Java, nothing is initialized to garbage.

		r.l = 10;
		r.b = 20;
		System.out.println(r.l);
		System.out.println(r.b);
	}
}
```


### Access Modifiers
Java offers four types of access modifiers:
	 **Private**. Accessible within class only. Cannot be accessed from outside class. 
	 **Default**. Accessible within package only. Cannot be accessed from outside 
                    package. Without specifying access level, this will be the default. 
	 **Protected**. Within package, as well as outside but only through the child class. If a 
                     child class is not created, this cannot be used beyond the package.
	**Public**. Accessible at all points. 

Any member function that is declared using the `static` keyword is a *static member function*. As a result, it can be called without an instance of the class. 

![[Pasted image 20220120085217.png]]

