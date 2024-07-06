# Solution (No peeking!)


<details> <summary> 👀 Answer  </summary>

```java

import java.util.ArrayList;
import java.util.HashMap;
import java.util.List;
import java.util.Map;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        List<String> studentNames = new ArrayList<String>();
        Map<String, Integer> studentGrades = new HashMap<String, Integer>();

        while (true) {
            System.out.print("Enter student name or 'exit' to see everything: ");
            String name = scanner.nextLine();

            if (name.equalsIgnoreCase("exit")) {
                break;
            }

            System.out.print("Enter grade percent for " + name + ": ");
            int grade = scanner.nextInt();
            scanner.nextLine();
            studentNames.add(name);
            studentGrades.put(name, grade);
        }

        System.out.println("\nStudent Names: " + studentNames);
        System.out.println("Student Grades: " + studentGrades);
        System.out.println("\nDetailed Student Grades:");
        for (String name : studentNames) {
            System.out.println(name + ": " + studentGrades.get(name));
        }

        scanner.close();
    }
}

```






</details>