# hesapMakinesi
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int secim;
        Scanner keyboard = new Scanner(System.in);
        System.out.println("birinci sayiyi gir");
        int n1= keyboard.nextInt();
        System.out.println("ikinci sayiyi gir");
        int n2= keyboard.nextInt();
        System.out.println("seçiminizi giriniz:\n\n1-Toplama\n2-Çıkarma\n3-Bölme\n4-Çarpma");
        secim = keyboard.nextInt();
        switch (secim){
            case 1:
                System.out.println(+n1 +" sayısı ile "+n2 +" sayısının toplamı "+(n1+n2));
                break;
            case 2:
                System.out.println(+n1 +" sayısı ile "+n2 +" sayısının farkı "+(n1-n2));
                break;
            case 3:
                if (n2!=0){
                    System.out.println(+n1 +" sayısı ile "+n2 +" sayısının bölümü "+(n1/n2));
                    break; }
                else {
                    System.out.println("Bir sayı 0a bölünemez.");
                    break;
                }
            case 4:
                System.out.println(+n1 +" sayısı ile "+n2 +" sayısının çarpımı "+(n1*n2));
                break;
        }
    }
}
