import java.util.InputMismatchException;
import java.util.Scanner;
public class Main{
  public static void main(String[]args){
    Scanner scanner=new Scanner(System.in);
    int a,b;
    while(true){
      try{
        System.out.println("enter the number 1:");
        a=scanner.nextInt();
        System.out.println("enter the number 2:");
        b=scanner.nextInt();
        System.out.println(a+b);
        break;
      } catch (InputMismatchException e){
        System.out.println("entereed wrong format.please enter again");
        scanner.nextLine();
      }
    }
  }
}
