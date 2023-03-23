# java

import java.util.Scanner;
public class Exam {
	public static void main(String args[]) {
		Scanner sc = new Scanner(System.in);

		System.out.print("실수1을 입력하시오 : ");
		int a = sc.nextInt();
		System.out.print("실수2를 입력하시오 : ");
		int b = sc.nextInt();
		System.out.print("연산자를 입력하시오 : ");
		char op = sc.next().charAt(0);

		if( op=='+') {
			System.out.println( a+" + "+b+" = "+(a+b) );
		}
		else if( op=='-') {
			System.out.println( a+" - "+b+" = "+(a-b) );
		}
		else if( op=='*') { 
			System.out.println( a+" * "+b+" = "+(a*b) );
		}
		else if( op=='/') {
			System.out.println( a+" / "+b+" = "+(a/b) );
		}
		else if( b==0 ){
			System.out.println("0으로 나눌 수 없음");
		}
		else {
			 System.out.println("사칙연산자가 아닙니다.");
		}
	}
}
