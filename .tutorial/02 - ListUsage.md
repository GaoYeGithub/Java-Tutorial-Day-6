# Dictionaries

You can also do stuff to the List like removing strings

```java
import java.util.ArrayList;
import java.util.List;

public class Main {
    public static void main(String[] args) {

      List<String> names = new ArrayList<String>();

        names.add("Gary");
        names.add("Bob");
        names.add("Joe");

        System.out.println("Names: " + names);
        // Remove an string from the list
        names.remove("Bob");
        System.out.println("Names after removal: " + names);

        // You can also pretty print all the names with out [] or commas
        System.out.println("Iterating through the list:");
        for (String name : names) {
            System.out.println(name);
        }
    }
}
```

Try Creating a interger list by yourself! Use Integer instead of int tho

<details> <summary> 👀 Answer  </summary>

```java
import java.util.ArrayList;
import java.util.List;

public class Main {
    public static void main(String[] args) {

      List<Integer> nums = new ArrayList<Integer>();

        nums.add(1);
        nums.add(2);
        nums.add(3);

        System.out.println("Numbers " + nums);
        }
    }
}
```
</details>