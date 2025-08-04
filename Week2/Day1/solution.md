# (RECURSICE FUNNCTIION) --

# Solution --1

public class Main {
    static int sum(int n) {
        if (n == 1)
            return 1;
        return n + sum(n - 1);
    }

    public static void main(String[] args) {
        System.out.println(sum(5));
    }
}


# Output -- 15

#Solution --2

public class Main {
    static int mystery(int a, int b) {
        if (b == 0)
            return 0;
        return a + mystery(a, b - 1);
    }

    public static void main(String[] args) {
        System.out.println(mystery(3, 4));
    }
}

Output -- 12

#Solution --3

public class Main {
    static int f(int n) {
        if (n == 0)
            return 0;
        else
            return n + f(n - 2);
    }

    public static void main(String[] args) {
        System.out.println(f(6));
    }
}

# Output -- 12

#Solution --4

public class Main {
    static void fun(int x) {
        if (x == 0)
            return;
        fun(x - 1);
        System.out.println(x);
    }

    public static void main(String[] args) {
        fun(3);
    }
}

Output -- 1,2,3

#Solution --5

public class Main {
    static int fact(int n) {
        if (n == 0)
            return 1;
        return n * fact(n - 1);
    }

    public static void main(String[] args) {
        System.out.println(fact(4));
    }
}

# Output -- 24

#Solution --6

public class Main {
    static int fib(int n) {
        if (n == 0)
            return 0;
        else if (n == 1)
            return 1;
        return fib(n - 1) + fib(n - 2);
    }

    public static void main(String[] args) {
        System.out.println(fib(6));
    }
}

# Output -- 8  (0, 1, 1, 2, 3, 5, 8)

#Solution --7

public class Main {
    static int fun(int n) {
        if (n <= 1)
            return n;
        return fun(n - 1) + fun(n - 3);
    }

    public static void main(String[] args) {
        System.out.println(fun(5));
    }
}

# Output -- 16

#Solution --8

public class Main {
    static int count = 0;

    static void fun(int n) {
        count++;
        if (n == 0)
            return;
        fun(n - 1);
        fun(n - 1);
    }

    public static void main(String[] args) {
        fun(3);
        System.out.println("Total recursive calls: " + count);
    }
}

Output --15

#Solution --9

public class Main {
    static int sumDigits(int n) {
        if (n == 0)
            return 0;
        return (n % 10) + sumDigits(n / 10);
    }

    public static void main(String[] args) {
        System.out.println(sumDigits(1234));
    }
}

Output --10

#Solution --10

public class Main {
    static void reversePrint(int n) {
        if (n == 0)
            return;
        System.out.println(n);
        reversePrint(n - 1);
    }

    public static void main(String[] args) {
        reversePrint(3);
    }
}

Output --3,2,1
