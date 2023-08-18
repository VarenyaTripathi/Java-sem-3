# Java-sem-3


// WAP in Java to get student name, registration number, marks in 5 subjects and their average 

package day2; 
 
import java.util.Scanner; 
 
public class program1 { 
 
public static void main(String[] args) { 
String name,reg_no; 
float marks[]=new float[5];; 
Scanner sc=new Scanner(System.in); 
System.out.println("Enter name:"); 
name=sc.nextLine(); 
System.out.println("Enter registration number:"); 
reg_no=sc.nextLine(); 
float sum=0; 
for(int i=0;i<5;i++) 
{ 
System.out.println("Enter marks "+(i+1)+":"); 
marks[i]=sc.nextFloat(); 
sum=sum+marks[i]; 
} 
float avg=sum/5; 
System.out.println("The average of marks is: "+avg); 
} 

 

// WAP in Java to calculate cgpa of 3 semesters of a student 

package day2; 
 
import java.util.Scanner; 
 
public class program2 { 
 
public static void main(String[] args) { 
Scanner sc=new Scanner(System.in); 
float gpa[]=new float[3]; 
float sum=0,cgpa=0; 
for(int i=0;i<3;i++) 
{ 
System.out.println("Enter gpa of sem"+(i+1)+":"); 
gpa[i]=sc.nextFloat(); 
sum=sum+gpa[i]; 
} 
cgpa=sum/3; 
System.out.println("The cgpa is:"+cgpa); 
} 
 
} 
