# RefactorMe
package refactorme;
import java.util.*;

public class RefactorMe {

    public static void main(String[] args) {
        getName();
        calculateSalary(2500, 400);
        calculateSides("circle");
        countLetters();
    }

    public static void getName(){
        Scanner I = new Scanner(System .in);
        System.out.println("WHat is your name: ");
        String name = I.nextLine();
        System.out.println("Your name is: " + name );
    }

    public static void calculateSalary(int income, int tax) {
        Scanner I = new Scanner(System.in);
        int calculateSalary = income - tax;
        System.out.println("Your salary is: " + calculateSalary);
    }

    public static void calculateSides(String shape) {
        
        Scanner I = new Scanner(System.in);
        System.out.print("Please enter your shape: ");
        shape = I.nextLine();
        shape.toLowerCase();

        if (shape.contains("square")) {
            System.out.println("Your shape has 4 sides");
        }
        if (shape.contains("circle")) {
            System.out.println("Your shape has 1 side");
        }
        if (shape.contains("hexagon")) {
            System.out.println("your shape has 6 sides");
        }
        if (shape.contains("dodecagon")) {
            System.out.println("Your shape has 12 sides");
        }
    }

    public static void countLetters() {
        Scanner I = new Scanner(System.in);
        System.out.println("Please enter a chosen word");
        String word = I.nextLine();
        System.out.println("You entered: " + word );

        System.out.println("You word is:  "  +  word.length()  +  " letters long.");
    }

}
