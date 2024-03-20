import java.util.Scanner;

public class letraN {

public static void main(String[] args){

     Scanner teclado = new Scanner(System.in);
     
     int opção; 
     
     double n1, n2, n3, aux;
     
     System.out.println("insira uma opção de 1 a 3" );
     
     opção = teclado.nextInt();
     
     if(opção<1 || opção>3) System.out.println("esse numero é invalido deve ser um valor de 1 á 3" );
     
     else {
         
         
         System.out.println("Insira o valore de n1 ");
     
     n1 = teclado.nextDouble();

     System.out.println("Insira o valore de n2 ");
     
     n2 = teclado.nextDouble();
     
     System.out.println("Insira o valore de n3 ");
     
     n3 = teclado.nextDouble();

         if(n2<n1){
         
             aux = n1;
             
             n1 = n2;
             
             n2 = aux;
             
         }
         
         if(n3<n1){
         
             aux = n1;
             
             n1 = n3;
             
             n3 = aux;
         }
         
         if(n3<n2){
         
             aux = n2;
             
             n2 = n3;
             
             n3 = aux;
             
         }
         
         if(opção==1) System.out.println("a ordem crescente dos valores é " + n1 + " " +n2+ " " +n3);
         
         else if(opção==2) System.out.println("a ordem decrescente dos valores é " +n3+ " " +n2+ " " +n1);
         
         else System.out.println("a ordem com o valor maior no meio " +n1+ " " +n3+ " " +n2);
     
     
    }
    
}

}
