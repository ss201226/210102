# 210102
package basic;
//0102
import java.util.Scanner;

public class CodeUp1468 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc=new Scanner(System.in);
		int n=sc.nextInt();
		int[][] arr=new int[n][n];
		int x=1;
		for (int i = 0; i < n; i++) {
				if(i%2==0) {
					for (int j = 0; j < n; j++) {
						arr[i][j]=x;
						x+=1;
					}			
				}
				else {
					for (int j = n-1; j >= 0; j--) {
						arr[i][j]=x;
						x+=1;
					}					
				}							
		}
		for (int i = 0; i < n; i++) {
			for (int j = 0; j < n; j++) {
				System.out.print(arr[i][j]+" ");
			}
			System.out.println();
		}		
	}
}
