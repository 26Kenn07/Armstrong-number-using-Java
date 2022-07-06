# Armstrong-number-using-Java
Check Armstrong Number of n digits using Java

package New;

import java.util.Scanner;

public class Number {
	
	public static void main(String[] args) {
		
		Scanner S = new Scanner(System.in);
		
		System.out.println("Enter a number:");
		int num = S.nextInt();
		int real;
		int n = 0;
		int ans = 0;
		int remain;
		
		real = num;
		
		for(real = num;real != 0; ++n) {
			real = real/10;
		}
		
		for(real = num; real != 0; real=real/10) {
			remain = real%10;
			
			ans = (int) (ans + Math.pow(remain,n));
		}
		
		if(ans == num) {
			
			System.out.println(ans + " is an Armstrong number");
			
		}
		
		else{
			
			System.out.println(ans + " is not an Armstrong number");
			
		}
	}

}
