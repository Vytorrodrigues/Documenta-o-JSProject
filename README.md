# Documenta-o-JSProject

- Documentação de todo conteúdo de Javascript que estudei até agora
- Está documentação é para organizar o conteúdo e facilitar nos estudos e revisões futuras
- Vocês podem adicionar as anotações de vocês, o objetivo é deixar essa documentação robusta e de fácil entendimento para todos
- **LEMBREM DE FAZER OS COMMITS REGISTRANDO AS MUDANÇAS PFV**

# Declaração de variáveis:

- Const, let e var: 
- Const possui escopo/alcance global e não pode ser alterado
- Var também possui escopo global, mas ela pode ser mudada facilmente, por isso não é muito bom usa-lá
- Let possui escopo global e local, a depender de onde for inserida
- Escopo é onde e como determinado elemento são acessíveis
- Variáveis em JS são case sensitive, ou seja: diferenciam letras maíusculas de minúsculas 
ex: let nome = "Pedro"; é diferente de let Nome = "Pedro";
- No js vc pode declarar tanto em camel case: nomeObjeto, como em snake case: nome_objeto
- Não pode usar espaço para declarar uma variável


# Operadores: 

* = em JS significa recebe determinado valor
- Números flutuantes em JS usam o . 
ex: 1.2, 4.56 etc
- + (Soma), - (Subtração), / (Divisão inteira), * (Multiplicação) , ** (Potência), % (Mod/ Módulo/ Resto)
- ++ (Incremento), -- (Decremento): Aritméticos
- += (a = a + 1), -=, *=, /=, **=, %=, : Atribuição
- == (Igual), === (Igual ao tipo de elemento, string, número, booleano etc), != (Diferente), !== (Dieferente do tipo), >(Maior), <(Menor), <= (Menor igual), >= (Maior igual), ??= (igual a null ou undefined): *Comparadores*
- && (*and*), || (*or*), !() (*not*): Operadores lógicos dão respostas binárias, True(1) ou False(0)
- *Ordem de procedência*: (), **, *  /  %, +  -
- *Ordem de procedência dos operadores lógicos*: !, &&, ||

# Ternário:

- Teste lógico
- ? :  -> ->  Teste? True: False;

# Functions:

- Conjunto de instruções dentro de um determinado escopo, que pode ser ativado ao digitar seu nome
ex: function falar(){};
falar(); Aqui eu estou chamando a função para ativala
- Dentro dos parenteses vão seus parametros ex: event
- Arrow function ou FUNÇÃO ANÔNIMA é a forma simplificada de escrever uma função ex: **() => {};**
- Muito utilizada em Programação Orientada a Objetos (POO), permite agrupamento e reuso do código, sequência lógica, além de permitir um código escalável, de fácil entendimento, boa manuntenção, prolongando a vida do script

# Comandos anotados:

- **typeof()** verifica o tipo do elemento, string, object, number
- **Number()** transforma elemento em número, usado quando não precisa definir se é inteiro ou decimal
- **parseInt()** para transformar em inteiro 
- **parseFloat()** para um flutuante
- **string()** ou toString() muda para uma string ou só colocar dentro de aspas ""
- **toUpperCase()**deixa maíusculo
- **toLowerCase()** deixa minúsculo
- **toFixed()** permite selecionar quantas casas decimais queremos que o número apresente
- **replace()** permite alterar ponto por vírgula
- **toLocaleString("pt-br", {style: "currency", currency: "BRL"})** exibição de valor monetário, euro, dolar, yen, etc
- **.createElement()** cria um elemento tag HTML
- **.setAttribute("atributo, nome")** coloca um atributo em um elemento HTML, id, class, src etc

# Formatador:

- Ao usar crase pode passar o formatador dentro  ex: `${variável}`
- Formatadores ajudam a evitar muitas concatenações, a depender do caso

# Document Object Notation (DOM):

- window, document, body, html etc. São elementos da árvore DOM, eles seguem a linha de como o código HTML é montado, como raízes de uma árvore, aqueles acima são pais dos elementos abaixo
ex: window -> location
    document -> head/body 
- **.querySelector()** nome da tag, com id ou classe que vc deseja selecionar no document
- **.querySelectorAll()** seleciona  todos os elementos de mesmo nome
- **.getElementById()** pega o elemento HTML baseado em seu ID
- **.getElementByTagName()**  não entendi como funciona esse direito *TODO: PESQUISAR*
- **.getElementByName()[]** não entendi como funciona esse direito *TODO: PESQUISAR*
- **.getElementByclassName()[]** não entendi como funciona esse direito *TODO: PESQUISAR*
- **.innerText = ""** usado para inserir texto no código HTML
- **.innerHTML = ""** pega a formatação e passa direto para o código, mas deve ter cuidado para não inserir códigos sensiveis pois pode exibir brechas e permitir invasões no sistema 

# DOM Events:

- **onclick**: ao clicar com o mouse no elemento
- **ondblclick**: dois clicks no elemento
- **onmouseover**: passar mouse em cima do elemento
- **onmouseout**:  dispara quando o mouse sai do elemento
- **onmousemove**: mouse movido dentro do elemento
- **onmousedown**: clique do scroll do mouse precionado
- **onmouseup**: quando o clique do botão do mouse que estava pressionado é solto
- **onfocus**:  dispara quando elemeno recebe foco
- **onchange**: dispara ao mudar o conteúdo
- **onblur**: quando o elemento perde o foco
- **onkeydown**: quando uma tecla é pressionada
- **onkeypress**: quando tecla pressionada é solta
- **onkeyup**: quando a tecla é solta sobre um elemento
- **onload**: dispara ao carregar página
- **onresize**: dispara ao redimensionar tela
- **focus**: focar campo

- Os eventos podem ser chamados de duas formas: variável.evento(função que quero chamar); ou variável.addEventListenner("evento", função sem parenteses);

# Objetos:

- Objetos são elementos declarados com {} onde recebem uma propriedade e um valor
ex: const localizacao = {
        cidade: "João Pessoa",
        cep: 679802,
        rua: "Antonio Valdenor Labamda"
        pais: function localidade(){}; -Isso é um método
}
- Objetos também podem receber funções em seus valores, o que chamamos de métodos

# Array/Matrizes:

- Usada para armazenar valores, objetos, variáveis etc. Ela é armazenada em uma variável
- Array vazio: let arr = [];
- As posições do array são contadas a partir do 0, ou seja: let arr = [1, 2, 3, 4]; equivale a 0, 1, 2, 3 em relação as posições
- **Array.isarray()** é usado para descobrir se tal elemento é um array

- **.join()** troca separador dos itens do meu array
- **.pop()** remove o último elemento do array
- **.shift()** remove o primeiro elemento 
- **.lenght()** mostra quantos elementos/comprimento do array 
- **array[array.length - 1(aqui eu passo o valor de quantos elementos quero verificar)]** verifica o elemento do array e me retorna seu valor, de trás para frente
- **unshift()** adiciona um item a primeira posição
- **.push()** adiciona elementos no final
- **.splice( posição do elemento, quantidade de itens que quero remover, qual item quero adicionar)**;
-* *.concat()** soma arrays
- **.slice(a,b)** fatia o array a: baseado na posição dos elementos citados, e b: ultima posição especificada não é contada
- **.sort()** deixa em ordem alfabética 
- **.sort((a,b) => a - b)** usado para ordenar de forma crescente ou .sort(function(a,b) => { return a - b})

# Laços de repetição:

- **For, While**;
- **For**: usamos quando temos uma quantidade definida de loops, *for(inicialização, enquanto/teste lógico, /o que o código deve fazer){}*;
ex: um incremento -> -> *for(let i = 0; i < array.length; i++){console.log(array[i])};* esse código faz uma iteração passando por todos os elementos de um array (iterar: executar repetidamente)
- **for in**: *for (var in array)* usado para ver os índices/valores 
- **for of**: *for (var array of array)* interação pelas propriedades
- **While:** usamos quando não sabemos a quantidades de loops a serem definidos, a variável de iteração é declarada fora do loop
- *while(condição){ código, incremento};*
- *do {código, incremento} while(condição);*
ex: 
    let array = [1, 2, 3, 4, 5, 6, 7];
    var i = 0;
    while(i < array.length){
        console.log(array[i]);
        i++
    };
- Nesse exemplo, assim como o do for, eu estou passando por cada elemento do array e imprimindo ele para ver seu elementos, se eu quisesse saber as posições bastava imprimir somente a váriavel de iteração i

# Condições:

- **If, Else, Else if, Switch**
- *if(condição){ true }* condição simples
- *if (condição){ true }else{ false };* condição composta
- *if(condição){ true }else if(condição2){ true }else{ false }* condição aninhada
- É possível colocar outros if e else if dentro de um if etc.
- *Switch()*{ 
    case1: 
        resultado que eu quero
        break
    case2:
        resultado que eu quero
        break
    default:  
        break
};
- No *case* colocamos os casos e suas respectivas condições, no *Default* colocamos um erro, caso as condições não sejam cumpridas
- O switch funciona de forma literal, igual ao tipo ===


# Eventos de tempo:

- Execução de código em intervalo de tempo
- **setTimeout(função, tempo em milisegundos)**: executado somente uma vez
- **setInterval(função, tempo em milisegundos)**: executa repetidamente em 
determinado intervalo
- **clearTimeout(), clearInterval()**: usado para parar esse evento de tempo, definimos eles a uma váriavel e colocamos essa váriavel dentro do clear
- 1000 = 1 segundo

# Classes:

- **Class**
- Herança baseada em protótipos
- Fábrica de objetos
- *constructor()* método para criação de objetos, baseado nos valores dentro dos parenteses
- *this* é usado para criar os atributos das classes
- Para criar um novo objeto é só fazer o seguinte: new nome da classe() dentro do parentese passo o atributo que quero adicionar entre aspas ""
ex:
    class Pessoa(){
        constructor(nome, idade){
            this.nome = nome; 
            this.idade = idade;
        }
    }
    const fulano = new Pessoa("Fulano", "45");

# DATAS e Manipúlações:

- **new Date()**: var.getHours(); -> pega a hora atual do pc
- **.getDay**: começa contar do domingo, por ser um array vai de 0 á 6
- **.getFullyear()**: pega o ano atual
- **.getMonth()**: pega o mês atual, array que vai de 0 - janeiro á 11 - dezembro
- **.getDate()**: pega os dias do mês, 1 á 31
- **.getHours()**: horas de 0 á 23
- **.getMinutes()**: minutos de 0 até 59
- **.getSeconds()**: 0 até 59
- **.getMilliseconds()**: 0 até 999
- **setDate, Hours etc(atributo, valor que deseja acrescentar)**: usado para acrescentar dias, horas, minutos, segundos etc
- **.tolocaleString()**: data do país para encurtar a impressão posso passar *{sateStyle/timeStyle:"short"}* dentro do parêntese para encurtar o valor
- Date.parse(data) converte para milisegundos *TODO: pesquisar, não entendi com funciona*

# Math:

- **.Math()**: cáculo matemático

# OBS:
- .value é usado para obter o valor de um input
- Declarar um input.value = ""; quer dizer que estou declarando para o input ser limpo
- Usar src dentro de aspas duplas necessita aspas simples
ex: "src = '' "
- A tag script vai no final do código HTML para indicar que o script pegue os respectivos elementos que o antecedem
- Comentários no JS são feitos com // para comentar linha e /**/ para comentar mais de uma linha
-  JS é fracamente tipado, então se vc somar "5" + 5 ele faz a correção e devolve 10, mas não é bom usar esse método pois pode conter erros de resultados
- JavaScript lê linha por linha durante a execução do código 
- **Null:** ausência de valor
- **NaN**: não é um número
- **Undefined**: variável não inicializada
- *console.table()*; imprimi em um formato de tabela
