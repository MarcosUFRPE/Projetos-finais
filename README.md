# Projetos-finais
public class Caracteristicapersonagem {
    String nome;
    float altura;
    int idade;
    int energia; 
    void ataque(int qtataque){
       energia-=qtataque;

    }

}


import java.util.Scanner;






/**
 * App
 */
public class App {

    public static void main(String[] args) {
       Caracteristicapersonagem amigo1 =new Caracteristicapersonagem();
           amigo1.nome="martin";
           amigo1.altura=2.10f;
           amigo1.idade=29;
           amigo1.energia=100;
           amigo1.ataque(0);
        Caracteristicapersonagem amigo2 =new Caracteristicapersonagem();
           amigo2.nome="Assasino";
           amigo2.altura=1.75f;
           amigo2.idade=30; 
           amigo2.energia=100;
           amigo2.ataque(0); 
        Caracteristicapersonagem amigo3 =new Caracteristicapersonagem();
           amigo3.nome="Joana";
           amigo3.altura=1.70f;
           amigo3.idade=26;
           amigo3.energia=100;
           amigo3.ataque(0);  
         Caracteristicapersonagem espirito=new Caracteristicapersonagem();
           espirito.nome="Joao";
           espirito.altura=3.00f;
           espirito.idade=500;
           espirito.energia=300;
           espirito.ataque(0);
        
         











         Scanner his=new Scanner(System.in);
         System.out.println("Um certo dia três amigos,"+amigo1.nome+","+amigo2.nome+" e "+amigo3.nome+ ",resoveram fazer uma trilha pela floresta"
          +" "+"chegando lá  eles avistaram uma  casa abandonada."); 

         System.out.println("O que eles tem que fazer?: 1 ir até a casa ou 2 passar direto");
         String resp= his.nextLine();
         if (resp.equals("1")){ 

           System.out.println("Chegando na casa abandonada ,eles entram e encontram um livro chamado ,os 7 espirito amaldiçoado .");
           System.out.println("1 :Eles pegam o livro e ler ?ou 2 :Deixam o livro queto ?");
           String reesp=his.nextLine();

           if (reesp.equals("1")){
           System.out.println("E assim que eles acabam de ler o livro ,sete espito amaldiçoado desperta para atormentar a vida daqueles ");
           System.out.println("que acordaram eles de seu sono profundo e entre esses sete espito está o " + espirito.nome );
           System.out.println( "um espirito de "+" "+ espirito.altura + "m de altura e " + espirito.idade + " anos  de idade");
           System.out.println ("e que quando era um homem foi um psicopata que matou milhares de pessoas");
           System.out.println( "e que  quando a polic1ia pegou ele  torturou e matou ele nessa casa abandonada   e até ");
           System.out.println("hoje seu espito vive nessa casa,sendo o lider dos outros seis espirito  ."  );

           System.out.println("Agora a missão dos três amigos é encontrar uma forma de fazer com que os 7 espiro voltem para o seu sono profundo,caso não ");
           System.out.println(" os espirito vão pegar  atormenta e tortura eles ate morre.");
           System.out.println("sedo  que as portas da casa abandonada se fecharam quando os espiritos depestaram"  );
           System.out.println("assim os tres amigos nao tem como simplemente sair da casa .");
           System.out.println("como eles nao conseguia sair da casa resolveram caçar alguma soluação dentro da casa "); 
           System.out.println(" em buca de alguma solução eles acabam dando de cara com um dos espitos que acaba atacando eles ");
           System.out.println("e que acaba acertado ,"+amigo2.nome+ " ,com uma paulada  fazendo com quer " +amigo2.nome );
           amigo2.ataque(1);
           System.out.println( "perca  energia ,deixando de ter 100 de sua energia e ficando com  " + amigo2.energia );
           }else{
            System.out.println("E deixando o livro quieto eles se livra do tormento de 7 espirito amaldiçoado.");
           }
         
          }else{ 
          System.out.println(" E assim foi mais um dia normal na vida deles!");
         }
         his.close();
    }


}
