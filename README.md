# perfectNumber
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int n;
        int total = 0;
        System.out.println("bir sayi giriniz : ");
        Scanner input = new Scanner(System.in);
        n = input.nextInt();
        for (int i = 1; i < n; i++) {
            if (n % i == 0) {
                total = total + i;
            }
        }
        if (total == n) {
            System.out.println(n + " mukemmel sayidir.");
        } else {
            System.out.println(n + " mukemmel sayidir Degildir.");
        }
    }
}
