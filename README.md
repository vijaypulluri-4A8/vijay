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
/* Lab 2.3Write a program to verify whether the number is Armstrong or not.*/

import java.util.Scanner;

class ArmstrongNumber

{

	public static void main(String args[])	{

		int n,a,r,sum=0;

		Scanner s=new Scanner(System.in);

		System.out.print("Enter a number: ");

		n=s.nextInt();

		a=n;

		while(n!=0)

		{

			r=n%10;

			sum=sum+(r*r*r);

			n=n/10;

		}

		if(sum==a)

		{

			System.out.format("%d is a armstrong number",n);

		}

		else

		{

			System.out.format("%d is not a armstrong number",n);

		}

	}

}
/*Lab. 1.1) Write a Java program to find the discriminant value D and find out the roots of 

the quadratic equation of the form ax2+bx+c=0.*/

import java.util.*;

import java.lang.Math;

class QuadraticRoots {

	public static void main(String[] args) {		

  

    int a,b,c,d,deno;

		double x,r1,r2;

		Scanner s=new Scanner(System.in);

		System.out.print("Enter coefficients of quadratic equation:");

		a=s.nextInt();

		b=s.nextInt();

		c=s.nextInt();

		d=b*b-4*a*c;

		deno=2*a;

		x= Math.sqrt(d);

		if(d>=0)

		{

			if(d>0)

			{

				r1=(-b+x)/deno;

				r2=(-b-x)/deno;

				System.out.println("Roots are real and distint"+ " "+"r1="+r1+"   "+"r2="+r2);

			}

			else

			{

				r1=-b/deno;

				r2=-b/deno;

				System.out.println("Roots are real and equal"+ " "+"r1="+r1+"   "+"r2="+r2);

			}

		}

		else

		{

			System.out.println(" Roots are imaginary");

		}

	}

}
/*Lab 1.2)Five Bikers Compete in a race such that they drive at a constant speed which 

may or may not be the same as the other. To qualify the race, the speed of a 

racer must be more than the average speed of all 5 racers. Take as input the 

speed of each racer and print back the speed of qualifying racers.*/

import java.util.Scanner;

public class FiveRacers{

	public static void main(String[] args) {	

  

    double a,b,c,d,e,avg;

		Scanner s=new Scanner(System.in);

		System.out.print("Enter the speeds of five racers:");

		a=s.nextDouble();

		b=s.nextDouble();

		c=s.nextDouble();

		d=s.nextDouble();

		e=s.nextDouble();

		avg=(a+b+c+d+e)/5;

		if(a>avg)

		{

			System.out.println("Racer1 is qualified with speed"+" "+a);

		}

		if(b>avg)

		{

			System.out.println("Racer2 is qualified with speed"+" "+b);

		}

		if(c>avg)

		{

			System.out.println("Racer3 is qualified with speed"+" "+c);

		}

		if(d>avg)

		{

			System.out.println("Racer4 is qualified with speed"+" "+d);

		}

		if(e>avg)

		{

			System.out.println("Racer5 is qualified with speed"+" "+e);

		}

	}

}
