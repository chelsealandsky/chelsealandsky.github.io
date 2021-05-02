---
layout: post
title:      "Classes and Instances"
date:       2021-05-02 14:09:14 +0000
permalink:  classes_and_instances
---

Ruby methods have two main types - classes and instances - each with different tasks that they perform. While first learning about these methods, I found myself often confusing the methods with each other, as they can seem a little abstract. In writing this, I hope to clear up some of the confusion and help distinguish between the two. 

Classes are methods that create an object by creating a new instance of the class. Instances, on the other hand, are the objects created by the class. Class methods are called on the class itself, which why you use the self identifier (self.method_name) when calling the method. Instances methods are called on a particular instance of the class, which is why they are called similarly to normal methods (method_name). Class methods can only be called on classes and instance methods can only be called on instances. 

Methods defined in classes that are not class methods with the 'self' identifier will always be instance methods and will be available to future instances of that class. 

In example:

Class Chelsea
   def self.hello                                                        #class method
	    puts "hello I'm Chelsea"
	 end
		def hello_there                                                   #instance method
		   puts "hello I'm Chelsea 1.0"
	 end
end

In the above class method, calling Chelsea.hello would put "hello I'm Chelsea" just fine because it is a class method being called on the class, but calling Chelsea.hello_there would cause a NoMethodError because you cannot call an instance method on the class itself. To get this instance method to work, we would have to call it on an instance of the Chelsea class. If we try Chelsea.new.hello_there we would see "hello, I'm Chelsea 1.0", meaning this instance method works on this newly created instance of the Chelsea class. If we tried calling Chelsea.new.hello, however, we would get another NoMethodError because we cannot call a class method on an instance of that object. 

Pretty cool, huh?

