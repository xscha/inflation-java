# Inflation Project

This project asks for the cost of an item, the number of years from now that the item will be purchased, and the rate of inflation. This program will output the estimated cost of the item after a period of time. 

````java
import java.util.Scanner;
public class inflation{
  public static void main (String[] args){
  Scanner input = new Scanner(System.in); // this line will allow the program to read the user inputs.

  System.out.println("Enter your cost: "); // this line asks the user to enter the cost of the item.
    double cost = input.nextDouble(); // initializes the cost
  System.out.println("Enter the number of years of inflation: "); //input the number of years of inflation
    int years = input.nextInt(); //initializes the years
  System.out.println("Enter the amount of inflation in percentage"); //inputs percentage of inflation
    double inflation = input.nextDouble(); //initialize inflation
    inflation = inflation / 100; //converts inflation percentage to decimal

  for(int x = 0; x < years; x++)
    cost += cost * inflation;
  System.out.printf("Your item will cost about $%,.2f in %d years. ", cost, years); //this will print out the calculation
  }
}
````

Once input, the outcome should be as follows: 

<b><img width="415" alt="Screenshot 2025-02-13 221906" src="https://github.com/user-attachments/assets/ab917d37-6631-4581-876c-5c3f8a2db945" />
