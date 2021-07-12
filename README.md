# Body-Mass-Indeks-BMI-
package bmi;
import java.util.Scanner;
public class BMI {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("KALKULATOR BMI (BODY MASS INDEKS)");
        System.out.print("Input Massa (kg): ");
        float m =sc.nextFloat();
        System.out.print("Input Tinggi Badan (cm): ");
        float t= sc.nextFloat();
        t /= 100;
        float bmi = m / t / t;
        if (bmi < 18.5) {
            System.out.printf("BMI= %.2f%s%n ", bmi, "(Kurus)");
        } else if (bmi >= 18.5 && bmi < 25) {
            System.out.printf("BMI= %.2f%s%n ", bmi, "(Normal)");
        } else if (bmi >= 25 && bmi < 30) {
            System.out.printf("BMI= %.2f%s%n ", bmi, "(Gemuk)");
        } else {
            System.out.printf("BMI= %.2f%s%n ", bmi, "(Obesitas)");
        }
    }
}
