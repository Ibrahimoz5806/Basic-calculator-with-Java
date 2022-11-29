# Basic-calculator-with-Java
It is a simple calculator made using switch case for Java entry level. 
It allows you to perform 4 operations with two variables.

--------------------------------------------------------------------------

import java.awt.*;
import java.util.Scanner;

public class hesap_makinesi {
    public static void main(String[] args) {


        // basic calculator with switch case
        // switch case ile hesap makinesi

        Scanner scanner = new Scanner(System.in);

        System.out.println("*****************************************");

        String actions = "1. addition\n" +                   // Toplama islemi
                            "2. subtraction\n" +             // Cikarma islemi
                            "3. multiplication\n" +          // Carpma islemi
                            "4. division";                   // Bolme islemi
        System.out.println(actions);
        System.out.println("*****************************************");

        System.out.print("Select action: ");
        String action = scanner.nextLine();

        double a;
        double b;

        switch (action){
            case "1":
                System.out.print("Number 1: ");
                 a = scanner.nextDouble();

                System.out.print("Number 2: ");
                b = scanner.nextDouble();

                double addition = a + b;

                System.out.print("Result: " + addition);

                break;

            case "2":
                System.out.print("Number 1: ");
                 a = scanner.nextDouble();

                System.out.print("Number 2: ");
                 b = scanner.nextDouble();

                double subtraction = a - b;

                System.out.print("Result: " + subtraction);

                break;

            case "3":
                System.out.print("Number 1: ");
                 a = scanner.nextDouble();

                System.out.print("Number 2: ");
                 b = scanner.nextDouble();

                double multiplication = a * b;

                System.out.print("Result: " + multiplication);

                break;

            case "4":
                System.out.print("Number 1: ");
                a = scanner.nextDouble();

                System.out.print("Number 2: ");
                b = scanner.nextDouble();

                double division = a / b;

                System.out.print("Result: " + division);

                break;

        }









    }
}
