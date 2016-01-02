import java.io.*;
import java.util.*;
import java.util.Scanner;
import java.lang.StringBuffer;
import java.text.DecimalFormat;

/* Sean Lachhander
 * Phone String Palindrome Conversions
 * This program will determine if an inputted phone number
 * (as a string) is a palindrome or not.
 * I will be using String, string tokenizer, string buffer, formatting and long integer
 * methods whenever possible (and will be using them as efficiently as possible)
 * */

public class Conversions
{
  public static void main(String[] args) throws IOException
  {
    String phoneNumber;
    Scanner keyboard = new Scanner(System.in);
    System.out.println("Please input a phone number.");
    phoneNumber = keyboard.nextLine();
    String First;

    First = FirstMethod(phoneNumber);
    PalindromeCheck(First);
    LastMethod(First);
  }
  
  public static String FirstMethod(String phoneNumber)
  {
    StringTokenizer numbers = new StringTokenizer(phoneNumber, "() -:;,");
    // StringTokenizer separates tokens and delimites the punctuations: () -:;, (including a blank space)

    StringBuffer buffer = new StringBuffer(numbers.nextToken()).append(numbers.nextToken()).append(numbers.nextToken());
    // Using StringBuffer to append the, "tokens" together that the tokenizer separated.
    
    // System.out.println(buffer);    // String Buffer (999 999 9999 phone number appended together)
    
    String phoneNumberTwo = buffer.toString();    // Converts phoneNumberTwo back to a String.
    // System.out.println(phoneNumberTwo);
  return phoneNumberTwo;
  }
  
  public static boolean PalindromeCheck(String First)
  {
    
    StringBuffer buffer = new StringBuffer(First);   // StringBuffer object with the argument of value of First!
    buffer.reverse();
    
    String UpdateTwo = buffer.toString();
    
    if(First.equals(UpdateTwo))    //First.equals because Strings are compared through the ".equals" not "==".
    {
      System.out.println("Your phone number is a palindrome");
    }
    else
    {
      System.out.println("Your phone number is not a palindrome");
    }
  return true;
  }
  
  public static void LastMethod(String First)
  {
    long num = Long.parseLong(First);
    DecimalFormat decimal = new DecimalFormat("0,000,000,000.");    // Decimal Format formats how the number will be displayed.
    System.out.println(decimal.format(num));
  }
}
