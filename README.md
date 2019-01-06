# Ex_1.5
Daily Profit


import java.text.DecimalFormat;
import java.util.Scanner;

public class Ex1_5 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int monthWorkDays = Integer.parseInt(sc.nextLine());
        double dailySalary = Double.parseDouble(sc.nextLine());
        double dollarToBgn = Double.parseDouble(sc.nextLine());

        double yearMoney = (monthWorkDays * dailySalary * (12 + 2.5)) * 0.75 * dollarToBgn;
        double average = yearMoney / 365;

        DecimalFormat format = new DecimalFormat("#.##");
        System.out.println(format.format(average));
    }
}
