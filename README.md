Задача с заказом на салат Цезарь

import java.util.Scanner; 

class Main {
  public static void main(String[] args) {

    Scanner in = new Scanner(System.in);

    final float CEZAR = 73.50f;
    int quantity;

    System.out.print("Введите количество салата Цезарь по стоимости 73.50 MDL:  " );
    quantity = in.nextInt();

    System.out.println();
    float sum = quantity * CEZAR;

    System.out.println("Вы заказали " + quantity + " салатов");

    System.out.println();
    System.out.println("Сумма заказа " + sum);
    
    System.out.println();
    if(sum >= 300 && sum <= 1000){
      System.out.print("При заказе от 300 леев доставка бесплатная ");
    } else if(sum >= 1000){
      System.out.print("При заказе от 1000 леев Вы выигрываете скидочную карточку");
    } else{
      System.out.print("Cтоимость доставки +50 лей ");
    }

  }
}
