# java-lab
//difference B/W global variable and local variable 

1-- code 

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


2-- code 
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

*WRITE THE PROGRAME FOR:
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
