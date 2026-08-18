import java.util.Scanner;

public class ExpenseTracker {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of expenses: ");
        int n = sc.nextInt();

        double total = 0;

        for (int i = 1; i <= n; i++) {
            System.out.print("Enter expense " + i + ": ₹");
            double expense = sc.nextDouble();

            total += expense;
        }

        System.out.println("\nTotal Expenses: ₹" + total);

        sc.close();
    }
}
Enter number of expenses: 3
Enter expense 1: ₹100
Enter expense 2: ₹250
Enter expense 3: ₹150

Total Expenses: ₹500.0