# CodSoft-task3

TASK 3: ATM INTERFACE

1.	Create a class to represent the ATM machine.
2.	Design the user interface for the ATM, including options such as withdrawing, depositing, and checking the balance.
3.	Implement methods for each option, such as withdraw(amount), deposit(amount), and checkBalance().
4.	Create a class to represent the user's bank account, which stores the account balance.
5.	Connect the ATM class with the user's bank account class to access and modify the account balance.
6.	Validate user input to ensure it is within acceptable limits (e.g., sufficient balance for withdrawals).
7.	Display appropriate messages to the user based on their chosen options and the success or failure of their transactions.

Ans:

	import java.util.Scanner;
	class Atm
	{
    public static void main(String [] args)
    {
       int a,bal=10000;
       float b,sum,c,d;
       System.out.println("1.Withdrawing Amount");
       System.out.println("2.Depositing Amount");
       System.out.println("3.Checking the balance");
       System.out.println("Choose your option");
       Scanner A=new Scanner(System.in);
       a=A.nextInt();
       if(a==1)
       {
         System.out.println("Enter Withdrwal Amount");
         c=A.nextFloat();
         if(c<bal)
         {
          d=bal-c;
          System.out.println("Current Balance:"+d);
         }
         else
         {
             System.out.println("Incaficient Balance");
         }
       }
       else if(a==2)
       {
          System.out.println("Enter Deposit Balance=");
          b=A.nextFloat();
          sum=b+bal;
          System.out.println("Current Balance="+sum);
       }
       else if(a==3)
       {
         System.out.println("Account balance="+bal);
       }
       else
       {
         System.out.println("Choose correct option");
       }
    }
	}

Instraction:

 	1. Copy Full code.
 	2. Save: Grade.java
 	3. Compile: javac Grade.java
 	4. Run: java Grade
