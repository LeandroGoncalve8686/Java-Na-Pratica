# Java-Na-Pratica
Aprendendo Java Na Prática.

import java.util.Scanner;
class exercicio1{
  public static void main(String[] args){
    int quantidade;
    int contador = 0;
    String nome;
    int serie;
    int nota;
    
    
    Scanner quantidade_aluno = new Scanner(System.in);
    Scanner nome_aluno = new Scanner(System.in);
    Scanner serie_aluno = new Scanner(System.in);
    Scanner resultado = new Scanner(System.in);
    
    System.out.println("Digite a Quantidade de Aluno:");
     quantidade = quantidade_aluno.nextInt();

     while (contador < quantidade ) {
      System.out.println("Digite o Nome do Aluno");
      nome = nome_aluno.nextLine();
      System.out.println("Digite a Serie do Aluno");
      serie = serie_aluno.nextInt();
      System.out.println("Digite sua Nota");
      nota = resultado.nextInt();

      if (nota == 0){
        System.out.println(nota + " "+ "Você Foi Reprovado! ");
      }
      else if (nota <= 6 ){
          System.out.print(nota + " " + "Você Esta Em Recuperação! ");
        }
        else if (nota >= 6){
          System.out.println( nota + " " + "Aluno Aprovado ");
        }
        else {
          System.out.println(nota + " " +  "A Nota Do Aluno Não Foi Aplicada! ");
        }
      
      contador++;
      
      System.out.println("O nome Do Aluno:" + nome + " A Serie do Aluno:" + serie );
         }
  }
}
