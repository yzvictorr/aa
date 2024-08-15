import java.util.Scanner;

public class IdadeEmDias {
    
    public static void main(String[] args) {
        // Criar um objeto Scanner para leitura de dados do usuário
        Scanner scanner = new Scanner(System.in);
        
        // Solicitar ao usuário a idade em anos, meses e dias
        System.out.print("Digite a idade em anos: ");
        int anos = scanner.nextInt();
        
        System.out.print("Digite a idade em meses: ");
        int meses = scanner.nextInt();
        
        System.out.print("Digite a idade em dias: ");
        int dias = scanner.nextInt();
        
        // Calcular a idade em dias
        int diasTotais = calcularDiasTotais(anos, meses, dias);
        
        // Exibir o resultado
        System.out.println("A idade em dias é: " + diasTotais);
        
        // Fechar o scanner
        scanner.close();
    }
    
    // Função para calcular a idade total em dias
    public static int calcularDiasTotais(int anos, int meses, int dias) {
        // Considerar 365 dias por ano e 30 dias por mês
        return (anos * 365) + (meses * 30) + dias;
    }
}
