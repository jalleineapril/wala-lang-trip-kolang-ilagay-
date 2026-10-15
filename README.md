import java.util.Scanner;

public class Main{
    public static void main(String[]args){

Scanner input = new Scanner(System.in);
char continueChoice;

do{
System.out.println("===============================");
System.out.println("CLASS MONITORING REPORT SYSTEM:");
System.out.println("===============================");
        
System.out.println("Enter your name:");
String name = input.nextLine();
        
System.out.println("Enter your age:");
String age = input.nextLine();
        
System.out.println("Enter grade for HCI:");
double  HCIgrade = input.nextDouble();

System.out.println("Enter grade for CC103:");
double CC103grade = input.nextDouble();

System.out.println("Enter grade for Networking2:");
double Networking2grade = input.nextDouble();

double average = (HCIgrade + CC103grade + Networking2grade) / 3;

System.out.println("\n===============================");
        System.out.println("STUDENT REPORT SUMMARY:");
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("HCI Grade: " + HCIgrade);
        System.out.println("CC103 Grade: " + CC103grade);
        System.out.println("Networking2 Grade: " + Networking2grade);
        System.out.println("Average Grade: " + average);
        System.out.println("===============================");

System.out.println("Do you want to enter another report?(y/n:) ");
input.nextLine();
String response = input.nextLine();
continueChoice = response.charAt(0);
        
System.out.println("\n");       
} while (continueChoice == 'y'|| continueChoice == 'Y');

System.out.println("Thank you for using Class Monitoring Report System! ");
    }
}


