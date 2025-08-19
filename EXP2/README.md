JAVA PROGRAM TO FIND THE LARGEST ELEMENT IN AN ARRAY
AIM:
To find the largest element in an array using Java programming language.

APPARATUS REQUIRED:
Computer


Eclipse IDE



THEORY:
Java is a high-level, class-based, object-oriented programming language that is designed to have as few implementation dependencies as possible. It is a general-purpose programming language intended to let programmers write once, run anywhere (WORA), meaning that compiled Java code can run on all platforms that support Java without the need to recompile.
Java applications are typically compiled to bytecode that can run on any Java Virtual Machine (JVM) regardless of the underlying computer architecture. The syntax of Java is similar to C and C++, but it has fewer low-level facilities than either of them.
The Java runtime provides dynamic capabilities (such as reflection and runtime code modification) that are typically not available in traditional compiled languages. As of 2019, Java was one of the most popular programming languages in use according to GitHub, particularly for client–server web applications, with a reported 9 million developers.

PROCEDURE:
Launch Eclipse IDE


Open Eclipse.


Select a workspace (folder for saving your projects).


Create a New Project


Click File > New > Java Project.


Enter the project name (e.g., EXP2).


Click Finish.


Create a New Class


Right-click on your package → New > Class.


Enter the class name (e.g., LargestElement).


Check public static void main(String[] args).


Click Finish.


Write Your Program


Eclipse opens the code editor automatically.


Type or paste your source code.


Save the Program


Press Ctrl + S or click File > Save.


Compile and Run the Program


Click the Run button (green ▶) on the toolbar.


View the output in the Console window.


Close Eclipse


PROGRAM:

package arrayprograms;
import java.util.Scanner;
public class LargestElement {
   public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       // Input array size
       System.out.print("Enter the number of elements: ");
       int n = sc.nextInt();
       int[] arr = new int[n];
       // Input array elements
       System.out.println("Enter " + n + " numbers:");
       for (int i = 0; i < n; i++) {
           arr[i] = sc.nextInt();
       }
       // Assume first element is the largest
       int largest = arr[0];
       // Compare with other elements
       for (int i = 1; i < n; i++) {
           if (arr[i] > largest) {
               largest = arr[i];
           }
       }
       // Output the result
       System.out.println("The largest element is: " + largest);
       sc.close();
   }
}


OUTPUT:

## OUTPUT

![Program Output Screenshot]([output_screenshot.png](https://raw.githubusercontent.com/DHRUV-D-MEHTA/Object-Oriented-Programming-for-Embedded-Applications-19CS304-4Y3-2/706a5966d091cec6451a10378af12ed8f3207752/EXP2/Screenshot%202025-08-19%20085158.png))

RESULT:
Thus, the largest element in an array using java program is developed, and the output is verified.


After finishing, click File > Exit to close Eclipse IDE.

