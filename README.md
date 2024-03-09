# AVC1
Primeira avaliação

/*Nome: Victória Mumpasi
  Id: 32493
  Engenharia Informática  
  Turma A
 */

/**
 * A classe PortaLogica representa uma porta lógica AND com duas entradas.
 */
public class PortaLogica {

    /** A primeira entrada da porta lógica. */
    private final boolean entrada1;

    /** A segunda entrada da porta lógica. */
    private final boolean entrada2;

    /**
     * Construtor da classe PortaLogica.
     * 
     * @param entrada1 O valor da primeira entrada.
     * @param entrada2 O valor da segunda entrada.
     */
    public PortaLogica(boolean entrada1, boolean entrada2) {
        this.entrada1 = entrada1;
        this.entrada2 = entrada2;
    }

    /**
     * Retorna as entradas da porta lógica.
     * 
     * @return Um array de booleanos contendo o valor das duas entradas.
     */
    public boolean[] obterEntradas() {
        return new boolean[] { entrada1, entrada2 };
    }

    /**
     * Retorna o valor da saída da porta lógica AND.
     * 
     * @return O valor da saída da porta lógica AND.
     */
    public boolean obterSaida() {
        return entrada1 && entrada2;
    }

    /**
     * Método de teste para demonstrar o funcionamento da classe.
     */
    public static void testar() {
        // Criar dois objetos da classe PortaLogica
        PortaLogica porta1 = new PortaLogica(true, false);
        PortaLogica porta2 = new PortaLogica(false, true);

        // Mostrar os valores das saídas das duas portas
        System.out.println("Saida da porta 1: " + porta1.obterSaida());
        System.out.println("Saida da porta 2: " + porta2.obterSaida());
    }

    /**
     * Método main para testar o funcionamento da classe.
     * 
     * @param args Os argumentos de linha de comando (não utilizados).
     */
    public static void main(String[] args) {
        // Testar o funcionamento da classe
        testar();
    }
}
