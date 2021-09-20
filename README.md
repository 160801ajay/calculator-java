import java.util.*;
class Calculator {

  public static void main(String[] args) {
  int i,j,ch,ch1;
    Scanner read = new Scanner(System.in);
  
    while(true)
    {
    System.out.print("press 1 to continue: ");
    ch1= read.nextInt();
    while(ch1==1)
    { System.out.print("Enter two numbers: ");
       i= read.nextInt();
       j= read.nextInt();

    // nextDouble() reads the next double from the keyboard
 
    System.out.print("Enter 1 for add");
    System.out.print("Enter 2 for sub");
    System.out.print("Enter 3 for mult");
    System.out.print("Enter 4 for div");
    ch= read.nextInt();

    int result = 0;

    switch (ch) {
      case 1:
        result = i + j;
        System.out.println("addition ="+result);
        
        break;

      case 2:
        result = i- j;
        System.out.println("subtraction ="+result);
        
        break;

      case 3:
        result = i * j;
        System.out.println("multiplication ="+result);
        
        break;

      case 4:
        result = i / j;
        System.out.println("division ="+result);
        
        break;

      // operator doesn't match any case constant (+, -, *, /)
      default:
        break; 
    }
    ch1++;
    } 
  }
 }
}
