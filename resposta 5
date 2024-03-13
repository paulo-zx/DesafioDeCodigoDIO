import java.util.Scanner;

// Antiga classe de conversão que só suporta a conversão de USD para GBP
class OldCurrencyConverter {
    public double convertUSDtoGBP(double amount) {
        return amount * 0.80; // 80% do valor em USD
    }
}

// Novo adaptador que usa a antiga conversão e aplica a taxa adicional de GBP para EUR
class CurrencyAdapter {
    private final OldCurrencyConverter oldConverter;

    public CurrencyAdapter(OldCurrencyConverter oldConverter) {
        this.oldConverter = oldConverter;
    }

    // Método de conversão de USD para EUR usando a conversão intermediária de USD para GBP
    public double convertUSDtoEUR(double amount) {
        // Convertendo USD para GBP
        double gbpAmount = oldConverter.convertUSDtoGBP(amount);
        // Convertendo GBP para EUR
        return gbpAmount * 1.0625; // 1 GBP = 1.0625 EUR
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        double input = Double.parseDouble(scanner.nextLine());

        OldCurrencyConverter oldConverter = new OldCurrencyConverter();
        CurrencyAdapter adapter = new CurrencyAdapter(oldConverter);

        // Chamando o método para converter USD para EUR
        double convertedAmount = adapter.convertUSDtoEUR(input);

        // Imprimindo o resultado da conversão
        System.out.println("USD: " + input);
        System.out.println("EUR: " + convertedAmount);
    }
}
       
