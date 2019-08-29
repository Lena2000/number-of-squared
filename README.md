package javaapplication11;

import java.util.Scanner;

/**
 *
 * @author LENOVO
 */
public class JavaApplication11 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
        int number,kvadrat;
        int count=0;
        int b=0;
        int c=0;
       do{
        System.out.println("Input your number: ");

        number = sc.nextInt();
        kvadrat= (int)Math.pow(number,2);
           if (number!=0){
               System.out.println(kvadrat);
               count++;
           }
           if (number>0){
            b++;
           }
           if (number<0){
               c++;
           }
       }
       while (number!=0);
        System.out.println("Кол-во возведений в квадрат - "+count);
        System.out.println("Из них положительных - "+ b +" и отрицательных - "+c);
    }

}
