# Calculator
www.patika.dev Basit hesap makinesi yapımı




        import java.util.Scanner;
        public class switchase {
        public static void main(String[] args) {
        Double n1,n2,sonuc;
        int select;
        System.out.println("Lutfen birinci sayiyi giriniz:");
        Scanner nn1=new Scanner(System.in);
        n1=nn1.nextDouble();
        System.out.println("Lutfen ikinci sayiyi giriniz:");
        Scanner nn2=new Scanner(System.in);
        n2=nn2.nextDouble();
        System.out.println("Lutfen islem seciniz: \n1-Toplama\n2-Cikarma\n3-Carpma\n4-Bolme");
        Scanner select1=new Scanner(System.in);
        select=select1.nextInt();
        System.out.println("Seciminiz: "+ select);
        switch (select){
            case 1:
                sonuc=n1+n2;
                System.out.println("islem sonucu:"+sonuc);
                break;
            case 2:
                sonuc=n1-n2;
                System.out.println("islem sonucu:"+sonuc);
                break;
            case 3:
                sonuc=n1*n2;
                System.out.println("islem sonucu:"+sonuc);
                break;
            case 4:
                if(n2 != 0){
                    sonuc=n1/n2;
                    System.out.println("islem sonucu:"+sonuc);
                }
                else {
                    System.out.println("Bir sayi sifira bolunmez!!");
                }
                break;
            default: System.out.println("Hatali islem yaptiniz tekrar deneyin!");
        }

    }
}
