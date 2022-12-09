# sinifagecme
import java.util.Scanner;
public class Main {

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        int math,phy,tr,chm,mus;

        System.out.print(" Matematik notunuzu giriniz: ");
        math = input.nextInt();
        if(math<=0 || math>=100){
            System.out.println("Geçersiz not girdiniz, tekrar deneyin.");
            return;
        }
        System.out.print(" Fizik notunuzu giriniz: ");
        phy = input.nextInt();
        if(phy<=0 || phy>=100){
            System.out.println("Geçersiz not girdiniz, tekrar deneyin.");
            return;
        }
        System.out.print(" Türkçe notunuzu giriniz: ");
        tr = input.nextInt();
        if(tr<=0 || tr>=100){
            System.out.println("Geçersiz not girdiniz, tekrar deneyin.");
            return;
        }
        System.out.print(" Kimya notunuzu giriniz: ");
        chm = input.nextInt();
        if(chm<=0 || chm>=100){
            System.out.println("Geçersiz not girdiniz, tekrar deneyin.");
            return;
        }
        System.out.print(" Müzik notunuzu giriniz:");
        mus = input.nextInt();
        if(mus<=0 || mus>=100){
            System.out.println("Geçersiz not girdiniz, tekrar deneyin.");
            return;
        }
        double avarage = (math+phy+tr+chm+mus)/5;
        if(avarage>54){
            System.out.println("Tebrikler geçtiniz.");
        }
        else if(avarage <0 && avarage >100){
            System.out.println("Tanımsız not girdiniz");
        }
        else{
            System.out.println("Kaldınız.");
        }
    }
}
