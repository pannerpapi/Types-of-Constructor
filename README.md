
# Constructors-and-Destructors


##  Aim
To study and implement **Constructors** and **Destructors** in C++. 

---

##  Theory

In **Object-Oriented Programming (OOP)**, **constructors** and **destructors** play a crucial role in the **object lifecycle**.

- **Constructor**  
  A constructor is a special member function of a class that is automatically invoked when an object is created. Its main purpose is to **initialize data members**.  
  - Same name as the class  
  - No return type (not even `void`)  
  - Can be **default, parameterized, or copy** constructor  

- **Destructor**  
  A destructor is a special member function that is automatically invoked when an object goes out of scope or is explicitly deleted. Its purpose is to **free resources, close files, or clean up memory**.  
  - Same name as the class, prefixed with `~`  
  - No return type  
  - Cannot be overloaded  

Together, constructors and destructors ensure **automatic object management** and help reduce memory leaks, errors, and uninitialized data.  

---

##  Programs

###  Program 1 – Constructor Inside Class
This program demonstrates a constructor defined inside the class.  
**Class:** `Car`  
- Data members: `price`, `carname`, `mileage`  
- Constructor reads values from the user  
- `display()` function outputs details  

**Algorithm:**
1. Start  
2. Define class `Car` with members  
3. Define constructor inside class  
4. Define `display()` function  
5. Create object in `main()` → constructor runs automatically  
6. Display values  
7. End  

---

###  Program 2 – Constructor Outside Class
This program demonstrates a constructor defined **outside** the class using the scope resolution operator `::`.  

**Algorithm:**
1. Start  
2. Define class `Car`  
3. Declare constructor & `display()` inside class  
4. Define constructor & `display()` outside class using `Car::`  
5. Create object → constructor executes  
6. Display values  
7. End  

---

### Program 3 – Parameterized Constructor
This program demonstrates a **parameterized constructor** in the `Product` class.  
- Allows initialization of objects with values at the time of creation.  

**Algorithm:**
1. Start  
2. Define class ` with data members  
3. Define parameterized constructor with arguments  
4. Define `display()` function  
5. In `main()`, create object with arguments  
6. Display product details  
7. End  

---

###  Program 4 – Copy Constructor
This program demonstrates a **copy constructor** in the `student` class.  
- Used to create a new object as a copy of another object.  

**Algorithm:**
1. Start  
2. Define class `student` with members `prn`, `name`, `fee`  
3. Define parameterized constructor  
4. Define copy constructor to duplicate data  
5. Define `display()` function  
6. Create object `s` using parameterized constructor  
7. Create object using copy constructor  
8. Display both objects  
9. End  

---

###  Program 5 – Destructors
This program demonstrates the **use of constructors and destructors** to track object creation and destruction.  

**Algorithm:**
1. Start  
2. Initialize global counters  
3. Define class `destruct` with constructor & destructor  
4. In constructor → increment and display object count  
5. In destructor → decrement and display destroy  
6. Create objects in `main()`  
7. Inner block object goes out of scope → destructor called  
8. Remaining destructors run at program termination  
9. End  

---

##  Conclusion
These programs collectively demonstrate **core concepts of C++ OOP**:
- **Constructors** (default, parameterized, copy)  
- **Destructor** (object cleanup)  
- **Encapsulation and object lifecycle**  

Key learnings:
- Constructors ensure **automatic initialization** of objects.  
- Parameterized constructors allow **flexibility** in assigning values.  
- Copy constructors help in **cloning objects** safely.  
- Destructors ensure **automatic cleanup**, preventing memory leaks.  

## 📌 Author
Created as part of **B.Tech – OOPs in C++ Lab Work**.  
