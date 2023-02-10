//coded by Gabriel Dario 
//RM 95946
//DIVINE GROUP Ω

package sprinyt;

import java.util.Arrays;
import java.util.Scanner;

public class Sprint3java {

	public static void main(String[] args) {
		Scanner entry = new Scanner(System.in);

		int numEscolhido = 0;
		int qntEquipes = 0;
		int[] numeroEquipes = new int[99];
		
		

		// captacao quantidade de equipes

		System.out.println("------------------------------------------------------");
		System.out.print("Digite a quantidade de equipes participantes da competição");
		qntEquipes = entry.nextInt();

		// criacao array bi-dim com tamanho igual a
		// quantidade de equipes solicitadas anteriormente
		int[][] infoEquipes = new int[qntEquipes][8];
		int[][] placar = new int[qntEquipes][3]; //numero c=0  c=1

		System.out.println("");
		System.out.println("------------------------------------------------------");
		System.out.println("INFORMACOES DA EQUIPE");

		for (int l = 0; l < infoEquipes.length; l++) {

			// captacao numero da equipe 11 a 99
			System.out.println("");
			System.out.println("numeros validos: 11 a 99.");
			System.out.print("Digite o numero da equipe " + (l + 1) + (": "));

				numEscolhido = entry.nextInt();

				//// validacao 11 a 99
					while (!((numEscolhido >= 11) && (numEscolhido <= 99))) {
					System.out.println("");
					System.out.println("Voce digitou um numero invalido!");
					System.out.println("numeros validos: 11 a 99.");
					System.out.print("Digite um numero valido para a equipe " + (l + 1) + (": "));
						numEscolhido = entry.nextInt();
			}

				//// validacao numero ja escolhido
					while (numeroEquipes[(numEscolhido-1)] == 1) {
					System.out.println("");
					System.out.println("Ja existe uma equipe registrada com esse numero!");
					System.out.print("Digite um numero ainda nao escolhido: ");
						numEscolhido = entry.nextInt();
			}
					//// salvando numero ja validado no array
						numeroEquipes[(numEscolhido-1)] = 1;
						infoEquipes[l][1] = numEscolhido;
			
			
			
			
			//captacao numero de combates
			
				////vitorias c=3
					System.out.println("");
					System.out.print("Digite o numero de VITORIAS da equipe " + (infoEquipes[l][1]) + (": "));
						infoEquipes[l][3]=entry.nextInt();
			
				////derrotas c=4
					System.out.println("");
					System.out.print("Digite o numero de DERROTAS da equipe " + (infoEquipes[l][1]) + (": "));
						infoEquipes[l][4]=entry.nextInt();
					
				////empates c=5
					System.out.println("");
					System.out.print("Digite o numero de EMPATES da equipe " + (infoEquipes[l][1]) + (": "));
						infoEquipes[l][5]=entry.nextInt();
					
					
			
						////somador numero de combates c=2 (c3+c4+c5)
						infoEquipes[l][2] = (infoEquipes[l][3])+(infoEquipes[l][4])+(infoEquipes[l][5]);
						
						
				
					
			//captacao nota c=6
			System.out.println("");
			System.out.print("Digite a nota de 0 a 100 para designer da equipe " + (infoEquipes[l][1]) + (": "));
				infoEquipes[l][6]=entry.nextInt();
				
				
			//processamento pontos c=7 (c3*5 + c4*3) 
				infoEquipes[l][7]=((infoEquipes[l][3])*5)+((infoEquipes[l][4])*3);
				
				
			//novo array 2d ponto numero
				placar[l][0]=infoEquipes[l][1];
				placar[l][1]=infoEquipes[l][7];
				placar[l][2]=infoEquipes[l][6];
		}
		
		//sort array placar
		
		System.out.println("");
		System.out.println("------------------------------------------------------");
		System.out.println("");
		
			////sort nota de designer		
					Arrays.sort(placar, (a, b) -> b[2] - a[2]);  // precisa desse sort para o criterio de desempate
					
					
			////sort pontos
					Arrays.sort(placar, (a, b) -> b[1] - a[1]);  
					
					
		//display do array
		for (int i = 0; i < placar.length; i++){	
			System.out.println("Colocacao "+(i+1)+"    Numero da equipe: "+(placar[i][0])+"   Pontos da equipe: "+placar[i][1] +"   Nota de designer: "+(placar[i][2]));
			}
					
					
			System.out.println("");
			System.out.println("------------------------------------------------------");
			System.out.println("Ω");

	}

}

//coded by Gabriel Dario. 
//RM 95946
//DIVINE GROUP Ω

