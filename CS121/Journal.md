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
}'

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
System.out.print is a constrcut that supports output. To output text you would type System.out.print("text");
System.out.print(x); is used to output a variable's value
Programmers often will combine outputs that must share a line for readibility in code, it is represented by a + sign in between two things to be outputted on the same line

`public class Salary {
   public static void main (String [] args) {
      int wage;

      wage = 20;

      System.out.println("Wage is: " + wage); 
      System.out.println("Goodbye."); 
   }
}`

### 1.3 Comments and whitespace

#### Definitions
**comments:** text added to code that is meant for humans and is ignored by the program.
**single-line comment:** starts with // and includes all following text on that line., usually follows a statement on that line
**multi-line comment:** starts with /* text */ and includes everything within the two slashes, used for multiple lines and is also called a
    **block comment**
**whitespace:** Whitespace refers to blank spaces (space and tab characters) between items within a statement and blank lines between statements (called newlines).      A compiler ignores most whitespace.

### 1.4 Why whitespace matters
#### Definitions


#### Observations
It is important to make sure that whitespace is correct. The system will not ignore whitespace or new lines within string literals, they will effect the output.
Precision is key when programming, every little character and line can change the output dramatically and could even cause compilation errors.

### 1.5 Errors and warnings

#### Definiitions
**syntax error:** errors that usually violate a languages allowable use of symbols (ex, in java, forgetting to end a statement with a semicolon
**compile-time error:** errors that are detected by the compiler
**logic errors:** also known as bugs, are parts of a programs that run just fine through the compiler, but still produce results that were not intetended
**warnings:** a compiler can give warnings if it finds logic errors, but will still run. However, a compiler will not always find these kinds of errors. A programmer should configure the compiler to not ignore any warning and be very picky.

#### Observations
`Traffic.java:4: ';' expected
      System.out.print("Traffic today")
                                       ^
1 error`
THe above code is a syntax error, 4 in the error says that there is an error on line 4 and shows what is missing.
SOmetimes errors point to a line that doesn't actually have a problem, but is being effecte dby something with an error and we
should actually look at previous lines to find out what's going on. SOmeimes the compiler will point an error that isn't true, but there is indeeed
an error.

Good practices:`
Focus on FIRST error message, ignoring the rest.
Look at reported line of first error message. If error found, fix. Else, look at previous few lines.
Compile, repeat.`

We should also compile manmy times, make sure to compile after a couple of lines rather than writiing a whole bunch of lines, it makes it ahrder to find the roots of problems, especially if they were made early in the program.

### 1.6 Computers and programs (general)
#### Definitions
**bits:**(binary digits) are the 0s and 1s that  computers use to do computations. 1s represent a positive voltage and 0s are zero voltage. 
    1s allow electricity to flow, 0s don't, which tell the computer how to calculate.
    
**processor:** numerous switches used in sequences to process specific calculations

**instructions:** each calculation  was called an instructions.

**memory:**a circuit that can store 0s and 1s in each of a series of thousands of addressed locations, like a series of addressed mailboxes that each can store an envelope (the 0s and 1s). Instructions operate on data, which is also stored in memory locations as 0s and 1s.

**machine instructions:** Instructions represented as 0s and 1s
**executable program:** sequence of machine instructions
**assembly language instructions:** Because 0s and 1s are hard to comprehend, programmers soon created programs called assemblers to automatically translate human readable instructions into machine language
**high-level languages** upport programming using formulas or algorithms, so a programmer could write a formula like: F = (9 / 5) * C + 32.
**compilers:** programs that automatically translate high-level language programs into executable programs.
**bytecode:**  compiler generate an executable using machine instructions of a "virtual" processor
** virtual machine:** executes the instructions in the bytecode
#### Observations



