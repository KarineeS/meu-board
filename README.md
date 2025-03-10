import java.util.Scanner;
import java.text.DecimalFormat;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Lendo o valor em dólares
        double valorDolar = scanner.nextDouble();
        scanner.close();

        // Cotação fixa: 1 dólar = R$5,00
        double cotacao = 5.00;
        double valorReais = valorDolar * cotacao;

        // Formatando o resultado para ter duas casas decimais
        DecimalFormat df = new DecimalFormat("0.00");

        // Exibindo o resultado no formato correto
        System.out.println("Valor em reais: R$" + df.format(valorReais));
    }
}
