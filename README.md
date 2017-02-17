1. 
import java.util.*;
public class acad {

	public static void main(String[] args) {
		Scanner ss = new Scanner(System.in);
		int a=ss.nextInt();//Input number
		int b=ss.nextInt();//Input number
		int d =ss.nextInt(); //Input number
		sum(a,b);//method called with two variables
		
		System.out.println(sum(a,b));//method called with two variables
		System.out.println(sum(a,b,d));//method called with three variables
		//print the result
		ss.close();
	
	
	}

	static int sum(int a,int b)//method to add two variables
	{
		
		
		int c;
		c=a+b;
		return c;
		
	}
	
	static int sum(int a,int b,int d)//method to multiply two variable and add third
	{
		int c;
		c=a*b+d;
		return c;
	}
}
/*we can overload the method with the same return type till when we have a different number
of variables in the the argument
if the methods have same number of arguments then if will throw an error*/

2.
import java.util.*;
public class acad {

	public static void main(String[] args) {
		Scanner ss = new Scanner(System.in);
		System.out.println("Input the size of an array");
		int a=ss.nextInt();//Size of an array
		ArrayList<String> d = new ArrayList<String>(a);//String array declared
		System.out.println("Enter the elements of the array");
		for(int i=0;i<a;i++)
		{
			d.add(ss.next()); //elements to be stored in an array
			
			
		}
		Collections.sort(d,Collections.reverseOrder());//for descending order arrangement
		System.out.println("Sorted Array");
		for(int j=0;j<a;j++)//display of the array as a sequence
		{
			System.out.println(d.get(j));
		}
		ss.close();
		
	}
	}
