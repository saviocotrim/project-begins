# project-begins
import java.time.LocalDate;
import java.util.Date;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int dia, mes, ano;  ;
        int idade;

        LocalDate currentDate = LocalDate.now();
        int day = currentDate.getDayOfMonth();
        int month = currentDate.getMonthValue();
        int Year = currentDate.getYear();


        System.out.println(currentDate);
        System.out.println(currentDate.getMonthValue());
        System.out.println(currentDate.getDayOfMonth());
        System.out.println(currentDate.getYear());
        System.out.println("somente numeros fdp!!");
        System.out.println("Em que dia voce nasceu? ");
        dia = scanner.nextInt();
        System.out.println("Em que mes voce nasceu?");
        mes = scanner.nextInt();

        System.out.println("Em que ano voce nasceu?");
        ano = scanner.nextInt();



         idade= Year - ano;
        if (mes>month||(mes == month & dia>day)){idade--;}
        else if (mes==month & dia ==day) {
        }
        else {
        }

        System.out.println(idade);

        scanner.close();
    }
}
