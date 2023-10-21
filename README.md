# string-reverse-assignment
# Java program to reverse a string
public class StringReverse {
    public String reverse(String input) {
        StringBuilder reversed = new StringBuilder();
        for (int i = input.length() - 1; i >= 0; i--) {
            reversed.append(input.charAt(i));
        }
        return reversed.toString();
    }
}


# JUnit test class to test the reverse method

import org.junit.jupiter.api.Test;
import static org.junit.jupiter.api.Assertions.assertEquals;

public class StringReverseTest {
    @Test
    public void testReverse() {
        StringReverse reverser = new StringReverse();
        String input = "my name is vikas";
        String expectedOutput = "sakiv si eman ym";
        String actualOutput = reverser.reverse(input);
        assertEquals(expectedOutput, actualOutput);
    }
}


