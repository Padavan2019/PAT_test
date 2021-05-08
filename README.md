# PAT_test
每日练题！


**2021-0508**  
1.1001 害死人不偿命的(3n+1)猜想  
```
import java.util.Scanner;

public class Main{
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		int step = 0;
		
		while(num !=1) {
			if(num % 2 == 0) {
				num = num / 2;
				step++;
			}
			else {
				num = num*3 + 1;
				num = num / 2;
				step++;
			}
		}
		System.out.println(step);
	}

}
```
