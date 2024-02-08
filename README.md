# Nested-if
import java.util.Scanner;

public class Nested {

	public static void main(String[] args) {
		Scanner sc=new Scanner(System.in);
		
		System.out.println("Enter fn");
		String fn=sc.nextLine();
		
		System.out.println("Enter qty");
		int qty=sc.nextInt();
		int cost=0;
		
		if(fn.equals("Apple"))
		{
			if(qty<=20)
			{
				cost=qty*5;
			}
			else {
				cost=qty*7;
			}
			System.out.println("The cost of the Apple = "+cost);
		}
			
		else if(fn.equals("Kiwi"))
		{
			if(qty<=10)
			{
				cost=qty*2;
			}
			else if((qty>=10)&&(qty<=25))
			{
				
				cost=qty*4;
			}
			else 
			{
				cost=qty*6;
			}
			System.out.println("The cost of the Kiwi = "+cost);
		}
		else if(fn.equals("Banana"))
				{
			if(qty<=100)
			{
				cost=qty*3;
			}
			else 
			{
				cost=qty*4;
			}
			System.out.println("The cost of the Banana = "+cost);
			
				}		

	}

}
