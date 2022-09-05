# calculatingTheAreaOfTheTriangle

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        double a,b,c,hip,dikA,alan,ucgenC,U,d,e,f;

        //1 örnek a ve b kullanıcıdan alarak dik üçgenin alanı ve hipotenüsü bulma

        //kullanıcıdan girdi almak için scanner tanımlamak

        Scanner inp = new Scanner(System.in);

        //A ve b girdilerini kullanıcıdan almak

        System.out.println("Lütfen Dik üçgenin A uzunluğunu giriniz: ");

        a= inp.nextDouble();

        //System.out.println(a);

        System.out.println("Lütfen Dik üçgenin B uzunluğunu giriniz: ");

        b= inp.nextDouble();

        dikA = (a*b)/2;

        c=Math.sqrt((a*a)+(b*b));

        System.out.println("Dik Üçgenin Alanı: "+dikA);

        System.out.println("Üçgenin Hipotenüsü: "+c);

        //2 örnek a,b,c kullanıcıdan alarak üçgenin alanı, çevresi, bulma

        //Scanner inp2 = new Scanner(System.in);

        System.out.println("Birinici kenarı giriniz:");

        d= inp.nextDouble();

        System.out.println("İkinci kenarı giriniz:");

        e= inp.nextDouble();

        System.out.println("Üçüncü kenarı giriniz:");

        f= inp.nextDouble();

        // üçgenin çevresi

        U=(d+e+f)/2;

        ucgenC=2*U;

        alan=Math.sqrt(U*(U-d)*(U-e)*(U-f));

        //ucgenA=U*(U-d)*(U-e)*(U-f);

        System.out.println("Üçgenin Çevresi: "+ucgenC);

        System.out.println("Üçgenin Alanı: "+alan);

    }
}

