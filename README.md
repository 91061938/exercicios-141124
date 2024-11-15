# exercicios-141124
<?php

class Pessoa {
    // Atributos
    private $nome;
    private $idade;

    // Construtor que recebe nome e idade
    public function __construct($nome, $idade) {
        $this->nome = $nome;
        $this->idade = $idade;
    }

    // Método para retornar o nome da pessoa
    public function setNome() {
        return $this->nome;
    }

    // Método para definir a nova idade da pessoa
    public function setIdade($idade) {
        $this->idade = $idade;
    }

    // Método para retornar a idade da pessoa
    public function getIdade() {
        return $this->idade;
    }
}

// Criando uma instância da classe Pessoa
$pessoa = new Pessoa("João", 30);

// Exibindo as informações
echo "Nome: " . $pessoa->setNome() . "<br>"; // Exibe o nome
echo "Idade: " . $pessoa->getIdade() . " anos<br>"; // Exibe a idade

// Alterando a idade da pessoa
$pessoa->setIdade(35);

// Exibindo as novas informações
echo "Nova idade: " . $pessoa->getIdade() . " anos<br>"; // Exibe a nova idade

?>
