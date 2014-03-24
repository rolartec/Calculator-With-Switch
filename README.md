Calculator-With-Switch
======================
//  By Reina Olarte

import java.util.Scanner;
// imports the scanner class

public class Switchcalculator 
{
//  Execution of Java program  (main Method begins)
	
	
	public static void main(String[] args)
	{
		
// Create a Scanner to input information
		Scanner input = new Scanner( System.in);
		//  Declaring the variables
		
		int Number1;
		int Number2;
		int Output;
		String operation;
		
		System.out.print("Enter the First Digit:  ");
		Number1 = input.nextInt();
		// Stores the input from user to number1 variable
		
		System.out.print("Enter the Second Digit:  ");
		Number2 = input.nextInt();
		
		System.out.print("Enter the Operation:\n(+ , - , * , / , % )");
		operation = input.next();
		
		
		switch (operation)
		{
			case "+":
					Output= Number1 + Number2;
					System.out.printf("\nThe Addition of %d + %d = %d\n", Number1, Number2, Output);
					break;
			case "-":
					Output= Number1 - Number2;
					System.out.printf("\nThe Subtraction of %d - %d = %d\n", Number1, Number2, Output);
					break;
			case "/":
					
					Output= Number1 / Number2;
					System.out.printf("\nThe Division of %d / %d = %d\n",Number1, Number2, Output);
					break;
			case "*":
					
					Output= Number1 * Number2;
					System.out.printf("\nThe Multiplication of %d * %d = %d\n",Number1, Number2, Output);
					break;				
					
			case "%":
				
				Output= Number1 * Number2;
				System.out.printf("\nThe Remainder of %d Mod %d = %d\n",Number1, Number2, Output);
				break;	
				
			default:
				
				System.out.println("\nWrong operator entered");
				break;
				
		}
}	// End method main

}	// End class
