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

// WAP in Java to print currencies converted from 1 dollar 

class CurrencyConverter {

    int rupee=63;

    int dirham=3;

    int brazilian = 3;

    int chilean_peso = 595;

    int mexican_peso = 18;

    int _yen = 107;

    int $australian = 2;

    int dollar=0;

    int Rupee;

    void printCurrencies(){

        System.out.println("1 dollar in rupee: " + rupee);

        System.out.println("1 dollar in dirham: " + dirham);

        System.out.println("1 dollar in brazilian: "+brazilian);

        System.out.println("1 dollar in chilean peso: "+chilean_peso);

        System.out.println("1 dollar in mexican peso: "+mexican_peso);

        System.out.println("1 dollar in yen: "+_yen);

        System.out.println("1 dollar in australian: "+$australian);

    }

}
class Main{
    
    public static void main(String[] args)
    {
        CurrencyConverter cc=new CurrencyConverter();
        cc.printCurrencies();
    }
}

// WAP in Java to create a shopping cart of apple, banana and orange and the last option as checkout. It calculates total cost based on how many fruits are added 

import java.util.*; 

import java.io.*; 

public class shopping { 

    public static void main( String[]args ) 

    { 

        Scanner sc=new Scanner(System.in); 

        double cost=0; 

        int apple_quant=0; 

        int banana_quant=0; 

        int orange_quant=0; 

        int totalquantity=0; 

        System.out.println("Welcome to the Shopping Program!"); 

        while (true) 

        { 

            System.out.println("\nAvailable items"); 

            System.out.println("1.Apple \t- $0.50"); 

            System.out.println("2.Banana\t- $0.25"); 

            System.out.println("3.Orange\t- $0.75"); 

            System.out.println("4.Checkout"); 

            System.out.println("\n\nEnter your choice"); 

            int c= sc.nextInt(); 

            if((c<=3)&&(c>=1)) 

            { 

                System.out.println("Enter Quantity"); 

                int q=sc.nextInt(); 

                if(q==0) 

                { 

                    while(q==0) 

                    { 

                        System.out.println("Invalid quantity"); 

                        q=sc.nextInt(); 

                    } 

                } 

                if(c==1) 

                { 

                    cost+= 0.50*q; 

                    apple_quant+=q; 

                } 

                else if(c==2) 

                { 

                    cost+= 0.25*q; 

                    banana_quant+=q; 

                } 

                else if(c==3) 

                { 

                    cost+=0.75*q; 

                    orange_quant+=q; 

                } 

                System.out.println("Item added to your cart"); 

            } 

            else if(c==4) 

            { 

                break; 

            } 

            else{ 

                System.out.println("Invalid Choice.\nPlease Enter a valid choice"); 

            } 

        } 

        totalquantity= apple_quant+banana_quant+orange_quant; 

        System.out.println("\nItems in your cart :");         

        if(apple_quant!=0) 

        { 

            System.out.println("Apple \tX"+apple_quant); 

        } 

        if(banana_quant!=0) 

        { 

            System.out.println("Banana\tX"+banana_quant); 

        } 

        if(orange_quant!=0) 

        { 

            System.out.println("Orange\tX"+orange_quant); 

        } 

        System.out.println("Total items in cart"+totalquantity+"\nTotal cost"+cost); 

   }   

} 
