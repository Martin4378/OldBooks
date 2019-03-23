# OldBooks

import java.util.Scanner;

public class P53_OldBooks {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String favoriteBook = scanner.nextLine();
        int capacity = Integer.parseInt(scanner.nextLine());
        int count = 0;

        while (count < capacity){
            String currentBook = scanner.nextLine();
            if(currentBook.equals(favoriteBook)){
                System.out.printf("You checked %d books and found it.", count);
                return;
            }
            count++;
        }
        System.out.println("The book you search is not here!");
        System.out.printf("You checked %d books.", count);
    }
}
