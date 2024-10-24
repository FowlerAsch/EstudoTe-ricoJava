# RoadMap JAVA ☕♨♨️

## Introdução: </>
Este repositório foi criado para guardar tudo o que aprendi na teoria sobre o desenvolvimento em Java. Além disso, também tem como foco ajudar aqueles que desejam iniciar o aprendizado na linguagem Java, oferecendo como base um RoadMap e conteúdos teóricos.

I created this repository to keep everything I've learned about Java development theory. It's also designed to help anyone looking to start learning Java, featuring a RoadMap and some theoretical content. Unfortunately, only in Portuguese yet.

## Sumário 💻

1. [Ideia sobre Classe, Atributos e Métodos](https://github.com/FowlerAsch/EstudoTeoricoJava/tree/main?tab=readme-ov-file#ideia-sobre-o-que-%C3%A9-classe-atributos-e-m%C3%A9todos)
2. [Atributo de Classe & Variável Local](https://github.com/FowlerAsch/EstudoTeoricoJava/tree/main?tab=readme-ov-file#classe--vari%C3%A1vel-local)
3. [Construtores](https://github.com/FowlerAsch/EstudoTeoricoJava/tree/main?tab=readme-ov-file#construtores)
4. [Sobrecarga](https://github.com/FowlerAsch/EstudoTeoricoJava/tree/main?tab=readme-ov-file#sobrecarga)
5. [Programação Orientada à objetos](https://github.com/FowlerAsch/EstudoTeoricoJava/tree/main?tab=readme-ov-file#programa%C3%A7%C3%A3o-orientada-%C3%A0-objetos)

# Ideia sobre o que é Classe, Atributos e Métodos:
> Vamos entender o que seria classe, atributos e métodos:
No mundo real, temos a estrutura/objeto 'carro' em diferentes países. A classe é a definição do que seria o carro; ou seja, possui quatro rodas, volante, marcha, entre outros atributos, que são chamados de atributos de classe ou gerais. A partir disso, o carro se diferencia de país para país. Em certos lugares, existem carros com o volante à direita, o tipo de marcha, o veículo pode ser elétrico, automático ou manual, entre outras variações de comportamento. Apesar dessas diferenças, ainda é considerado um carro, e essas variações são representadas nos métodos.

# Atributo de Classe & Variável Local
> ## Qual a diferença entre Atributo de Classe e Variável local?
> Anotação : Atributo de Classe & Variável Local: Quando você cria um atributo geral daquela classe ele se torna uma variável única que pode ser utilizada em diferentes métodos. Quando você não utiliza e precisa criar uma mesma variável em cada método ela se torna três variáveis diferentes com o mesmo nome existindo ao mesmo tempo, se tornando uma variável local. <br><br>
> Atributo de Classe: Ele pode ser acessado e modificado por diferentes métodos da classe, o que o torna uma variável compartilhada dentro da instância do objeto. Isso significa que, enquanto o objeto existir, o atributo pode ser acessado em qualquer método da classe. O valor do atributo é persistente enquanto o objeto estiver em uso, e qualquer alteração feita nele em um método será visível para os outros métodos da mesma instância. <br><br>
> Variável local: Uma variável local é definida dentro de um método e só existe enquanto o método está em execução. Ela é criada quando o método é chamado e destruída quando o método termina sua execução. Cada vez que o método é chamado, a variável local é recriada, e seu valor não é compartilhado entre chamadas de métodos ou entre outros métodos da classe. Isso significa que ela tem um escopo limitado e não pode ser acessada fora do método em que foi criada. <br>

# Construtores:
> Em Java , um construtor é um bloco de códigos similar ao método. É um tipo especial de método usado para inicializar o objeto. Ele fornece valores iniciais para variáveis de instâncias definidas pela classe. Ele também pode ser usado para configurar componentes que o objeto precisará utilizar. Toda vez que um objeto é criado usando a palavra-chave new(), pelo menos um construtor é chamado. Ele chama um construtor padrão se não houver nenhum construtor disponível na classe. Nesse caso, o compilador Java fornece um construtor padrão por padrão. Existem dois tipos de construtores em Java: construtor sem argumentos e construtor parametrizado.
> # Construtor vazio (Padrão):
> Esse tipo de construtor é utilizado quando você quer criar uma instância de uma classe, mas não tem valores específicos para inicializar os atributos do objeto logo de início. O construtor vazio geralmente deixa os atributos com valores padrão (como `null`, `0`, ou `false`, dependendo do tipo). Posteriormente, você pode definir os valores desses atributos através de métodos *setter* ou diretamente, se os atributos forem públicos.
> Como no exemplo abaixo:

> public class Carro { <br>
> private String modelo; <br>
> private int ano; <br>
> <br>
> // Construtor vazio (padrão) <br>
> public Carro() {<br>
> }<br>
>
> // Métodos Set para definir os valores<br>
> public void setModelo(String modelo) {<br>
>    this.modelo = modelo;<br>
}<br>
> <br>
> public void setAno(int ano) {<br>
>    this.ano = ano;<br>
> }<br>
>
> Carro carro = new Carro();<br>
> carro.setModelo("Fusca"); // inserindo as informações pelo método set<br>
> carro.setAno(1970);<br>

> # Construtor com paramêtro:
> O construtor com parâmetros permite inicializar o objeto com valores logo no momento da criação. Isso é útil quando você já tem todas as informações necessárias para definir o estado inicial do objeto. <br> <br>
> public class Carro {<br>
    private String modelo;<br>
    private int ano;<br>
>
>    // Construtor com parâmetros<br>
    public Carro(String modelo, int ano) {<br>
        this.modelo = modelo;<br>
        this.ano = ano;<br>
    }
>
>    // Métodos get para acessar os valores<br>
    public String getModelo() {<br>
        return modelo;<br>
    }
>
>    public int getAno() {<br>
        return ano;<br>
    }<br>
}

# Sobrecarga:
>  uma técnica que permite definir vários métodos com o mesmo nome, mas com diferentes parâmetros. A sobrecarga é muito útil porque permite que você use o mesmo nome de método para realizar diferentes tarefas, dependendo dos tipos ou quantidades de argumentos passados.
> ### Como funciona a sobrecarga?
>
> Para um método ser sobrecarregado, ele deve ter:
>
> - O **mesmo nome**.
> - **Parâmetros diferentes** (quantidade, tipo ou ordem).
>
>   public class Calculadora {<br>
>public int soma(int a, int b) {<br>
>    return a + b;<br>
> }<br>
>public int soma(int a, int b, int c) {<br>
>    return a + b + c;<br>
> }<br>
>}<br>

# Programação Orientada à Objetos:
> ### Herança
> O princípio da herança permite que uma classe (conhecida como superclasse ou classe pai) compartilhe atributos e métodos com outra classe (conhecida como subclasse ou classe filha). Essa relação hierárquica entre classes promove a reutilização de código e facilita a organização e manutenção do sistema. Um dos principais benefícios da herança é a **reutilização de código**. Em vez de reescrever o mesmo código em várias classes, você pode definir atributos e métodos comuns em uma superclasse e permitir que as subclasses herdem essas características. Outro aspecto importante da herança é a **sobrescrita de métodos** (ou overriding), onde uma subclasse pode fornecer uma implementação específica de um método que já existe na superclasse. Isso permite que diferentes subclasses se comportem de maneira distinta, mesmo que compartilhem uma interface comum. Por exemplo, uma superclasse `Animal` pode ter um método `fazerSom()`, enquanto as subclasses `Cachorro` e `Gato` podem sobrescrever esse método para produzir sons específicos, como "Au Au!" e "Miau!", respectivamente.
> ### Encapsulamento
> Encapsulamento é um conceito fundamental na programação orientada a objetos (POO). Ele se refere à prática de agrupar dados (atributos) e métodos (funções) que operam sobre esses dados em uma única unidade chamada de classe. A ideia principal do encapsulamento é restringir o acesso direto a alguns dos componentes de um objeto, o que ajuda a proteger o estado interno do objeto e a manter a integridade dos dados.
>  1. **Proteção dos Dados**: O encapsulamento permite que os dados de um objeto sejam protegidos contra acesso indevido. Isso é feito utilizando modificadores de acesso (como `private`, `protected`, `public`) que controlam a visibilidade dos atributos e métodos.
>  2. **Interface Pública**: Embora os dados sejam protegidos, a classe pode fornecer métodos públicos (também chamados de métodos de acesso ou "getters" e "setters") que permitem interagir com os dados de forma controlada. Por exemplo, em vez de permitir que um código externo acesse diretamente um atributo, você pode criar métodos que retornem ou modifiquem esse atributo.
> ### Polimorfismo
> O polimorfismo é um dos princípios fundamentais da programação orientada a objetos (POO). Ele se refere à capacidade de um objeto assumir várias formas. Em termos práticos, polimorfismo permite que uma classe derive outras classes e que essas classes derivadas possam ter comportamentos específicos, mesmo quando acessadas por meio de uma referência comum, como a de uma classe base. O polimorfismo se manifesta principalmente de duas formas: polimorfismo de sobrecarga (overloading) e polimorfismo de sobrescrita (overriding).
>  1. **O polimorfismo de sobrescrita** ocorre quando uma subclasse fornece sua própria implementação de um método que é declarado na superclasse, permitindo que a mesma interface (método) tenha comportamentos diferentes dependendo da classe que o invoca. Por exemplo, se tivermos uma classe Animal com o método fazerSom(), e subclasses como Cachorro e Gato que sobrescrevem esse método, um programa pode tratar todos os objetos como Animal, mas invocar o método fazerSom() produzirá sons específicos de cada tipo de animal, como "Au Au!" para cães e "Miau!" para gatos.
>  2. **O polimorfismo de sobrecarga**, por outro lado, ocorre quando uma classe tem vários métodos com o mesmo nome, mas com assinaturas diferentes (por exemplo, variando o número ou o tipo de parâmetros). Isso permite que um método seja utilizado de várias formas dependendo dos argumentos fornecidos. Um exemplo seria um método calcular que, dependendo dos parâmetros, pode somar dois números, calcular a área de um círculo ou realizar outras operações.
> ### Abstração
> Abstração é um dos pilares fundamentais da programação orientada a objetos (POO). Ela se refere à capacidade de modelar os aspectos essenciais de um objeto ou sistema, deixando de lado os detalhes complexos ou desnecessários para o contexto atual. Na prática, a abstração permite que os programadores definam classes e objetos com foco apenas nas propriedades e comportamentos relevantes para o problema que estão resolvendo, simplificando a complexidade Por exemplo, imagine uma classe abstrata FormaGeometrica com métodos como calcularArea() e calcularPerimetro(). A classe FormaGeometrica não sabe como calcular a área ou o perímetro de uma forma específica, mas define que todas as formas geométricas, como Círculo ou Retângulo, devem implementar esses métodos. Cada subclasse fornecerá sua própria implementação de acordo com suas características.<br>
> ### Associação
> A associação é um dos conceitos mais fundamentais na programação orientada a objetos (POO) e descreve o relacionamento entre duas classes, onde uma classe usa ou "se relaciona" com outra. Diferente de herança, onde há uma relação hierárquica (classe pai e classe filha), na associação as classes estão no mesmo nível e podem se relacionar de diferentes maneiras. Existem diferentes tipos de associação, dependendo da natureza do vínculo entre as classes:
>
> 1. Associação Simples: Representa uma relação simples entre duas classes, em que uma instância de uma classe pode conhecer a outra. Não há restrição de "posse" ou controle. Um exemplo seria a relação entre uma classe Aluno e uma classe Professor, onde um Aluno pode estar associado a um Professor sem que um possua o outro.
>
> 2. Agregação: É um tipo especial de associação que indica uma relação "todo-parte", onde uma classe (o "todo") é composta de outras classes (as "partes"), mas essas partes podem existir independentemente. Por exemplo, uma classe Carro pode ser composta por Rodas, Motor, e Portas, mas cada uma dessas partes pode existir separadamente ou ser reutilizada em outro carro. A agregação é representada por uma linha com um losango vazio em diagramas UML.
>
> 3. Composição: Similar à agregação, a composição também representa uma relação "todo-parte", mas com uma diferença crucial: na composição, as partes não podem existir sem o todo. Isso significa que a existência de uma classe depende totalmente da outra. Um exemplo clássico seria uma classe Casa e Quarto. Se a Casa for destruída, os Quartos também deixam de existir. Nos diagramas UML, a composição é representada por um losango preenchido.

