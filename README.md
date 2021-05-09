# PAT_test
每日练题！


**2021-0508**  
1.1001 害死人不偿命的(3n+1)猜想  
```java
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

**2021-0509**  
1.1011 A+B 和 C 
```java
import java.util.Scanner;
public class P0509_01 {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);

		int m=sc.nextInt();
		long[][] num= new long[m][4];
		
		for(int i=0;i<m;i++) {
			for(int j=0;j<3;j++) {
				num[i][j] = sc.nextLong();
			}
			if((num[i][0] + num[i][1]) > num[i][2]) {
				num[i][3] = 1;
			}
			else {
				num[i][3] = 0;
			}
		
		}
		for(int k=0;k<m;k++) {
			System.out.print("Case #" + (k+1) + ": ");
			if(num[k][3] == 1) {
				System.out.println("true");
			}
			else {
				System.out.println("false");
			}
		}
	}

}

```
