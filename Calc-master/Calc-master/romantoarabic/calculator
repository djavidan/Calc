package Calc-master/romantoarabic;
import java.io.IOException;
import java.io.InputStreamReader;
import java.util.NoSuchElementException;
import java.util.Scanner;

public class RomCalc {
   

    
    public static void calculate(String leftNumber, String operation, String rightNumber) {
        
        boolean numValid = true;
        boolean opValid = true;
        int leftInt, rightInt;
        int left, right;
        int resultInt = 0;
        int resInt = 0;
        leftInt = RomanNumerals.parse(leftNumber.toUpperCase());
        rightInt = RomanNumerals.parse(rightNumber.toUpperCase());
          
        left = converterroman.parseDecimalNumber(leftNumber.toUpperCase());
        right = converterroman.parseDecimalNumber(rightNumber.toUpperCase());
      
     

        if (operation.equals("+") || operation.equals("-") || operation.equals("*") ||
                operation.equals("/")) {
            opValid = true;
        } else {
            opValid = false;
            System.out.println("invalid operation");

        }
          
      if(operation.equals("+")){
                resInt=left+right;
            }
           else if(operation.equals("*")){
                resInt=left*right;
            }
        else if(operation.equals("/")){
            resInt=left/right;
        }
        else if(operation.equals("-")){
            resInt=left-right;
        }
        if (numValid == true && opValid == true) {

            
            if (operation.equals("+")) {
                resultInt = leftInt + rightInt;
            }
            else if (operation.equals("-")) {
                resultInt = leftInt - rightInt;
            }
            else if (operation.equals("*")) {
                resultInt = leftInt * rightInt;
            }

             
            else if (operation.equals("/")) {
                resultInt = leftInt / rightInt;
            }
      if(left <= 0  || left >= 10 || right <= 0 || right >= 10){
                    System.out.print("");
                }
                else{
                    System.out.print(resInt);
                }
    if(opValid && numValid) {

               
                if (leftInt <= 0 || leftInt >= 10 || rightInt <= 0 || rightInt >= 10 ) {
                    System.out.println("result out of range");
                } else {
                    System.out.println(RomanNumerals.format(resultInt));
                }
            }
if(resInt==resultInt){
System.err.print("Erorr");
System.exit(0);
}
 
    }

    
    public static void main(String[] args) throws IOException {
      
        final BufferedReader reader = new BufferedReader(new InputStreamReader(System.in));
        
        while (true) {
           
            System.out.print("Введите число: ");
            int number1, number2;
            final String line = reader.readLine();
            if (line.length() == 0) {
                System.out.println("done");
                break;
            }
           
            Scanner scan=new Scanner(System.in);
            System.out.print("Результат: ");
            final Scanner scanner = new Scanner(line);
            final String leftNumber, operation, rightNumber;
           System.out.println();
            try {
                leftNumber = scanner.next();
                operation = scanner.next();
                rightNumber = scanner.next();
               
             }
 
            catch (NumberFormatException e) {
               
                System.out.println();
                continue;
            }
            
            calculate(leftNumber, operation, rightNumber);

        }
    }


}
            
