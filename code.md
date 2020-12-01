public class Main {
    public static void main(String[] args) {
        long balance = 200; // остаток на счете
        long Limit = 1000; // лимит пополнения, для начисления бонуса
        long transfer = 1900; //сумма пополнения

        if ( transfer > Limit) {
            long bonus = transfer + (transfer / 100) + balance; // где 100 стоимость 1 балла
            System.out.println("Платеж принят. Баланс, с учетом бонусных баллов: " + bonus);

        } else {
            long bonusno = transfer + balance;
            System.out.println("Платеж принят. Баланс: " + bonusno);
        }
    }
}