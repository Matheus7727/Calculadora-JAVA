# calculadora java

import java.util.Scanner;

public class missao1 {

	public static void main(String[] args) {

	  Scanner entrada = new Scanner(System.in); 
		
	     //SOMA
		System.out.println("Digite um numero: "); 
		int n1 =  entrada.nextInt(); 
		System.out.println("Digite um outro numero:"); 
		int n2 =  entrada.nextInt(); 
		double RESULTADO = (n1 + n2);
		System.out.println("O resultado da SOMA e: " + RESULTADO );
        System.out.println("___________________________________");
       
         //SUBTRAÇÃO
		System.out.println("Digite um numero: "); 
		int n3 =  entrada.nextInt(); 
		System.out.println("Digite um outro numero:"); 
		int n4 =  entrada.nextInt(); 
		double RESULTADO2 = (n3 - n4);
		System.out.println("O resultado da SUBTRACAO e: " + RESULTADO2 );
		 System.out.println("___________________________________");
		 
		 //MULTPLICAÇÃO
		System.out.println("Digite um numero: "); 
		int n5 =  entrada.nextInt(); 
		System.out.println("Digite um outro numero:"); 
		int n6 =  entrada.nextInt(); 
		double RESULTADO3 = (n5 * n6);
		System.out.println("O resultado da MULTPLICACAO e: " + RESULTADO3 );
		 System.out.println("___________________________________");
       
		 //DIVISÃO
		System.out.println("Digite um numero: "); 
		int n7 =  entrada.nextInt(); 
		System.out.println("Digite um outro numero:"); 
		int n8 =  entrada.nextInt(); 
		double RESULTADO4 = (n5 / n6);
		System.out.println("O resultado da DIVISAO e: 0.0" );
		 System.out.println("___________________________________");
		 }}

	*
 * Autor: Matheus Silva Batista
 * Data: 12/09/2002
 */
public class Missao3_Calculadora {
	//DECLARANDO OS ATRIBUTOS DA CLASE
	private double R;
	
   public double SOMAR(double N1, double N2)
   {//INICÍO DO MÉTODO SOMAR 
	   //AQUI DEVE SER INSERIDO O BLOCO DE CÓDIGO QUE FAZ A SOMA
	   R= N1 + N2;
	   return R;
   }   //FIM DO MÉTODO SOMAR
   
     public double SUBTRAIR(double N1, double N2)
     {//INICIO DO MÉTODO SUBTRAIR
    	 //AQUI DEVE SER INSERIDO O BLOCO DE CÓDIGO QUE FAZ A SUBTRAÇÃO
    	 R = N1 - N2;
    	  return R;
     }//FIM DO MÉTODO SULBTRAIR
   
     public double MULTIPLICAR(double N1, double N2)
     {//INICIO DO MÉTODO MULTIPLICAR
    	 //AQUI DEVE SER INSERIDO O BLOCO DE CÓDIGO QUE FAZ A MULTIPLICAÇÃO
    	 R = N1 * N2;
    	  return R;
     }//FIM DO MÉTODO MULTIPLICAR
    
     
     
     //METODO DIVIDIR
     public double DIVIDIR(int N1, int N2)
     {  
    	 try
    	 {
    	 if(N1/N2<Double.MAX_VALUE)
    	 {
     
    	 return N1/N2;
    	 }
     else 
     {
    	 System.out.println("Divisao por zero!");
    	 return 0;
     }
    	 }
    	 catch(Exception e)
    	 {
     System.out.println("Erro ao executar a divisao!");
     return 0;
    	 }
     
     }}
		    
	
	public static void main(String[] args) {
		  
		 double R_SOMA, R_SUBTRAIR, R_MULTIPLICAR, R_DIVIDIR;
		
		 
		 System.out.println("Início da Missão 3");
		Missao3_Calculadora obj_calculadora = new Missao3_Calculadora();
	R_SOMA = obj_calculadora.SOMAR(1,2);
	System.out.println("O resultado da soma é: " + R_SOMA);
	R_SUBTRAIR = obj_calculadora.SUBTRAIR(10.5 , 4.2);
	System.out.println("O resultado sa soma é: " + R_SUBTRAIR);
	R_MULTIPLICAR = obj_calculadora.MULTIPLICAR(2.2,5.5);
	System.out.println("O resultado sa soma é: " + R_MULTIPLICAR);
	R_DIVIDIR = obj_calculadora.DIVIDIR(0,0);
   System.out.println("Oresultado da soma é: " + R_DIVIDIR);
	
	
	
	
	
}

}
	
