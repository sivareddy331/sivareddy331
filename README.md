1) reversse a word 
public class WordReverser {
    public static void main(String[] args) {
        String word = "akhil";
        String reversedWord = reverseWord(word);
        System.out.println("Reversed word: " + reversedWord);
    }

    public static String reverseWord(String word) {
        String reversedWord = "";
        for (int i = word.length() - 1; i >= 0; i--) {
            reversedWord += word.charAt(i);
        }
        return reversedWord;
    }
}
                              input:akhil
                              output:lihka
2) string to integer
public class StringToInteger {
    public static void main(String[] args) {
        String str = "12345";
        int num = Integer.parseInt(str);                                        INPUT:12345
        System.out.println("Converted Integer: " + num);                        OUTPUT:12345    
    }}



3)  vowels
public class VowelCounter {
    public static void main(String[] args) {
        String statement = "This is a sample statement to count vowels.";
        int vowelsCount = countVowels(statement);
        System.out.println("Number of vowels in the statement: " + vowelsCount);
    }
    public static int countVowels(String str) {
        int count = 0;
        for (int i = 0; i < str.length(); i++) {
            char ch = Character.toLowerCase(str.charAt(i));
            if (ch == 'a'||ch=='e'||ch=='i'||ch=='o'||ch =='u'){
                count++;
            }}
        return count;
    }}


4) factorial
public class Factorial {
    public static void main(String[] args) {
        int num = 5;
        int factorial = 1;
        for(int i = 1; i <= num; i++) {
            factorial *= i;
        }
        System.out.println("Factorial of " + num + " is " + factorial);
    }}



6) multiplication
public class Multiplication {
    public static void main(String[] args) {
        int num1 = 5;
        int num2 = 10;

        int result = num1 * num2;

        System.out.println("Multiplication Result: " + result);
    }
}


7) validity checker
public class CharacterNumberSeparator {
    public static void main(String[] args) {
        String input = "Hello123World456";
        String characters = input.replaceAll("[^a-zA-Z]", "");
        String numbers = input.replaceAll("[^0-9]", "");
        System.out.println("Characters: " + characters);                      input : santhosh11435
        System.out.println("Numbers: " + numbers);                            output :santhosh
    }                                                                                :11435
}


8) special characters
import java.util.regex.Matcher;
import java.util.regex.Pattern;
public class SpecialCharactersCounter {
    public static void main(String[] args) {
        String line = "Hello! How are you? 123 #$%^&*";
        Pattern pattern = Pattern.compile("[^a-zA-Z0-9\\s]");
        Matcher matcher = pattern.matcher(line);
        int count = 0;
        System.out.println("Special Characters in the Line:");
        while (matcher.find()) {
            System.out.println(matcher.group());
            count++;
        }
        System.out.println("Number of Special Characters: " + count);
    }}
9) ALPHABETICALLY REVERSE
  import java.util.ArrayList;
import java.util.Collections;
import java.util.Comparator;
import java.util.List;

public class ReverseAlphabetical {
    public static void main(String[] args) {
        List<String> fruits = new ArrayList<>();
        fruits.add("Apple");
        fruits.add("Banana");
        fruits.add("Orange");
        fruits.add("Pineapple");
        fruits.add("Grapes");
        Collections.sort(fruits, new Comparator<String>() {
            @Override
            public int compare(String o1, String o2) {
                return o2.compareTo(o1);
            }
        });
        System.out.println("Fruits sorted in reverse alphabetical order:");
        for (String fruit : fruits) {
            System.out.println(fruit);
        }
    }
}

10) HALLOW SQUARE PATTERN
  public class HollowSquarePattern {
    public static void main(String[] args) {
        int rows = 5; 
        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= rows; j++) {
                if (i == 1 || i == rows || j == 1 || j == rows) {
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }
    }
}
