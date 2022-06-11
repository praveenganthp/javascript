# javascript
DAY || 2  => TASK

😎😎😊🙄😐
1.DIFFERENCE B/W HTTP1.1 AND HTTP2 ==>
HTTP1.1 :
* it work on the textual format.
* there is head of line is blocking that blocks all the requestsnbehind it until it doesn't get its all resources.
* it uses requests resources lnlining for use getting multiple pages.
* it compress data by itself.

HTTP2 :
* it works on the binary protocol.
* it allows multiplexingn. so one TCP connection is required for multiple requests.
* it uses PUSH frame by server that collects all multiple pages.
* it uses HPACK for data compression.

😎😎😊🙄😐
2.OBJECT'S AND ITS INTERNAL REPRESENTATION IN JAVASCRIPT :
   JavaScript is designed for on a simple object based paradigm. An object is colllection of properties, and a property is an association between a name and a value. A property value can be a function, in which case the property is known as a method.
   A JavaScript object has properties associated with it. A property of an object can be explained as a variable as a variable that is attached to the object. Object properties are basically the same as ordinary JavaScript variables, except for the attachment to objects. The properties of an object define the characteristics of the object. We can access the properties of an object with a simple dot-notation:
   objectName.propertyName
   
   Like all JavaScrript variables, bot the object name (which could be a normal variable) and property name are casse sensitive. You can define a property by assigning it a value. For example, let's create an object named myCar and give it properties named make , model and year as follows:
   var myCar = new object();
   myCar.make ='ford';
   myCar.model='mustang';
   myCar.year=1969;
   
   
 The above example could also be written using an object initializer, which is a comma-delimited list of zero or more pairs of property names and associated values of an object, enclosed in curly braces({}):
 var myCar={
 make:'ford',
 model:'mustang',
 year:1969
 };

 JAVASCRIPT'S INTERNAL REPRESENTATION OF OBJECTS:
   A simle ddiagram is probably the best way to give a quick overview of the object representation in JavaScript.
   ![0_o7djQk16c9fY-BYz](https://user-images.githubusercontent.com/87014435/173168432-fac16492-6e38-4d32-87f5-1831f689fde4.png)
   Most objects contain all their properties in a single block of memory('a' and 'b'). All blocks of memory have a pointer to  map, which describes their structure.
   Named properties that don't fit in an object are usually storeed in an overflow array('c' and 'd').
   
   numbered properties are stored separately, usually in a contiguous array.
   The JavaScript standard allows developers to define objects in a very flexible way, and it is hard to come up with an efficient representation tat works for everything. An object is essentially a collection of properties: basically key-value paits. We can access properties using two different kind of expressions:
   * obj.prop
   * obj["prop"]

According to the spec, property names are always strings. If we use a name that is not a string , it is implicitly converted to a string. This may be a little surprising : if we a number as a property name, it gets converted to a string as well. so a javascript object is basically a map from strings two values.


   

