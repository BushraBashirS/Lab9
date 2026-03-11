# PRG210 \- Lab 9

In this lab, you will be working with Microsoft Visual Studio 2022 to create a solution named Lab9. Within this solution, you will create a single project to implement a class. This lab is the continuation of Lab 8, so you will need the files stock.cpp and stock.h from Lab 8. Follow the instructions given below.

## Instructions for creating solution and projects

## Create a New Solution

1. Open Microsoft Visual Studio 2022\.  
2. In the Create a new project dialog, select Empty Project.  
3. Click Next.  
4. Uncheck the checkbox: "Place solution and project in the same directory".  
5. For the Project name, type StockInheritance.  
6. Enter lab9 as the Solution name.  
7. Choose a location to save the solution. This should be: "C:\\Users\<yourusername\>\\PRG210\\Labs"  
8. Click Create. This will create the solution and project for the first task.  
9. For any subsequent tasks, follow the steps in \#2. below.

## Create Projects for Each Task

## Copy The Files from Lab8

* Copy the files `stock.h`, and `stock.cpp` from lab 8 and add them into this project.

## Instructions for Lab submission

* Take screenshots wherever required.  
* Name the screenshots as the project name (task1.jpg, task2.jpg, etc)  
* Add the screenshots in a word document in the correct order.  
* Export the word document as pdf. Name the PDF as StudentName\_Lab9.pdf.  
* Submit the pdf on Blackboard.  
* The following deductions apply:  
* Incorrect screenshot names: \-20% of overall grade.  
* Incorrect document name: \-20% of overall grade.  
* Missing username in the terminal: \-100%

## **Investigation 1: Derived Class for Preferred Stocks**

### **Task 1: Derived Class for Preferred Stocks**

* Add a new class  `PreferredStock` that inherits from `Stock` using public inheritance.
* Let's also change access specifier of base class data members to protected
* Add a private member double `dividendRate` to store the stock’s dividend percentage, in `PreferredStock` class.  
* Declare a constructor in `PreferredStock` that takes:  
  * `companyName`  
  * `shares`  
  * `sharePrice`  
  * `dividendRate`  
* Initialize the base class data members by calling appropriate base class constructor, and initialize `dividendRate` as well in derived class constructor.  
* Implement the **show()** function in `PreferredStock` that shadows `Stock::show()`. In this method you should first display Stock data members by calling base class show method and then display `dividendRate`.  
* Open main.cpp, create two `PreferredStock` class objects, and display their details.  
* Build the solution and run `main.exe` from the terminal.  
* Take screenshots of the code and output. Put them under the heading **`task1`** in the document **`StudentName_Lab9.doc`.**

### **Task 2: Shadowing a Member Variable in Derived Class**

* In **PreferredStock**, declare a new public data member: **long shares** that will shadow **Stock::shares**.  
* Implement a **setShares()** function in `PreferredStock` that updates only the new **shares** variable in the derived class.  
* Add a member function **getBaseShares** in **PreferredStock** that returns the original shares from the base class.  
* Open **main.cpp** and create a **PreferredStock** object.  
* Update its shares by using **setShares()**. 
* Print both **PreferredStock::shares** using object’s `shares` data member and **Stock::shares** using **getBaseShares** to demonstrate shadowing.  
* Save all files.  
* Build the solution and run `main.exe` from the terminal.  
* Take screenshots of the code and output. Put them under the heading **`task2`** in the document **`StudentName_Lab9.doc`.**

### **Task 3: Order of Constructors & Destructors in Derived Classes**

* Add the following constructor messages in both `Stock` and `PreferredStock` to track object creation:  
  * Base Constructor called  
  * Derived Constructor called  
* Add a destructor in `PreferredStock` that prints a message when an object is destroyed.  
* Add the following destructor messages in both `Stock` and `PreferredStock` to track object destruction:
  * Base Destructor called  
  * Derived Destructor called  
* In **main.cpp**, create two `PreferredStock` objects.  
* Build the solution and run `main.exe` from the terminal.  
* After the execution, explain both the object’s  and destruction in your own words in **comments** above the **main** function.  
* Take screenshots of the code and output. Put them under the heading **`task3`** in the document **`StudentName_Lab9.doc`.**

 
## Lab 9 Sign-Off
- Submit the PDF document `StudentName_Lab9.pdf` on BB.

