# SistemaDeContaBancaria

ackage sistemadecontabancaria;


public class SistemaDeContaBancaria {

    
    public static void main(String[] args) {
        Cliente C1 = new Cliente("Douglas Vieira", "87289989015");
        C1.exibir();
        ContaBancaria CB1 = new ContaBancaria("Douglas Vieira", 331815, 1.350);
        CB1.exibir();
    }
    
}

//Crie uma classe chamada `Cliente` com os seguintes atributos:
//- `nome`: uma string representando o nome do cliente.
//- `cpf`: uma string representando o número de CPF do cliente.
//A classe `Cliente` deve ter um construtor que recebe o nome e 
//o CPF do cliente e métodos para obter o nome e o CPF.
package sistemadecontabancaria;

public class Cliente {

    // variaveis
    private String Nome;
    private String Cpf;

    // metodo construtor
    public Cliente(String Nome, String Cpf) {

        this.Nome = Nome;
        this.Cpf = Cpf;

    }

    // metodo setNome
    public String setNome(String Nome) {
        this.Nome = Nome;
        return Nome;
    }

    // metodo getNome
    public String getNome() {
        return Nome;
    }

    //metodo setCpf
    public String setCpf(String Cpf) {
        this.Cpf = Cpf;
        return Cpf;

    }

    //metodo getCpf
    public String getCpf() {
        return Cpf;
    }

    public void exibir() {

        System.out.println("Nome: " + getNome());
        System.out.println("Cpf:" + getCpf());
        

    }
}


//2. **ContaBancaria**:
//Crie uma classe chamada `ContaBancaria` com os seguintes atributos:
//- `cliente`: um objeto da classe `Cliente` representando o titular da conta.
//- `numeroConta`: um número inteiro representando o número da conta.
//- `saldo`: um valor decimal representando o saldo atual da conta.
//A classe `ContaBancaria` deve ter os seguintes métodos:
//- `depositar(valor)`: adiciona o valor especificado ao saldo da conta.
//- `sacar(valor)`: retira o valor especificado do saldo da conta, desde que o saldo seja suficiente.
//- `getSaldo()`: retorna o saldo atual da conta.
//- `getNumeroConta()`: retorna o número da conta.
//- `getCliente()`: retorna o objeto `Cliente` associado à conta.
// Certifique-se de que o saldo nunca seja negativo ao realizar saques.
package sistemadecontabancaria;

public class ContaBancaria {

    //variaveis
    private String Cliente = "Douglas Vieira";
    private int NumeroConta = 331815;
    private double Saldo = 1.350;

    public ContaBancaria(String Cliente, int NumeroConta, double Saldo) {
        this.Cliente = Cliente;
        this.NumeroConta = NumeroConta;
        this.Saldo = Saldo;

    }
    //metodo setCliente

    public String setCliente(String Cliente) {

        this.Cliente = Cliente;
        return Cliente;
    }
    // metodo getCliente 
    public String getCliente(){
    
        return Cliente;
    }
    
    // metodo setNumeroConta
    public int setNumeroConta(int NumeroConta){
    this.NumeroConta = NumeroConta;
    return NumeroConta;
    }
    
    // metodo getNumeroConta
    public int getNumeroConta(){
    return NumeroConta;
    
    }
    
    // metodo setSaldo
    public double setSaldo(double Saldo){
    this.Saldo = Saldo;
    return Saldo;
    }
    
    // metodo getSaldo
    public double getSaldo(){
    return Saldo;
    }
    
    public double Depositar(){
    double Valor;
        System.out.println("Valor do Deposito:");
        Valor = Leia.nextdouble();
        
        
 }

}


package sistemadecontabancaria;


public class Transacao {
    
}


package sistemadecontabancaria;


public class Banco {
    
}
