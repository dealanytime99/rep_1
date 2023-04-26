public class GCD {
    public static void main(String[] args) {
        int num1 = 48, num2 = 60;
        int gcd = findGCD(num1, num2);
        System.out.printf("GCD of %d and %d is %d", num1, num2, gcd);
    }

    private static int findGCD(int num1, int num2) {
        if (num2 == 0) {
            return num1;
        } else {
            return findGCD(num2, num1 % num2);
        }
    }
}
