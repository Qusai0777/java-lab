# java-lab
//difference B/W global variable and local variable 

==1-- code 

public class PI
{
    static int a=10;
    public static void main(String[]args)
{
    int b=20;
    System.out.println(a);
    System.out.println(b);
    P1();
}
public static void P1()
{
    System.out.println(a);
    System.out.println(b);
}
}

output:
ERROR!
javac /tmp/1TjEu8Mm7C/PI.java
/tmp/1TjEu8Mm7C/PI.java:14: error: cannot find symbol
    System.out.println(b);
                       ^
symbol:   variable b
  location: class PI
1 error


==2-- code 
public class PI
{
    static int a=10;
    public static void main(String[]args)
{
    int b=20;
    System.out.println(a);
    System.out.println(b);
    P1();
}
public static void P1()
{
    System.out.println(a);
  //  System.out.println(b);
}
}
output:
10
20
10

*WRITE THE (JAVA)PROGRAME FOR:
1) PRE INCREAMENT
2) POST INCREAMENT
3) PRE DICREMENT
4) POST DICREAMENT


==1) PRE INCREAMENT

class pi {
    public static void main(String[] args) {
        int a=7;
        ++a;
        System.out.println(a);
    }

    OUTPUT
    8



 ==2) POST INCREAMENT


   class pi {
    public static void main(String[] args) {
        int a=7;
       System.out.println(a++);
        System.out.println(a);
    }
}

OUTPUT
7
8



==3) PRE DICREMENT

class pi {
    public static void main(String[] args) {
        int a=7;
        --a;
        System.out.println(a);
    }
    }

OUTPUT
6



==4) POST DICREAMENT

class pi {
    public static void main(String[] args) {
        int a=7;
       System.out.println(a--);
        System.out.println(a);
    }
}

OUTPUT
7
6



*Q)* explain type casting with example

--A)
Type Casting in Java:
In Java, type casting is a method or process that converts a data type into another data type in both ways manually and automatically.

Type casting
Convert a value from one data type to another data type is known as type casting.

Types of Type Casting
There are two types of type casting:

--Widening Type Casting
--Narrowing Type Casting

Widening Type Casting
Converting a lower data type into a higher one is called widening type casting. It is also known as implicit conversion or casting down. It is done automatically. It is safe because there is no chance to lose data. It takes place when:

The target type must be larger than the source type.
byte -> short -> char -> int -> long -> float -> double  

WideningTypeCastingExample.java::


public class WideningTypeCastingExample  
{  
public static void main(String[] args)  
{  
int x = 7;  
//automatically converts the integer type into long type  
long y = x;  
//automatically converts the long type into float type  
float z = y;  
System.out.println("Before conversion, int value "+x);  
System.out.println("After conversion, long value "+y);  
System.out.println("After conversion, float value "+z);  
}  
}  

Output

Before conversion, the value is: 7
After conversion, the long value is: 7
After conversion, the float value is: 7.0



Narrowing Type Casting
Converting a higher data type into a lower one is called narrowing type casting. It is also known as explicit conversion or casting up. It is done manually by the programmer. If we do not perform casting then the compiler reports a compile-time error.

The target type must be larger than the source type.
double -> float -> long -> int -> char -> short -> byte  

public class NarrowingTypeCastingExample  
{  
public static void main(String args[])  
{  
double d = 166.66;  
//converting double data type into long data type  
long l = (long)d;  
//converting long data type into int data type  
int i = (int)l;  
System.out.println("Before conversion: "+d);  
//fractional part lost  
System.out.println("After conversion into long type: "+l);  
//fractional part lost  
System.out.println("After conversion into int type: "+i);  
}  
}  
Output

Before conversion: 166.66
After conversion into long type: 166
After conversion into int type: 166




==even or odd using ternary operator==

public class pi{
    public static void main(String[] args) {
        int a=1;
        
       System.out.println(a%2==0?"even":"odd");
    }
}

==OUTPUT==
odd




==The if Statement==
* Use the if statement to specify a block of Java code to be executed if a condition is true.

  *SYNTAX*

  if (condition) {
  // block of code to be executed if the condition is true
}
