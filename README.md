Printing Hollow Square Star Pattern
In this program we’re going to code a java program for hollow square star pattern program. A hollow square star pattern is one with star only on its boundaries and free space on all other places.
Take a input from user, for determining the number of rows and columns, and store it in the variable named as row and col, respectively and then write a “for loop” starting from i=1 to i<=row and then take another for loop to start from j=1 to j<=col and then we’ll use a  if statement “if(i==1 or i==col) or (j==1 or j==col)” for printing the stars on the desired places.

Hollow Square Star Pattern
Algorithm:
Take number of rows input from the user and store it in any variable (‘row’ in this case).
Take number of coloum input from the user and store it in any variable (‘col’ in this case).
Run  a loop ‘i’ number of times to iterate through all the rows. From i=1 to i<=row. The loop should be structured as for (int i = 1; i <=row; i++).
Run a nested loop inside the main loop for printing stars . From j=1 to j<=col. The loop should be structured as for (int j = 1; j <= col; j++).
Inside the above loop print stars only if  i==1 or i==col or j=1 or j=col in all other cases print a blank space.
Move to the next line by printing a new line. System.out.println();.
Code in Java:
import java.util.Scanner;
public class Pattern1 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter row and col">);
		int row = sc.nextInt();
		int col = sc.nextInt();
		for (int i = 1; i <=row; i++) {
			for (int j = 1; j <= col; j++) 
				if((i==1 || i==col) || (j==1 || j==col))
					System.out.print("*");
				else
					System.out.print(" ");
			
			System.out.println();
			
		}
	}
}
