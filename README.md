import java.util.Scanner;

public class Main{ 

	public static void main(String[] args) {
        
	Scanner scanner = new Scanner(System.in);

        float salario;
        float inflacao = 0.038f;
        float aumento; 
        float novoSalario;
        float aumentoReal;
        
        System.out.println("digite o salario");
            salario = scanner.nextFloat();
        
        if (salario > 0 && salario < 280) {
            aumento = salario * 0.20f; 
            novoSalario = salario + aumento;
            aumentoReal = aumento - (aumento * inflacao);
            System.out.println("o salario é:" + salario);
            System.out.println("o Aumento é de 20%");
            System.out.println("o valor aumentado é " + aumento);
            System.out.println("o novo salario é: " + novoSalario);
            System.out.println("o valor aumentado Real descontando inflacao é: " + aumentoReal);
            
        }
        
        if (salario >= 280 && salario < 700) {
            aumento = salario * 0.15f; 
            novoSalario = salario + aumento;
            aumentoReal = aumento - (aumento * inflacao);
            System.out.println("o salario é:" + salario);
            System.out.println("o Aumento é de 15%");
            System.out.println("o valor aumentado é " + aumento);
            System.out.println("o novo salario é: " + novoSalario);
            System.out.println("o valor aumentado Real descontando inflacao é: " + aumentoReal);
            
        }
        
        if (salario >= 700 && salario < 1500) {
            aumento = salario * 0.10f; 
            novoSalario = salario + aumento;
            aumentoReal = aumento - (aumento * inflacao);
            System.out.println("o salario é:" + salario);
            System.out.println("o Aumento é de 10%");
            System.out.println("o valor aumentado é " + aumento);
            System.out.println("o novo salario é: " + novoSalario);
            System.out.println("o valor aumentado Real descontando inflacao é: " + aumentoReal);
            
        }
        if (salario >= 1500) {
            aumento = salario * 0.05f; 
            novoSalario = salario + aumento;
            aumentoReal = aumento - (aumento * inflacao);
            System.out.println("o salario é:" + salario);
            System.out.println("o Aumento é de 5%");
            System.out.println("o valor aumentado é " + aumento);
            System.out.println("o novo salario é: " + novoSalario);
            System.out.println("o valor aumentado Real descontando inflacao é: " + aumentoReal);
            
        }
    }
}
