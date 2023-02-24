# Calcula a média

## Classe que recebe as notas e retorna a média
````
package br.com.principal;

import javax.swing.JOptionPane;

import br.com.calculo.bo.Calculo; 

public class Principal {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		double nota1, nota2, nota3;
		
		JOptionPane.showMessageDialog(null, "Informe as três notas para o calculo da média.");
		
		nota1 = Double.parseDouble(JOptionPane.showInputDialog("Primeira nota:"));
		nota2 = Double.parseDouble(JOptionPane.showInputDialog("Segunda nota:"));
		nota3 = Double.parseDouble(JOptionPane.showInputDialog("Terceira nota:"));

		Calculo media = new Calculo();

		JOptionPane.showMessageDialog(null, "A sua média é: " + media.media(nota1, nota2, nota3));
		  
		}
}
````

## Classe que calcula a média
````
package br.com.calculo.bo;

public class Calculo {
	
	public double media(double n1, double n2, double n3) {
		return (n1+n2+n3)/3;
	}

}
````