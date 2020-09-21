package com.company;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        int height;
        do{
            System.out.println("Enter the height of the pyramid");
            height = input.nextInt();
        }while(height <1 || height >8);

        int i,j,k;

        for(i=0; i<height; i++){
            for(j=0; j< (height-i-1); j++){
                System.out.print(" ");
            }
            for(k=0; k<=i; k++){
                System.out.print("#");
            }
            System.out.print("  ");
            for(k=0; k<=i; k++){
                System.out.print("#");
            }
            System.out.println();
        }
    }
}
