The finalize method in Object class has been deprecated Java 9 Onwards
Examples of Immutable classes in Java are String and all the wrapper classes like Integer,Float,Boolean etc

Here's what we need to do to create an immutable class.

declare the class as final so it cannot be extended
all class members should be private so they cannot be accessed outside of class
shouldn't contain any setter methods to change the value of class members
the getter method should return the copy of class members
class members are only initialized using constructor

final class Immutable {

  // private class members
  private String name;
  private int date;

  Immutable(String name, int date) {

    // class members are initialized using constructor
    this.name = name;
    this.date = date;
  }

  // getter method returns the copy of class members
  public String getName() {
    return name;
  }

  public int getDate() {
    return date;
  }

}



==============================================================


Collection is an interface
Collections is a class

Interface like List,Set and queue implement the collection interface
The map interface does not implement the collection interface


======================================================================

What is blocking queue

https://www.baeldung.com/java-blocking-queue

===========================================================================

Both Synchronized collection and concurrent collection provide thread safety to us
Main difference is Performance of these 2
Concurrent collections have a better performance than the synchronized collection
Reason is locking

==================================================================================

What is Try Catch Finally in Java

// try block contains risky code , the one which can possibly throw exceptions
// catch block catches the exception thrown by try block and performs appropriate information
// finally block is used for clean up activities like clsoing db connection or closing any other resource






==================================================================================================================





Throwable -------------Exception
          -------------Error


Exception ---------------------------CheckedException --------- File not Found, SQL Exception
          ---------------------------Unchecked Exception ------ Null Pointer Exception

===================================================================================================================


Differences between Error and Exception in Java

Exceptions are recoverable but error are not
Exceptions can be managed or handelled via try catch finally nothing can be done about errors
Exceptions can be checked or unchecked but errors are always unchecked
Exceptions are related to application but errors are related to environment where application runs


=====================================================================================================================

An Alone Try Statement will throw compilation error in Java, try either must have catch block or finally block

Try must be immediately followed by a catch block or finally block in between we cant write any statement

=====================================================================================================================

Difference Between Throw and Throws Keyword

Java Throw Keyword is used to Explicitly throw an exception  || Java Throws Keyword is used to declare an exception

Checked Exception Cant be propogated using throw only || Checked Exception can be propogated using throws

Throw is used with in the method || Throws is used with the method signature

You can't throw multiple exceptions || You can declare multiple exceptions

=====================================================================================================================

All Runtime exceptions are unchecked

=====================================================================================================================

All checked exceptions are subclasses of exception
All Unchecked Exceptions are subclasses of Runtime Exception

=====================================================================================================================


