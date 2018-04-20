import java.util.ArrayList;
public class sorting{
public static void main(String a [] ) {
	int [] ar1 = {108,55,22,32,14,9,64,13,91,27,18,7};
	System.out.println("Before: ");
	for (int i : ar1) {
		System.out.print(i + " ");
	}

	int count = 0;
	for(int  i =0; i< ar1.length-1;i++) {
		int index = i;
		for(int j =i+1;j<ar1.length;j++) {
			if(ar1[j]<ar1[index]) {
				index= j;
				count++;
			}
		}
		int s = ar1[index];
		ar1[index]= ar1[i];
		 ar1[i]= s;
		 
}
	System.out.println("\nAfter:");
	 for (int e : ar1) {
			System.out.print(e + " ");
		}
	 System.out.println("\nSteps: "+count);
	 
int mynum=18;


	
	}
}
