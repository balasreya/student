# student
import java.util.*;
class student
{
    String name;
    int roll_no;
    Scanner k=new Scanner(System.in);
    void read()
    {
        System.out.println("enter the name");
        name=k.next();
         System.out.println("enter the number");
         roll_no=k.nextInt();
        
    }
}
class test extends student
{
    int m1,m2,m3,m4,m5,m6;
     Scanner k=new Scanner(System.in);
     void marks()
     {
       System.out.println("enter the marcks of 1st subject");
       m1=k.nextInt();
       System.out.println("enter the marcks of 2st subject");
       m2=k.nextInt();
       System.out.println("enter the marcks of 3st subject");
       m3=k.nextInt();
       System.out.println("enter the marcks of 4st subject");
       m4=k.nextInt();
       System.out.println("enter the marcks of 5st subject");
       m5=k.nextInt();
       System.out.println("enter the marcks of 6st subject");
       m6=k.nextInt();
     }
}
class result extends test
{
    void result()
    {
        int Totalmarks;
        Totalmarcks=m1+m2+m3+m4+m5+m6;
        System.out.println("enter the  total marks subject"+Totalmarks);
    }
}
class multilevelinheretence
{
    public static void main(String[]args)
    {
        Scanner k=new Scanner(System.in);
        System.out.println("enter the n");
        int n=k.nextInt();
        student s=new student();
        test t=new test();
        result r=new result();
        int i;
        for(i=0;i<=n;i++)
        {
            r.read();
            r.marks();
            r.result();
        }
    }
}
