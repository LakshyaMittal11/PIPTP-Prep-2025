Solution:1
import java.util.*;
public class Main {
    public static void main(String[] args) {
        fun(40, 4);
    }
    static void fun(int w, int x) {
        int y = 0;
        if (x % w == 0 || w % x == 0) {
            y = y + 1;
        } else {
            y = y + 10;
        }
        System.out.println(y);
    }
}

(Approach):
Inputs:
w = 40
x = 4
Initialize:
y = 0
x mod w → 4 mod 40 → 4
w mod x → 40 mod 4 → 0
 condition: 4 == 0 || 0 == 0 → false || true → true
condition is true, y = y + 1 → y = 0 + 1 = 1
Output = 1
