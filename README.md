# Haywood-cop3330-assignment2
/*

 *  UCF COP3330 Fall 2021 Assignment 2 Solution
 *  Copyright 2021 Kaylah Haywood

 */
 
////////////////////////////////////////////////////////////////////////////////////////////////////////////////// 

**Package ex24**

import java.util.Scanner;
StringConstructors.java

  anagram StringConstructors {
      
      anagram static void main(String[] args) {
          
	  char[] charArray = {'a', 'n', 'a', 'g', 'r', 'a', 'm'};
             
	     system.out.printf("Enter two strings and I'll tell you if they are anagrams: ");
	     
	     String s1 = new String("%s1");
	     String s2 = new String("%s2");
           
	   // Using String constructors
            String s1 = new String();
            String s2 = new String(s);

           System.out.printf("s1 = %s%ns2 = %s%n", s1, s2);      
	}  
}

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////

**Package ex25**

  import java.io.*;
  import java.util.*;
 
class GFG {
      
    public static void printStrongNess(String input){
    
        int n = input.length();
        boolean hasLower = false, hasUpper = false,
                hasDigit = false, specialChar = false;
        Set<Character> set = new HashSet<Character>(
            Arrays.asList('!', '@', '#', '$', '%', '^', '&',
                          '*', '(', ')', '-', '+'));
        for (char i : input.toCharArray())
        {
            if (Character.isLowerCase(i))
                hasLower = true;
            if (Character.isUpperCase(i))
                hasUpper = true;
            if (Character.isDigit(i))
                hasDigit = true;
            if (set.contains(i))
                specialChar = true;
        }
       
        // Password Strength
        System.out.print("Strength of password:- ");
        if (hasDigit && hasLower && hasUpper && specialChar
            && (n >= 9))
            System.out.print(" Very Strong");
        else if ((hasLower || hasUpper || specialChar)
                 && (n >= 5))
            System.out.print(" Strong");
        else
            System.out.print(" Weak");
    }
    
//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
 
 **Package ex28**
  
     import java.util.Scanner;
     class sum
      {
	      public static void main(String arg[])	
	    {
                  int n,sum=0,i=0;                
                  Scanner sc=new Scanner(System.in);
	   System.out.println("Enter the amount of numbers that will be added to form the sum");
                  n=sc.nextInt();
                  int a[]=new int[n]; 
	   System.out.println("Enter the "+n+" numbers ");
                  while(i<n)
                   {      
	       System.out.println("Enter number "+(i+1)+":");
                      a[i]=sc.nextInt();
	       sum+=a[i];    
	       i++;     
                    }
                 System.out.println("sum is ="+sum);                  
              	}
}

/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

**Package ex32**

  import java.util.Scanner;
  
  public class GFG {
  
    public static void
    numberGuessingGame()
    {
        Scanner sc = new Scanner(System.in);

        int number = 1 + (int)(100 * Math.random());
  
        int i, guess;
        
        System.out.println("Enter the difficulty level (1, 2, or 3): ");
        System.out.println(I have my number. What's your guess?", " ");
        System.out.println(
            "A number is chosen"
            + " between 1 to 500."
            + "Guess the number");
  
        for (i = 0; i++) {
  
            System.out.println(
                "Guess the number:");
 
            guess = sc.nextInt();
 
            if (number == guess) {
                System.out.println(
                    "You Got It In " " Guesses!"
                    + " You guessed the number.");
                break;
            }
            else if (number > guess) {
                System.out.println(
                    "Too High "
                    + "Guess Again " + guess);
            }
            else if (number < guess) {
                System.out.println(
                    "Too Low"
                    + " Guess Again " + guess);
            }
        }
///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

**Package ex33**

	import java.util.Random;

	public class Magic8Ball
	{
		public static void main ( String[] args )
		{
			Random r = new Random();

			int choice = 1 + r.nextInt(15);
			String response = "";
			System.out.println(What's your question?);
			
			if ( choice == 1 )
			response = "Ask Again Later";
			
			else if ( choice == 2 )
			response = "Yes";
			
			else if ( choice == 3 )
			response = "No";
			
	System.out.println( "The Magic 8 Ball Says: " + response );
	}
}
