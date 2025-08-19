# JAVA PROGRAM TO FIND THE LARGEST ELEMENT IN AN ARRAY

## AIM
To find the largest element in an array using Java programming language.

---

## APPARATUS REQUIRED
- Computer  
- Eclipse IDE  

---

## THEORY
Java is a high-level, class-based, object-oriented programming language that is designed to have as few implementation dependencies as possible.  
It is a general-purpose programming language intended to let programmers *write once, run anywhere (WORA)*, meaning that compiled Java code can run on all platforms that support Java without the need to recompile.

Java applications are typically compiled to bytecode that can run on any Java Virtual Machine (JVM). The syntax of Java is similar to C and C++, but it has fewer low-level facilities than either of them.  
The Java runtime provides dynamic capabilities (such as reflection and runtime code modification) that are typically not available in traditional compiled languages.  
As of 2019, Java was one of the most popular programming languages in use according to GitHub, particularly for client–server web applications, with a reported 9 million developers.

---

## PROCEDURE
1. Launch **Eclipse IDE**  
2. Open Eclipse and select a workspace (folder for saving your projects).  
3. Create a New Project → `File > New > Java Project` → enter project name (e.g., EXP2) → **Finish**.  
4. Create a New Class → Right-click on your package → `New > Class` → enter class name (e.g., LargestElement) → check `public static void main(String[] args)` → **Finish**.  
5. Write your program (Eclipse opens the code editor automatically).  
6. Save the program (`Ctrl + S`).  
7. Compile and Run → Click the **Run** button (green ▶).  
8. View the output in the Console window.  
9. Close Eclipse (`File > Exit`).  

---

## PROGRAM
```java
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


## OUTPUT

![Program Output Screenshot](Screenshot%202025-08-19%20085158.png)


RESULT:
Thus, the largest element in an array using java program is developed, and the output is verified.


After finishing, click File > Exit to close Eclipse IDE.

