# Ucak-Bileti

        import java.util.Scanner;
    public class ucak {
    public static void main(String[] args) {

        int km, age, yolculukTipi;
        double perKm = 0.10, total;


        Scanner input = new Scanner(System.in);

        System.out.print(" mesafeyi km cinsinden giriniz ");
        km = input.nextInt();

        System.out.println("Yaşınınız Giriniz");
        age = input.nextInt();

        System.out.println("Yolculuk tipi (1=> Tek Yön, 2=>Gidiş-Dönüş):");
        yolculukTipi = input.nextInt();


        total = perKm * km;

        if ((age<0 || age>120) || km>4000 || yolculukTipi !=1  ||   yolculukTipi!=2 ){
            System.out.println("Hatalı Giriş Yaptınız");
        }

    else if (age < 12 && yolculukTipi == 1) {
            System.out.println("Ücretiniz: " + total / 2);
        } else if (age < 12 && yolculukTipi == 2) {
            System.out.println("Ücretiniz: " + total * 0.8);
        } else if (age > 65 && yolculukTipi == 1) {
            System.out.println("Ücretiniz: " + total * 0.7);
        } else if (age > 65 && yolculukTipi == 2) {
            System.out.println("Ücretiniz: " + total * 0.8);
        } else if ((age > 12 && age < 24) && yolculukTipi == 1)
            System.out.println("Ücretiniz: " + total * 0.9);
        else if ((age > 12 && age < 24) && yolculukTipi == 2) {
            System.out.println("Ücretiniz: " + total * 0.8);
        } else if ((age > 24 && age < 65) && yolculukTipi == 1) {
            System.out.println("Ücretiniz: " + total );
        }
        else if ((age > 24 && age < 65) && yolculukTipi == 2)
            System.out.println("Ücretiniz: " + total * 0.8);
         }

        }






