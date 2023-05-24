package transposition;
import java.util.*; 
public class TrabsitionCipher { 
 
 	public static void main(String[] args) { 
 	 	 
 	 	Scanner sc = new Scanner(System.in); 
 	 	System.out.println("Enter the string: "); 
 	 	 
 	 	String msg = sc.nextLine(); 
 	 	 
 	 	int no_of_Rows=3; 
 	 	String msg1 = msg.replaceAll(" ", ""); 
 	 	 
 	 	 
 	 	 
// 	 	System.out.println(msg.charAt(0)); 
 	 	System.out.println("The origanal Msg is: "+ msg); 
 	 	System.out.println("The origanal msg after removing all the Spaces: "+msg1); 
 	 	System.out.print("The Encrypted msg is: ");  	 	for(int i=0;i<msg1.length();i++) 
 	 	{ 
 	 	 	if(i%4==0) 
 	 	 	{ 
 	 	 	 	System.out.print(msg1.charAt(i)); 
 	 	 	} 
 	 	} 
 	 	 
 	 	for(int i=1;i<msg1.length();i++) 
 	 	{ 
 	 	 	if((i+1)%2==0) 
 	 	 	{ 
 	 	 	 	System.out.print(msg1.charAt(i)); 
 	 	 	} 
 	 	} 
 	 	for(int i=2;i<msg1.length();i++) 
 	 	{ 
 	 	 	if((i+2)%4==0) 
 	 	 	{ 
 	 	 	 	System.out.print(msg1.charAt(i)); 
 	 	 	} 
 	 	} 
 
 	} 
 
} 
