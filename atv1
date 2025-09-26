public class AtividadesPOO2 {

    // ====================== QUESTÃO 1 ======================
    // Classe Livro (ProjetoLivraria)
    public static class Livro {
        String titulo;
        String autor;
        double preco;

        public Livro(String titulo, String autor, double preco) {
            this.titulo = titulo;
            this.autor = autor;
            this.preco = preco;
        }

        public void mostrarInfo() {
            System.out.println("Título: " + titulo + ", Autor: " + autor + ", Preço: R$" + preco);
        }

        public void aplicarDesconto(double porcentagem) {
            preco -= preco * (porcentagem / 100);
        }
    }

    // ====================== QUESTÃO 2 ======================
    // Nova classe para a Livraria: Cliente
    public static class Cliente {
        String nome;
        String email;
        int idade;

        public Cliente(String nome, String email, int idade) {
            this.nome = nome;
            this.email = email;
            this.idade = idade;
        }

        public void mostrarInfo() {
            System.out.println("Cliente: " + nome + ", Email: " + email + ", Idade: " + idade);
        }

        public void comprarLivro(Livro livro) {
            System.out.println(nome + " comprou o livro " + livro.titulo);
        }
    }

    // ====================== QUESTÃO 3 ======================
    // ProjetoAluno
    public static class Aluno {
        String nome;
        int matricula;
        double notaAv1;
        double notaAv2;

        public Aluno(String nome, int matricula, double notaAv1, double notaAv2) {
            this.nome = nome;
            this.matricula = matricula;
            this.notaAv1 = notaAv1;
            this.notaAv2 = notaAv2;
        }

        public void mostrarDados() {
            System.out.println("Nome: " + nome + ", Matrícula: " + matricula +
                    ", Av1: " + notaAv1 + ", Av2: " + notaAv2);
        }

        public double calcularMedia() {
            return (notaAv1 + notaAv2) / 2;
        }

        public void verificarAprovacao() {
            double media = calcularMedia();
            if (media >= 7.0) {
                System.out.println(nome + " foi aprovado! Média: " + media);
            } else {
                System.out.println(nome + " foi reprovado. Média: " + media);
            }
        }
    }

    // ====================== QUESTÃO 4 ======================
    // ContaBancaria
    public static class ContaBancaria {
        String numeroConta;
        String titular;
        double saldo;

        public ContaBancaria(String numeroConta, String titular, double saldoInicial) {
            this.numeroConta = numeroConta;
            this.titular = titular;
            this.saldo = saldoInicial;
        }

        public void depositar(double valor) {
            saldo += valor;
            System.out.println("Depósito de R$" + valor + " realizado. Saldo atual: R$" + saldo);
        }

        public void sacar(double valor) {
            if (valor <= saldo) {
                saldo -= valor;
                System.out.println("Saque de R$" + valor + " realizado. Saldo atual: R$" + saldo);
            } else {
                System.out.println("Saldo insuficiente!");
            }
        }

        public void consultarSaldo() {
            System.out.println("Saldo da conta " + numeroConta + ": R$" + saldo);
        }
    }

    // ====================== QUESTÃO 5 ======================
    // ProjetoCarro
    public static class Carro {
        String marca;
        String modelo;
        int ano;

        public Carro(String marca, String modelo, int ano) {
            this.marca = marca;
            this.modelo = modelo;
            this.ano = ano;
        }

        public void mostrarInfo() {
            System.out.println("Carro: " + marca + " " + modelo + ", Ano: " + ano);
        }

        public void ligar() {
            System.out.println("O carro " + marca + " " + modelo + " está ligado!");
        }
    }

    // ====================== MAIN ======================
    public static void main(String[] args) {

        // ===== Questão 1 =====
        System.out.println("\n=== QUESTÃO 1 ===");
        Livro l1 = new Livro("Dom Casmurro", "Machado de Assis", 50.0);
        Livro l2 = new Livro("O Hobbit", "J.R.R. Tolkien", 80.0);

        l1.mostrarInfo();
        l2.mostrarInfo();
        l1.aplicarDesconto(10);
        l1.mostrarInfo();

        // ===== Questão 2 =====
        System.out.println("\n=== QUESTÃO 2 ===");
        Cliente c1 = new Cliente("João", "joao@email.com", 25);
        c1.mostrarInfo();
        c1.comprarLivro(l2);

        // ===== Questão 3 =====
        System.out.println("\n=== QUESTÃO 3 ===");
        Aluno a1 = new Aluno("Maria", 101, 8.0, 7.0);
        Aluno a2 = new Aluno("Pedro", 102, 5.0, 6.0);

        a1.mostrarDados();
        a1.verificarAprovacao();

        a2.mostrarDados();
        a2.notaAv2 = 8.5; // atualizando nota
        a2.mostrarDados();
        a2.verificarAprovacao();

        // ===== Questão 4 =====
        System.out.println("\n=== QUESTÃO 4 ===");
        ContaBancaria conta1 = new ContaBancaria("123", "Ana", 1000.0);
        ContaBancaria conta2 = new ContaBancaria("456", "Carlos", 500.0);

        conta1.depositar(200);
        conta1.sacar(300);
        conta1.consultarSaldo();

        conta2.depositar(100);
        conta2.sacar(700);
        conta2.consultarSaldo();

        // ===== Questão 5 =====
        System.out.println("\n=== QUESTÃO 5 ===");
        Carro carro1 = new Carro("Toyota", "Corolla", 2020);
        Carro carro2 = new Carro("Honda", "Civic", 2018);

        carro1.mostrarInfo();
        carro1.ligar();

        carro2.mostrarInfo();
        carro2.ano = 2022; // modificando atributo
        carro2.mostrarInfo();
        carro2.ligar();
    }
}
