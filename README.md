# -O-Impacto-da-tecnologia-no-aprendizado-dos-estudantes
Projeto de extensão
import java.util.Scanner;
public class QuestionarioApp {
public static void main(String[] args) {
Scanner scanner = new Scanner(System.in);
String idade;
String usaTecnologia;
int horasEstudo;
// Boas-vindas e coleta de informações do estudante
System.out.println("Este é um Questionário de Estudo e Tecnologia");
System.out.print("Por favor, insira sua idade: ");
idade = scanner.nextInt();
scanner.nextLine(); // Consumir a nova linha deixada pelo nextInt()
// Perguntas sobre o uso de tecnologia
System.out.println("\nUso de Tecnologia:");
System.out.print("Você usa tecnologia para seus estudos? (Sim/Não): ");
usaTecnologia = scanner.nextLine();
System.out.print("O uso da tecnologia atrapalha seus estudos?: ");
horasEstudo = scanner.nextInt();
// Exibe o resumo das respostas do estudante
System.out.println("\nResumo das Respostas:");
System.out.println("Idade: " + idade);
System.out.println("Usa Tecnologia para os Estudos: " + usaTecnologia);
System.out.println("Horas de Estudo por Dia: " + horasEstudo);
// Exemplo de feedback com base nas respostas
if (usaTecnologia.equalsIgnoreCase("Sim")) {
System.out.println("Que ótimo! A tecnologia pode ser uma ótima aliada nos estudos.");
} else {
System.out.println("Sem problemas! Métodos tradicionais de estudo também são
eficazes.");
}if (horasEstudo < 2) {
System.out.println("Tente dedicar mais tempo aos estudos para melhorar seu
desempenho.");
} else if (horasEstudo <= 5) {
System.out.println("Você tem uma boa rotina de estudos!");
} else {
System.out.println("Parabéns pela dedicação aos estudos!");
}
scanner.close();
