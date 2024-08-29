import java.util.Scanner;
public class SimpleCa{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter the first number:");
        int firstNumber =sc .nextInt();
        System.out.print("Enter the second number:");
        int secondNumber =sc .nextInt();
        System.out.print("Enter the tpe of operation you want to perform(+,-,*,/,%):");
        String operation = sc.next();
        int result = performOperation(firstNumber, secondNumber, operation);
        System.out.print("Your answer is:" + result);
    }

    public static int performOperation(int firstNumber, int secondNumber, String operation )
    {
        int result = 0;
        if(operation.equals("+")){
            result = firstNumber + secondNumber;
        }
        else if(operation.equals("-")){
            result = firstNumber - secondNumber;
        }
        else if(operation.equals("*")){
            result = firstNumber * secondNumber;
        }
        else if(operation.equals("/")){
            result = firstNumber / secondNumber;
        }
        else if(operation.equals("%")){
            result = firstNumber % secondNumber;
        }
        else {
            System.out.println("Invalid operation");
        }
        return result;
    }
}
