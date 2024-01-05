# Coding Journal
## Reading Notes
### 1.1
#### Definitions
**program:** instructions executed one at a time
**input:** data inputted form a certain location (eg: file, keyboard, touchscrren, etc)
**process:** computation performed on  data (eg: adding two number x + y)
**output:** data that a program gives and is placed somewhere (eg: file, screen, network, etc)
**variable:** name that is assigned a value by user or program (eg x, y, z)
**computational thinking:** creating a sequence of instructions to solve a problem
**algorithm:** a sequence of instructions that solve a problem
#### Observations
The order of instructions matter and can drastically change the desired output (or even create an error)

### 1.2
#### Definitions
**int:** in java creates an integer variable
**print and println:** both tells computer to output given data. println will move cursor to the next line but it will output data on line before cursor is moved.
They give an output to the screen (UI)
**Scanner:** a text parser that can get numbers, words or phrases from an input source like a keyboard. 
**string literal:** anything within a double quote ("") will be printed character for character.

#### Observations
In java a program starts in main() and executes in main's {} one line at a time.
Each statement occurs on separate lines and ends with a semicolon (;)
To assign an integer to a variable, declare it as an integer using int wage, and then use the "=" sign
ex: int wage;
    wage = 20;

  public class Salary {                       

  public static void main (String [] args) {
      int wage;

      wage = 20;                        

      System.out.print("Salary is ");       
      System.out.println(wage * 40 * 52);   
  }
}

In above code, the variable wage **HOLDS** the value of 20, it is not an input.

##### Input

Getting input is achieved by first creating a Scanner object via the statement: Scanner scnr = new Scanner(System.in);. System.in corresponds to keyboard input. Then, given Scanner object scnr, the following statement gets an input value and assigns x with that value: x = scnr.nextInt() ;

" import java.util.Scanner;

public class Salary {
   public static void main(String [] args) {
      int wage;

      Scanner scnr = new Scanner(System.in);
      wage = scnr.nextInt();

      System.out.print("Salary is ");
      System.out.println(wage * 40 * 52);
   }
}"


##### Output
System.output.print is a constrcut that supports output. To output text you would type System.output.print("text");




