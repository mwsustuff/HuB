Design patterns 
=================================================
* Designpattens are set of rules which come as best solutions for re-occuring problems of 
application development.
* Designpattens are best practices to use s/w technologies much effectively.
* The worst solution for reocurring problems if application develop is called anti pattern.
* The iso organization maintained documentation of both design patterns and anti patterns.
* Most of the design patterns are given by Four people called Gof(Fama,Fleem,Johnson and Vlissed)

__Every Design pattern contain The following essential details__
pattername
problem
solution
consequences.
 
We can implmenet these Design patterns in multiple languages and Techologies
java is most suitable language to implement design pattern.

 Classfication of Design patterns
 -----------------------------------

Mainly There are 3 basic classfications of patterns 
1. __Creational Patterns__:-- The process of object creation
  * AbstractFactory patterns
  * Builderpattern
  * Factorypattern
  * ProtoType pattern
  * singleton pattern
2. __Structural patterns__:-- Deal with the Composition of classes and objects. How objects and classes can be combined to form larger structure.
  * Adapterpattern
  * Bridgepattern
  * compositepattern
  * Decoratorpattern
  * Facadepattern
  * flyweight pattern
  * proxypattern

3 __Behavioral patterns__:-- Deal with the interaction of classes and objects
  * ChainofResponsiblitypattern
  * commandpattern
  * interpreterpattern
  * iterator pattern
  * mediatorpattern
  * Momoent pattern
  * Observerpattern
  * statepattern
  * starategypattern
  * Templatepattern
  * visitor pattern

> Now we can see the Regularly used design patterns in real time java projects as they are classfied based on the type of applciations which we are developing.
 
 Corejavalevel or Standalone Application level Designpatterhs
=============================================================
* FactoryMethod DesignPattern
* SingleTon DesignPattern
* Synchronized singleton DesignPattern
* Factory pattern DesignPattern
* AbstractFactory DesignPattern
* Builder DesignPattern
* ProtoType DesignPattern
* Template method DesignPattern
* Adapter DesignPattern
* FastlineReader DesignPattern
* DTo/Vo Design pattern
* Ioc or Dependency Injection Design pattern
* Fly Weight DesignPattern

### Web Level designPattern

* Mvc1&Mvc2 DesignPattern
* ViewHelperDesignPattern
* Compositeview DesignPattern
* FrontController DesignPattern
* InterceptingFilter DesignPattern
* Abstract controller Design pattern

### Enterprise Application level Design patterns
================================================
* DAO DesignPattern
* DAO Factory DesignPattern
* ServiceLocator DesignPattern
* BusinessDelegate DesignPattern
* SessionFacade DesignPattern
* MessageFacade DesignPattern

Note:  Integration Tier design patterns:-- ServiceLocation,Businedeligates,dao
Buseiness tier-->sessionfacade,messagefacde,business object.

FactoryMethod DesignPattern
============================
 __problem__
When a java class hving private constructor , then outside of that class object creation of that class is not possible

__solution__
use Factory method desginpatten

*def*: (Factory method is java method) The method in javaclass which is capable of constructing its own javaclassobject is called factory method .
__Application Areas__
 When java class is hving only private constrcutor then in order to create object of that java class
 outside of that class, we use Factory method.
 To make java class as immutable java class(like  java.lang.String) we use factory method as helper class or code.
__Rules to use this Factory method__

1. The factory method should hv current class name as return type.
2. Method definitation should hv logic of creating & returning current class object.
3. factory method must be a public method.

> note: The factory method can be static factory method or an instance factory method
if current class is an abstract class, then method should return one of its subclass object.

static factory method is usefull to create an object f a java class outside of that class when that class is hving only private Constrcutor.
~~~
ex:  Some of the examples for predefined methods.are.
a)Class c=Class.forName(--);
b)Thread t=Thread.currentThread();
~~~
> note: Java class can hv Factory methods even though that class is hving public constructor.
instance factory method usefull to create a new object for java class by useing existing object and its data.
ex: Example for predefined instance factory methods is
String s1="welcome to shiva online Training";//Existing object
String s2="s1.substring(s1);//new Objectt...

eg:
~~~
class A
{
int a=100;
private A()
{


}

public static A funA()
{

A  b=new A();
return b;

}
}

class B
{

public static void main(string[]args)
{
A  b=A.funA();// factory method design patterns
// Class.forName()

}


}
~~~
eg:
~~~
class Test
{
	int x;
	//private zero argument constructor
	private Test()
	{
		System.out.println("Test : ):-arg Con");
	}
	//Static factory method
	public static Test staticFactoryMethod()
	{
		Test t=new Test();
		t.x=5;
		return t;
	}
	//instace factory method
	public Test instanceFactoryMethod()
	{
		Test t=new Test();
		t.x=this.x+5;
		return t;
	}
	public String toString()
	{
		return "x="+x;
	}
}//Test
public class FactoryEx {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Test t=Test.staticFactoryMethod();
		System.out.println(t);//which internally calls toString();
		Test t1=t.instanceFactoryMethod();
		System.out.println(t1);

	}

}
~~~
eg:--
~~~
Class c=Class.forName(---)
Thread t=Thread.currentThread();
String s=String.valueOf(20);
~~~

Now we can see one example on how we can develop our own  immutable java class by useing factory method.

__Defination of immutable javaclass:__

immutable class is java class which once created its contnets cannot be changed .immutable object are the java objects whose state cannot be changed once constructred eg:string class.
__Advanatages with immutable nature__
Immutable objects are automatically thread-safe,the overhead casused due to use of Synchronization is avoided.
once created the state of the immutable object cannot be changed so there is not possiblity of them geting into inconcstistent state.
__rules__
1. take class as final class (or) make method and memeber variale as final.
2. to take all member varibles as private
3. if mehod demands to modfy data take that method as factory method.
eg
~~~

public class Demo {

	/**
	 * @param args
	 */
private String name;
public Demo(String name, int no) {
		super();
		this.name = name;
		this.no = no;
		System.out.println("2-argument constructor");
	}

private int no;
public Demo()
{
	System.out.println("0-argument constructor");
}

	public Demo(String name) {
	super();
	this.name = name;
	System.out.println("1-Stringargument constructor");
}

	public Demo(int no) {
	super();
	this.no = no;
	System.out.println("0-intargument constructor");
}
~~~
~~~
	//instance factory method
	public Demo modifyName(String s)
	{
		Demo d=new Demo();
		d.no=this.no;;
		return d;
	}
	//instance factory method
	public Demo modifyNo(int n)
	{
		Demo d=new Demo();
		d.name=this.name;;
		return d;
	}
	public String toString()
	{
		return "Name="+name+"  NO="+no;
	}
	}

~~~
~~~
class ImmutableTest
{
	public static void main(String[] args) 
	{
		Demo d=new Demo("shiva",31);
		System.out.println("Hahscode of d object:"+d.hashCode());
		System.out.println(d.toString());
		System.out.println();
		
		Demo d1=d.modifyName("sirisha");
		System.out.println("Hahscode of d1 object:"+d1.hashCode());
		System.out.println(d1);
		System.out.println();
		
		Demo d2=d.modifyNo(25);
		System.out.println("Hahscode of d2 object:"+d2.hashCode());
		System.out.println(d2);
		System.out.println();
		
		
		System.out.println("Hello World!");
	}
}
~~~
### SingleTon DesignPattern



__problem__

creating mutiple objects for java class with same data is wastage of memory..

__solution__

use Singleton java class,which says create only one object for java class and use it for multiple times
on each jvm in order to minimize the memory wastage and to increase the performance.

__def__: Stingleton java class ,which allowes us to create only one object per jvm.


The method in javaclass which is capable of constructing its own javaclassobject is called factory method .
java class that allowes to create only one object per jvm is called singletonjavaclass.

note: For a normal java class if programmer or container is creating only one object even though that class allowes to create multiple object then that java class is not singleton java class.
According to this,then a java class of servlet program is not singleton java class. it is a normal java class for which servelt container creates only one object.

__Applicability__

The singleton pattern should be used when there must be exactly one instance of a class,and when it must be accessible to clients from a global access point.
If multiple applications of a project that are running from a single jvm wants to work with objects
of java class hving same data then it is recommendend to make that java class as singleton java class. so that only one object will be allowed to create for that class and we can use that object for multiple applications.

ex:
   most of of jdbc driver classes are given as singleton java classes for bettern utilization
   in log4j environemnt,the Logger class is given as singleton java class.
   java.lang.Runtime class is singleton java class.
__Rules to develop singleton java class__

1)take  private static referece varible of the current class as instance varible
2)To preven instantating the class more then once, take private constructor so that an instance can be created only from within the static method of the class.
3)develop static factory method,which will return an instance of current class,or null, if the class has already been instanatiated.
4)override clone() and return the above created object to suppress the object creation throght cloning process.


eg:
====
class A
{
private static A n=null;
private A()
{

System.out.println("constructor");
}

static A funA()
{

if(n==null)
n=new A();
return n;
}
public static void main(string[]args)
{
funA();
funA();
funA();



}


}

eg
=====

public class Demo1 {

	/**
	 * @param args
	 */
private static Demo1 instance;
private Demo1()
{
	System.out.println("Demo : )-param con");
}
//static factory method
public static Demo1 getInstance()
{
	//Singleton logic
	if(instance==null)
		instance=new Demo1();
	return instance;
}
//Override Object class clone()
public Object clone()
{
	return instance;
}
//normal method
public void called()
{
	System.out.println("The normal method will be called");
}
}


public class SingleTonPatternTest {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub

	Demo1 d=Demo1.getInstance();
	System.out.println("Hashcode of d object"+d.hashCode());
	d.called();
	Demo1 d1=d.getInstance();
	System.out.println("Hashcode of d1 object"+d1.hashCode());
	d1.called();
	
	Demo1 d2=(Demo1)d.clone();
	System.out.println("Hashcode of d2 object"+d2.hashCode());
	d2.called();
	
	
	}

}
========================================================================
TemplatemethodDesignPattern
=======================
Instead of invoking mulitple different methods to combined task,it is recommendd to combine all these methods into a single method 
task1--->a(),b(),C()

task2--->a(),b(),C()

task3--->a(),b(),C()
         
	 void a(){}
	 void b(){}
	 void c(){}
	       abc()--->Templatemethod designpattern
	       {
a();
b();
c();

	       }
task1--->abc

task2--->abc

task3--->abc
         
	 CommandLine View Design pattern
	 ===============================
	 class Test
	 {

	 bm()
	 {}
bm1()
	 {}

}

class client
{
p s.v.m()
{
bm();
bm1();

}
}
class client1
{
p s.v.m()
{
bm();
bm1();

}
}

class Command
{
abc()
{
bm();
}
xyz()
{
bm1();
}
}

class client
{
p s.v.m()
{
abc();
xyz();
}
}
class client1
{
p s.v.m()
{
abc();
xyz();

}
}
Prototype deisgnPattern
========================
Istead of creating multiple objects for same java class which consumes lot of time it is recommeded to create only one object and make multiple copies of the same object either by usieng cloning approach or any other approach,later modify them as appropriate


Adapter designPattern
==============
interface xyz
{
a();
b();
c();
}
interface Abc
{

x();
y();
}
class client imple xyz,Abc
{
//here each and every method implementation.....
}
class client1 imple xyz,Abc
{
//here each and every method implementation.....
}


abstract class Adapter implements abc,xyz
{
a(){}
b(){}
c(){}
x(){}
y(){}
}

class client extends Adapter
{
a()

{
implementation
}
class client1 extends Adapter
{
x()
{}

}

Factory Pattern
=================
problem
=====
creating multiple objects for multiple subclasses and utilizing one of them based on the supplied data is wrong methodolgy bcz the remaining objects became unnecssarily
created objects.

Solution
=====
here the mehtod of super class or some other class instantiates/creates one of the several subclasses obj
ect based on the supplied data provided by user(at compile time/at runtime)that means objects for remaining subclasses will not be created.

Def: Define an inteface for creating an object,but let the sbclasses decide which class to instatiate . the factory method lets a class defer instatiation to subclasses.

eg:
===
In jdbc Applications DriverManager.getConnection(---) method logic is nothing but factory pattern logic 

EG
===
abstract class ShapeEx
{
public abstract void draw();
}
class Line extends ShapeEx
{
public line()
{
System.out.println("You are choosen line to Draw");
}
public void draw()
{
System.out.println("line to Draw()");;
}
}
class Square extends ShapeEx
{
public Square()
{
System.out.println("You are choosen squre to Draw");
}
public void draw()
{
System.out.println("square to Draw()");;
}
}

public class FactoryPattenTest
{


public static void main(String[]args)
{
FactoryPattenTest fp=new FactoryPattenTest();
ShareEx s=fp.getShapre(args[0]);//data is supplied at runtime

}

//Factory pattern logic
public ShapeEx getShape(String  shapes)
{
if(shape.equals("L"))
return new Line();
else if(shape.equals("s"))
return new Square();
else
return null;


}

}

AbstractFactoryPattern
=====================
prvide an interface for creating dependent object without specifying their concrete classes.

eg
===
abstract class College
{
public abstract Display getBranchName();
public abstract Display getCount();
}
class Cse extends College
{
public  Display getBranchName()
{
return new Display("cse");
}
public Display getCount()
{
return new Display("120");
}
}//end cse

class It extends College
{
public  Display getBranchName()
{
return new Display("IT");
}
public Display getCount()
{
return new Display("90");
}
}//end It

class MCA extends College
{
public  Display getBranchName()
{
return new Display("MCA");
}
public Display getCount()
{
return new Display("60");
}
}//end It
class Display
{
pulbic String value;
public Display(String s)
{
this.value=s;
}
public String getValue()
{
return value;
}
}

public class AbstractFactoryPatternTest
{

private College cname;
public Static void main(String[]args)
{
AbstractFactoryPatternTest af=new AbstractFactoryPatternTest();
College c=ag.getCollege("IT);
System.out.println("Object is created"+c.getClass());
System.out.println("BranchName is "+c.getBrachName().getValue());
System.out.println(c.getBrachName().getValue()+"Branch contains "+c.getCount().getValue()+"No.ofStudent");
}

//Factory pattern Logic
public College getCollege(String s)
{
if(s.equals("CSE");
cname=new CSE();
else (s.equals("IT");
cname=new It();
else (s.equals("MCA");
cname=new MCA();

return cname;
}
}

BuilderDesign pattern
========================
Builder as thename suggest builds complex objects from simple ones step-by-step.Itseparates the constructor of complex objects from their representation
problem
======
In order to complete a task working with simple and individual objects is always complex process to perform

solution
===============
use this patter,which says creates complex object fro simple objects and work with that complex object to complete the task.
eg
===
class CPU
{

public String name()
{
return "cpu";
}
public int price()
{
return 7000;
}
}
class Monitor
{
public String name()
{
return "Monitor";
}
public int price()
{
return 5000;
}
}

class Perphirals
{
public String name()
{
return "perphilrals";
}
public int price()
{
return 4500;
}
}
public class BuilderTest
{
public static void main(String[] args) 
	{
BuilderTest b=new BuilderTest();
String s=bt.parts();
int cost=bt.calPrice();
System.out.pritnln("Your product constist of"+s);
System.out.pritnln("Your product Total coast"+cost+"/-");
		System.out.println("Hello World!");
	}
public String parts()
{
return "One"+new Cpu().name()+"One"+new Monitor().name()+"&some"+new Perphirals().name();

}

public int calPrice()
{
return new Cpu().price()+new Monitor().price()+new Perphirals().price();
}
}
DI/ioc
======
The process of Injecting(pushing)the depencecies into an object is known as dependecy injection .

Mvc(Model View Control)
=======================
Model
Model2

DataTransferObject
===================
Dto(DataTransferObject)/vo(ValueObject)
============================================
probleam-1
==========
We cannot send jdbc Resultset Object from one layer to another layer over the network bcz it is not a serliable object
              To solve the requirement copy JdbcResultSetObject data to any collection f/w data structure
	      and send that data structure over the network. since all collection f/w data structure are by default serializable objects.

	      Note: if you are just performing read operation on collection framework data structures then you can take any non-Synchronized data Structure like Arraylist.if you want to perform read,
	      update,delete etc... operations on collection f/w data structure then use any synchronized data structure like vector.
probleam-2
==========

While transfering ResuletSet object record to set/list data structure elements the following problem will be raised. we cannot move each record of ResultSet object to each element of Arraylist object bcz each record of ResultSet object may contains multiple values where as each element of ArrayList can store only
one java object at a time.

Solution
============
create a user defined java class object hving each record values and add tha object to the elements
of ArrayList .Here the class of that user defined object is called as DTO/Vo class (it is generally a java Bean)

def: Useing a serializable class to act as a data carrier,grouping related attributes,froming a compositvalue and working as return type from remote business method. also known as value object.

note: teh elements added to collection framework data structure must be taken as serializabl object in order to send that collection  f/w data structure over the network.

note: Logic to transfer ResultSet object to Arraylist Object by taking the support of DTO/Vo

CompositeViewDesignpattern
=============================
FRontController Desigpattern
===============================
is a spacial webresource program of a web applciation that is capable of trapping and taking the request coming to toher web resources of web application by hving common and global pre-requesting processing logic eg: ActionServlet in struct 1.x ,springwebmvc DispatchServlet...
    The frontController design pattern means that all request taht come for a resource in an application will be handled by a single handler and then dispatched to the appropriate thandler for that type
    of request the front controller may use other helpers to achieve the dispatching mechaism.

    note: The front contoller design pattern is applicable and usefull for all kind of applications be it web or desktop applciations and is not limited to any single programing language or f/w
  Abstract Controller
  ====================
Abstract Controller is the helper class for front controller(servlet/jsp) it provides environment to programer to customize the logic of front controller.

ex: in Structs 1.x environment Requestprocessor class acts as Abstract controller for the FrontController(ActionServlet);
In structs 1.x environemtn,if you wnat to customize the logic of ActionServlet(Front constoller) then we hv to develop custom RequestProcessor class(Abstract Controller) and then instantiates in front contoller and call its methods.


Dao(DataAccessObject) DesignPattern
======================================
problem
================
In any project if persistence is combined with the other logics of the application(like Businesslogic,Servicelogic)Then persistence logic will not become Flexible to modify the modifications done
in persistence logic may distub other logics of the applications.
Solution:Use DAo Designpattern.
def: The java class or Component that separates persistence logic from other logics of the application to make persistence logic as flexible logic to modify is called as DAO.
  Generally Dao class it Contains.
     Logic to establish the connection
     Logic to release the connection
     Logic to perform persistnece operations like update,delete insert.
     some transaction managment code.(if required)
  
  A single Dao class/Component can be used by  all business components or each business componetn can contain their own dao class/Component. But it is alwasy recommended to use separate dao classes/component for each business component.
we can develop this Dao classs/Component useing my persistence logic like jdbc,Hibernate,EjbEntitybean ,spring-jdbc,spring-ormcomponent.etc....
Eg:
====
//BaseDao.java
===============
public class BaseDao
{
    public static Connection getConnection()
    {
----
----
    }
    public int insert(--,--)
    {
---
----

    }

    public List fetch()
    {
    ---
    ---
    }
    public static void closeConnection()
    {
    ---
    ---
    }}

    public class Bcomp1
    {
    public Bcomp1()
    {

Connection con=BasicDao.getConnection();
    }

    public void insertRecords()
    {
    ---
    con.insert(--,--);
    }
    public void fetchREcords()
    {

    ---
    con.fetch(--);
    ---
    }}

DAOFACTORYDESIGNPATTERN
=========================
The DaoFactory desing pattern is nothing but an extension to DAo design pattern.
Generally we can use DaoDesign patterns in order to separate persistence logic from other logics
of the application.Here implemented Dao class/Component contains persistence logic with respective to a single a database.If you wnat to work with multiple databases then go through the DAOFActory design pattern.

Def: DaoFactory design pattern is class or component,which contains logic of constructoring and returning one database sowtware specific Dao class object based on the database software name we are provided 
Dao factory design pattern is  a combination of both Factory pattern and DaoDesign pattern.

  This design pattern helps the programer to change the database sofware of the project with minimum changes done in jdbc persistence logic.
  Eg
  =====
  //BComp1aseDao.java
  public abstract class BComp1aseDao
  {
  public abstract Connection getConnection();
  public abstract void closeConnection();
  public abstract int insert(--);
public abstract list fetch(--);
public static BComp1aseDao chooseDao(String dbname)
{
if(dbname.equals("Oracle"))
{

return new comp1OracleDAO();
}
else if(dbname.equals("sqlserver"))
{

return new comp1mySqlDAO();
}
else
{

throw new Exception("Please provide Existed D/bname");
return null;

}


}

public class comp1OracleDAO extends BComp1aseDao
{
public static Connection getConnection()
    {
----
----
    }
    public int insert(--,--)
    {
---
----

    }

    public List fetch()
    {
    ---
    ---
    }
    public static void closeConnection()
    {
    ---
    ---
    }}


public class comp1MysqlDAO extends BComp1aseDao
{
public static Connection getConnection()
    {
----
----
    }
    public int insert(--,--)
    {
---
----

    }

    public List fetch()
    {
    ---
    ---
    }
    public static void closeConnection()
    {
    ---
    ---
    }}


 public class Bcomp1
    {
BComp1aseDao dao=null;

    public Bcomp1()
    {

dao=BComp1aseDao.chooseDAO("oracle");
    }

public void bm1()
{
dao.getConnection();
//write some business logic
//implemet some persisten logic
dao.insert(---);
dao.closeConnection();


}


 public class Bcomp1
    {
BComp1aseDao dao=null;

    public Bcomp1()
    {

dao=BComp1aseDao.chooseDAO("mySql");
    }

public void bm1()
{
dao.getConnection();
//write some business logic
//implemet some persisten logic
dao.insert(---);
dao.closeConnection();


}

