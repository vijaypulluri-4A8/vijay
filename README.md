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
