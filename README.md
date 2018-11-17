# tecacsInheritProject

package inheri2;
import java.util.Scanner;
class Inheri1 {
    
    int result;
    public void add(int x, int y) {
        result = x + y;
        System.out.println("Sum = " + result);
    }
    public void sub(int x, int y) {
        result = x - y;
        System.out.println("Diff = " + result);
    }
    
}

public class Inheri2 extends Inheri1 {
    public void multiply(int x, int y) {
        result = x * y;
        System.out.println("Multi = " + result);
    }
  public static void main(String[] args) {
      Scanner number1 = new Scanner(System.in);
      System.out.println("Enter 1st number: ");
      int a = number1.nextInt();
      System.out.println("Enter 2nd number: ");
      int b = number1.nextInt();
      
      Inheri2 object1 = new Inheri2();
      object1.add(a,b);
      object1.sub(a,b);
      object1.multiply(a,b);
      
  }  
}
