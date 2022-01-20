# Desafio da semana #3

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Declarar uma variável qualquer, que receba um objeto vazio.

var pessoa = {};


/*
Declarar uma variável `pessoa`, que receba suas informações pessoais.
As propriedades e tipos de valores para cada propriedade desse objeto devem ser:
- `nome` - String
- `sobrenome` - String
- `sexo` - String
- `idade` - Number
- `altura` - Number
- `peso` - Number
- `andando` - Boolean - recebe "falso" por padrão
- `caminhouQuantosMetros` - Number - recebe "zero" por padrão
*/

var pessoa = {
    nome: 'Diego',
    sobrenome: 'Silva',
    sexo: 'Masculino',
    idade: 20,
    altura: 1.67,
    andando: false,
    caminhouQUantosMetros: 0,
}


/*
Adicione um método ao objeto `pessoa` chamado `fazerAniversario`. O método deve
alterar o valor da propriedade `idade` dessa pessoa, somando `1` a cada vez que
for chamado.
*/

var pessoa = {
    nome: 'Diego',
    sobrenome: 'Silva',
    sexo: 'Masculino',
    idade: 20,
    altura: 1.67,
    andando: false,
    caminhouQUantosMetros: 0,
    fazerAniversario : function() {
        return this.idade = this.idade +1;
      }
}
// pessoa.fazerAniversario()

/*
Adicione um método ao objeto `pessoa` chamado `andar`, que terá as seguintes
características:
- Esse método deve receber por parâmetro um valor que representará a quantidade
de metros caminhados;
- Ele deve alterar o valor da propriedade `caminhouQuantosMetros`, somando ao
valor dessa propriedade a quantidade passada por parâmetro;
- Ele deverá modificar o valor da propriedade `andando` para o valor
booleano que representa "verdadeiro";
*/

var pessoa = {
    nome: 'Diego',
    sobrenome: 'Silva',
    sexo: 'Masculino',
    idade: 20,
    altura: 1.67,
    andando: false,
    caminhouQUantosMetros: 0,
    fazerAniversario : function() {
        return this.idade = this.idade +1;
    },
    andar: function(QntMC) {
        this.caminhouQUantosMetros += QntMC
        this.andando = true
    }
}
pessoa.andar(100);
// console.log(`Caminhou ${pessoa.caminhouQUantosMetros} mentros`);

/*
Adicione um método ao objeto `pessoa` chamado `parar`, que irá modificar o valor
da propriedade `andando` para o valor booleano que representa "falso".
*/
var pessoa = {
    nome: 'Diego',
    sobrenome: 'Silva',
    sexo: 'Masculino',
    idade: 20,
    altura: 1.67,
    andando: false,
    caminhouQUantosMetros: 0,
    fazerAniversario : function() {
        return this.idade = this.idade +1;
    },
    andar: function(QntMC) {
        this.caminhouQUantosMetros += QntMC
        this.andando = true
    },
    parar: function() {
        this.andando = false
    }
}

/*
Crie um método chamado `nomeCompleto`, que retorne a frase:
- "Olá! Meu nome é [NOME] [SOBRENOME]!"
*/

var pessoa = {
    nome: 'Diego',
    sobrenome: 'Silva',
    sexo: 'Masculino',
    idade: 20,
    altura: 1.67,
    andando: false,
    caminhouQUantosMetros: 0,
    fazerAniversario : function() {
        return this.idade = this.idade +1;
    },
    andar: function(QntMC) {
        this.caminhouQUantosMetros += QntMC
        this.andando = true
    },
    parar: function() {
        this.andando = false
    },
    nomeCompleto: function() {
        return `Olá! Meu nome é ${this.nome} ${this.sobrenome}!`
    }
}


/*
Crie um método chamado `mostrarIdade`, que retorne a frase:
- ""
*/
var pessoa = {
    nome: 'Diego',
    sobrenome: 'Silva',
    sexo: 'Masculino',
    idade: 20,
    altura: 1.67,
    andando: false,
    caminhouQUantosMetros: 0,
    fazerAniversario : function() {
        return this.idade = this.idade +1;
    },
    andar: function(QntMC) {
        this.caminhouQUantosMetros += QntMC
        this.andando = true
    },
    parar: function() {
        this.andando = false
    },
    nomeCompleto: function() {
        return `Olá! Meu nome é ${this.nome} ${this.sobrenome}!`
    },
    mostrarIdade: function() {
        return `Olá, eu tenho ${this.idade} anos!`
    }
}

/*
Crie um método chamado `mostrarPeso`, que retorne a frase:
- ""
*/
var pessoa = {
    nome: 'Diego',
    sobrenome: 'Silva',
    sexo: 'Masculino',
    idade: 20,
    altura: 1.67,
    peso: 50,
    andando: false,
    caminhouQUantosMetros: 0,
    fazerAniversario : function() {
        return this.idade = this.idade +1;
    },
    andar: function(QntMC) {
        this.caminhouQUantosMetros += QntMC
        this.andando = true
    },
    parar: function() {
        this.andando = false
    },
    nomeCompleto: function() {
        return `Olá! Meu nome é ${this.nome} ${this.sobrenome}!`
    },
    mostrarIdade: function() {
        return `Olá, eu tenho ${this.idade} anos!`
    },
    mostrarPeso: function() {
        return `Eu peso ${this.peso}Kg`
    },
}
/*
Crie um método chamado `mostrarAltura` que retorne a frase:
- "Minha altura é [ALTURA]m."
*/
var pessoa = {
    nome: 'Diego',
    sobrenome: 'Silva',
    sexo: 'Masculino',
    idade: 20,
    altura: 1.67,
    peso: 50,
    andando: false,
    caminhouQUantosMetros: 0,
    fazerAniversario : function() {
        return this.idade = this.idade +1;
    },
    andar: function(QntMC) {
        this.caminhouQUantosMetros += QntMC
        this.andando = true
    },
    parar: function() {
        this.andando = false
    },
    nomeCompleto: function() {
        return `Olá! Meu nome é ${this.nome} ${this.sobrenome}!`
    },
    mostrarIdade: function() {
        return `Olá, eu tenho ${this.idade} anos!`
    },
    mostrarPeso: function() {
        return `Eu peso ${this.peso}Kg`
    },
    mostrarAltura: function () {
        return `Minha altura é ${this.altura}m`
    }
}

/*
Agora vamos brincar um pouco com o objeto criado:
Qual o nome completo da pessoa? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
pessoa.name // Diego

/*
Qual a idade da pessoa? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
pessoa.idade // 20 

/*
Qual o peso da pessoa? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
pessoa.peso // 50

/*
Qual a altura da pessoa? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
pessoa.altura // 1.67

/*
Faça a `pessoa` fazer 3 aniversários.
*/
pessoa.fazerAniversario // 21
pessoa.fazerAniversario // 22
pessoa.fazerAniversario // 23

/*
Quantos anos a `pessoa` tem agora? (Use a instrução para responder e
comentários inline ao lado da instrução para mostrar qual foi a resposta
retornada)
*/
pessoa.mostrarIdade() // 23

/*
Agora, faça a `pessoa` caminhar alguns metros, invocando o método `andar` 3x,
com metragens diferentes passadas por parâmetro.
*/
pessoa.andar(100)
pessoa.andar(20)
pessoa.andar(300)

/*
A pessoa ainda está andando? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
pessoa.andando // true

/*
Se a pessoa ainda está andando, faça-a parar.
*/
pesso.parar()

/*
E agora: a pessoa ainda está andando? (Use uma instrução para responder e
comentários inline ao lado da instrução para mostrar a resposta retornada)
*/
pessoa.andado  // false

/*
Quantos metros a pessoa andou? (Use uma instrução para responder e comentários
inline ao lado da instrução para mostrar a resposta retornada)
*/
pessoa.caminhouQUantosMetros // 420

/*
Agora vamos deixar a brincadeira um pouco mais divertida! :D
Crie um método para o objeto `pessoa` chamado `apresentacao`. Esse método deve
retornar a string:
- "Olá, eu sou o [NOME COMPLETO], tenho [IDADE] anos, [ALTURA], meu peso é [PESO] e, só hoje, eu já caminhei [CAMINHOU QUANTOS METROS] metros!"

Só que, antes de retornar a string, você vai fazer algumas validações:
- Se o `sexo` de `pessoa` for "Feminino", a frase acima, no início da
apresentação, onde diz "eu sou o", deve mostrar "a" no lugar do "o";
- Se a idade for `1`, a frase acima, na parte que fala da idade, vai mostrar a
palavra "ano" ao invés de "anos", pois é singular;
- Se a quantidade de metros caminhados for igual a `1`, então a palavra que
deve conter no retorno da frase acima é "metro" no lugar de "metros".
- Para cada validação, você irá declarar uma variável localmente (dentro do
método), que será concatenada com a frase de retorno, mostrando a resposta
correta, de acordo com os dados inseridos no objeto.
*/
var pessoa = {
    nome: 'Diego',
    sobrenome: 'Silva',
    sexo: 'Masculino',
    idade: 20,
    altura: 1.67,
    peso: 50,
    andando: false,
    caminhouQUantosMetros: 0,
    fazerAniversario : function() {
        return this.idade = this.idade +1;
    },
    andar: function(QntMC) {
        this.caminhouQUantosMetros += QntMC
        this.andando = true
    },
    parar: function() {
        this.andando = false
    },
    nomeCompleto: function() {
        return `Olá! Meu nome é ${this.nome} ${this.sobrenome}!`
    },
    mostrarIdade: function() {
        return `Olá, eu tenho ${this.idade} anos!`
    },
    mostrarPeso: function() {
        return `Eu peso ${this.peso}Kg`
    },
    mostrarAltura: function () {
        return `Minha altura é ${this.altura}m`
    },
    apresentacao: function(){
        return `Olá, eu sou o ${this.nome} ${this.sobrenome}, tenho ${this.idade} anos, ${this.altura}, meu peso é ${this.peso} e, só hoje, eu já caminhei ${this.caminhouQUantosMetros} metros!`
    }
}


// Agora, apresente-se ;)

pessoa.apresentacao();
```