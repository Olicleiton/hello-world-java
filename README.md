AdivinheOnumPanel - Modified Example Book Java for Dummies

	import javax.swing.JOptionPane;
	import java.util.Random;

	class AdininheOnumPanel {

		public static void main(String args[]) {

			String numDig = JOptionPane.showInputDialog("Digite um número inteiro de 1 a 20");
			int numDigitado = Integer.parseInt(numDig);
			int numAl = new Random().nextInt(20)+1;
			String numAleatorio = String.valueOf(numAl);

			if (numDigitado > 20) {
				JOptionPane.showMessageDialog(null ,"Número digitado fora do range solicitado"); // null dentro da JOptionMessage.Dialog é para não mostrar outra janela
			}

			else {
				if (numDigitado == numAl) {
					JOptionPane.showMessageDialog(null, "VOCÊ ACERTOU");
				}
				else {
					JOptionPane.showMessageDialog(null, "O numero era: " + numAleatorio);
				}

			}


		}

	}
