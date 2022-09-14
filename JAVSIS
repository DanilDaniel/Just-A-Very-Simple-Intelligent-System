package bot;

import java.time.LocalDate;
import java.time.format.DateTimeFormatter;
import java.util.Scanner;

public class SimpleBot {
    final static Scanner scanner = new Scanner(System.in);
    public static void main(String[] args) {
        greet("J.A.V.S.I.S.", "2022");
        remindName();
        guessAge();
        count();
        test();
        //end();
    }

    static void greet(String assistantName, String birthYear) {
        System.out.println("Hello! My name is " + assistantName + ".");
        System.out.println("I was created in " + birthYear + ".");
        System.out.println("Please, remind me your name.");
    }

    static void remindName() {
        String name = scanner.nextLine();
        System.out.println("What a great name you have, " + name + "!");
    }

    static void guessAge() {
        System.out.println("Let me guess your age.");
        System.out.println("Enter remainders of dividing your age by 3, 5 and 7.");
        int rem3 = scanner.nextInt();
        int rem5 = scanner.nextInt();
        int rem7 = scanner.nextInt();
        int age = (rem3 * 70 + rem5 * 21 + rem7 * 15) % 105;
        System.out.println("Your age is " + age + "; that's a good time to start programming!");
    }

    static void count() {
        System.out.println("Now I will prove to you that I can count to any number you want.");
        int num = scanner.nextInt();
        for (int i = 0; i <= num; i++) {
            System.out.printf("%d!\n", i);
        }

    }

    static void test() {
        System.out.println("Let's test your Java knowledge.)))");
        System.out.println("What is Java release first version?");
        System.out.println("1. 1990");
        System.out.println("2. 1995");
        System.out.println("3. 1996");
        System.out.println("4. 1998");
        int answerYear = scanner.nextInt();
        if (answerYear == 3){
            end();
        } else {
            System.out.println("Please, try again.");
            test();
        }
        System.out.println("Do you know, what is the date today?");
        DateTimeFormatter dtf = DateTimeFormatter.ofPattern("uuuu/MM/dd");
        LocalDate localDate = LocalDate.now();
        System.out.println("Today is " + dtf.format(localDate));

    }

    static void end() {
        System.out.println("Congratulations, have a nice day!");
    }
}
