# lab-2
import java.util.Scanner;

public class YearToMonthDaysConverter {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the number of years: ");
        float years = scanner.nextFloat();

        // Assuming an average year has 365.25 days to account for leap years
        float days = years * 365.25f;

        int months = (int) (days / 30);  // Assuming an average month has 30 days

        System.out.println(years + " years is approximately " + months + " months and " + (days % 30) + " days.");

        scanner.close();
    }
}

