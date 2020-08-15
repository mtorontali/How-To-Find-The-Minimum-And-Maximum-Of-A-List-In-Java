# How To Find The Minimum And Maximum Values Of A List In Java

```java
import java.util.*;

/**
 *
 * @author Matthew Torontali
 */
public class MinMaxList {

    public static void main(String[] args) {
        
        // try catch statement to trap errors
        try {
            output();
        }
        catch (Exception e) {
            System.out.println("Exception occured");
            
        }
    }
    
    public static void output() {
        
        // initialize character arraylist
        List<Character> list = new ArrayList<Character>();

        // add characters to arraylist
        list.add('P');
        list.add('C');
        list.add('M');

        // print arraylist
        System.out.println("List Contains: ");
        System.out.print("The list is: ");
        System.out.println(list);
        System.out.println("Max: " + Collections.max(list) + " Min: " + Collections.min(list) + "\n");
        
        // reverse list
        Collections.reverse(list);
            
        System.out.println("After calling reverse, list contains: ");
        System.out.print("The list is: ");
        System.out.println(list);
        System.out.println("Max: " + Collections.max(list) + " Min: " + Collections.min(list) + "\n");
        
        // copy list into new list
        List<Character> copyList = new ArrayList<Character>(list);
            
        System.out.println("After copying, copyList contains: ");
        System.out.print("The list is: ");
        System.out.println(copyList);
        System.out.println("Max: " + Collections.max(copyList) + " Min: " + Collections.min(copyList) + "\n");
        
        // fill list with R
        Collections.fill(list, 'R');
            
        System.out.println("After calling fill, list contains: ");
        System.out.print("The list is: ");
        System.out.println(list);
        System.out.println("Max: " + Collections.max(list) + " Min: " + Collections.min(list) + "\n");
    }
    
}
```
