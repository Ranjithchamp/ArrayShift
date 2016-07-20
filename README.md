# ArrayShift
import java.util.Scanner;

public class ArrayShift {

	
	public static void main(String[] args) {
		Scanner qq = new Scanner(System.in);
		System.out.println("enter size of array");
		int nn = qq.nextInt();
		int count[] = new int[nn];
		System.out.println("enter array element");
		for (int i = 0; i < nn; i++) {
			count[i] = qq.nextInt();
		}
		System.out.println("Enter no of digit to Shift :");
		int shift= qq.nextInt();
		int []ShiftArr=new int[nn];
		int k=0;
		for(int i=0;i<count.length;i++)
		{
			if((i+shift)<count.length)
			{
				k=i+shift;
				ShiftArr[k]=count[i];
			}
			else 
			{
				k=i-shift;
				ShiftArr[k]=count[i];
			}
			}
		System.out.print("Shifted Array : ");
		for (int h :ShiftArr){
			System.out.print(h+" ");
		}
			
		}
	}


