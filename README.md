import java.util.Scanner;

public class Taksimetre {

    public static void main(String[] args){

        Scanner yol = new Scanner(System.in);

        double KMyol;
        int KMBaslangicFiyati = 10;
        double KMBirim = 2.2;
        double tutar;

        System.out.println("Kaç KM Yol Gideceksiniz");
        KMyol = yol.nextDouble();

        tutar = (KMyol*KMBirim) + KMBaslangicFiyati;

        if (tutar <= 20) {
            tutar = 20;
            System.out.println("Taksi Ücreti : " + tutar + "TL dir");
        } else {

            System.out.println("Taksi Ücreti : " + tutar +"TL dir");
        }
