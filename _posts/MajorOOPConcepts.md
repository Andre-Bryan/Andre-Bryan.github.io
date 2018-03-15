---
layout: post
title:  "Object Orientation and Major Object Orientation Concepts"
date:   2018-02-11
desc: "Quick test on writing code snippets in a blog post"
keywords: "Java, Encapsulation, Polymorphism, Inheritance, Abstraction, Object-Orientation"
categories: [SoftwareDev]
tags: [Java, Python, Encapsulation, Polymorphism, Inheritance, Abstraction, Object-Orientation]
icon: icon-html
---
A programming paradigm that is very common is called Object Oriented Programming. Much like the name implies this paradigm is based around what is called "objects". These objects hold data which I refer to as attributes and code which I call methods. So instead of the traditional programming concept which revolves around actions and data, Object Oriented Programming revolves around objects. This shifts the focus of how to do something with full on logic to how can we manipulate the attributes and methods of the object to complete our task. Object Oriented Programming is not an easy concept to grasp but after messing around with it and getting hands on practice it is not that bad. When it comes to Object Oriented Programming(OOP) there are 4 major concepts:Encapsulation, Abstraction,Polymorphism, and Inheritance.

# Encapsulation`
Encapsulation is the wrapping of code and data into a single unit. An example is a Java class.
```
/* File name : Employee.java */
class EmployeeCount
{
   private int numOfEmployees = 0;
   public void setNoOfEmployees (int count)
   {
       numOfEmployees = count;
   }
   public double getNoOfEmployees ()
   {
       return numOfEmployees;
   }
}
public class EncapsulationExample
{
   public static void main(String args[])
   {
      EmployeeCount obj = new EmployeeCount ();
      obj.setNoOfEmployees(5613);
      System.out.println("No Of Employees: "+(int)obj.getNoOfEmployees());
    }
}
```
---
## Abstraction
Abstraction is the process of hiding internal details and showing functionality. Essentially it is the process of just showing what needs to be shown, show only what is relevant.

```
/* File name : Employee.java */
public class Main{
	public static void main(String args[]){
        TwoWheeler test = new Honda();
        test.run();
    }
}
abstract  class TwoWheeler {
    public abstract void run();
}
class Honda extends TwoWheeler{
	public void run(){
		System.out.println("Running..");
	}
}


```
### Polymorphism
Polymorphism is a task that is performed in different ways.

```
/* File name : Employee.java */
class DisplayOverloading
{
    public void disp(char c)
    {
         System.out.println(c);
    }
    public void disp(char c, int num)  
    {
         System.out.println(c + " "+num);
    }
}
public class ExampleOverloading
{
   public static void main(String args[])
   {
       DisplayOverloading obj = new DisplayOverloading();
       obj.disp('a');
       obj.disp('a',10);
   }
}
```

#### Inheritance
Inheritance is when an object acquires the same properties and behavior of parent object. It allows for the reuse of code. In order to inherit a class the keyword to use in extend.

```
/* File name : Employee.java */
class ChildClass extends ParentClass {


}
```
