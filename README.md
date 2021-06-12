# vijay/*Lab 2.1)Write a Java program to select all the prime numbers within the range of 1 

to100. */

class PrimeNumbers{

	public static void main(String[] args) {		

    

        int i,j,temp=0;

    

        System.out.println("Prime numbers in the range of 1-100"+" ");

		for(i=1;i<=100;i++)

		{

			for(j=1;j<=i;j++)

			{

				if(i%j==0)

				{

					temp++;

				}

			}

      

			if(temp==2)

			{

				System.out.print(i+" ");

			}

				temp=0;

		}

	}

}
/*Lab 2.2)Write a program to print sum of even numbers in Fibonacci sequence*/

import java.util.Scanner;

class FibonacciSum

{

	public static void main(String[] args)	{

		int n,sum=0,f,temp,i,x=0,y=1;

		Scanner s=new Scanner(System.in);

		System.out.print("Enter a number:");

		n=s.nextInt();

		for(i=0;i<=n;i++)

		{

			temp=x;

			f=x+y;

			x=y;

			y=f;

			if(temp%2==0)

			{

				sum=sum+temp;

			}

		}
    
    System.out.println("sum of even numbers in Fibonacci sequence"+sum);

		

	}

}
