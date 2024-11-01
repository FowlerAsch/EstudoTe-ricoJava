# Ideia sobre o que é Classe, Atributos e Métodos:
> Vamos entender o que seria classe, atributos e métodos:
No mundo real, temos a estrutura/objeto 'carro' em diferentes países. A classe é a definição do que seria o carro; ou seja, possui quatro rodas, volante, marcha, entre outros atributos, que são chamados de atributos de classe ou gerais. A partir disso, o carro se diferencia de país para país. Em certos lugares, existem carros com o volante à direita, o tipo de marcha, o veículo pode ser elétrico, automático ou manual, entre outras variações de comportamento. Apesar dessas diferenças, ainda é considerado um carro, e essas variações são representadas nos métodos.

# Atributo de Classe & Variável Local
> ## Qual a diferença entre Atributo de Classe e Variável local?
> Anotação : Atributo de Classe & Variável Local: Quando você cria um atributo geral daquela classe ele se torna uma variável única que pode ser utilizada em diferentes métodos. Quando você não utiliza e precisa criar uma mesma variável em cada método ela se torna três variáveis diferentes com o mesmo nome existindo ao mesmo tempo, se tornando uma variável local. <br><br>
> Atributo de Classe: Ele pode ser acessado e modificado por diferentes métodos da classe, o que o torna uma variável compartilhada dentro da instância do objeto. Isso significa que, enquanto o objeto existir, o atributo pode ser acessado em qualquer método da classe. O valor do atributo é persistente enquanto o objeto estiver em uso, e qualquer alteração feita nele em um método será visível para os outros métodos da mesma instância. <br><br>
> Variável local: Uma variável local é definida dentro de um método e só existe enquanto o método está em execução. Ela é criada quando o método é chamado e destruída quando o método termina sua execução. Cada vez que o método é chamado, a variável local é recriada, e seu valor não é compartilhado entre chamadas de métodos ou entre outros métodos da classe. Isso significa que ela tem um escopo limitado e não pode ser acessada fora do método em que foi criada. <br>

# Métodos
> Em produção...

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
