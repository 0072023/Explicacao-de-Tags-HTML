<!DOCTYPE html>
<html lang="pt-BR"> <!--é um atributo global do HTML que define o idioma de um elemento ou de uma página inteira. 
-->

<head>
    <!--<meta charset="UTF-8"> é uma codificação de caracteres que inclui quase todos os caracteres de todos os sistemas de escrita do mundo-->
    <!--<meta name="viewport" content="width=device-width, initial-scale=1.0">. Esta meta tag viewport fornece ao navegador instruções sobre como controlar o dimensionamento da página quando acessada de diferentes tamanhos de dispositivos.-->
    <!--<meta name="description">serve para resumir o conteúdo de uma página e aparecer nos resultados de pesquisa do Google. -->
    <!--<link rel  é utilizado para conectar arquivos -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="explicando sobre tags">
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <h2 align="center">
        <marquee behavior="alternate" scrollamount="16">Utilizando Listas</marquee>
    </h2>
    <hr size="6" color="#000">
    <!--A tag <ol> é responsavel pela criacao de listas ordenadas -->
    <!--<li> representa as linhas-->
    <!--<ol type="I" significa que esta em numeros romanos, type="A" em ordem alfabetica-->
    <ol>Lista Ordenada
        <li>United States</li>
        <li>China</li>
        <li>Russia</li>
    </ol>
    <ol type="I">Lista Ordenada em numeros Romanos
        <li>Primeiro</li>
        <li>Segundo</li>
        <li>Terceiro</li>
    </ol>
    <ol type="A">Lista Ordenada em Ordem Alfabetica
        <li>Artificial</li>
        <li>Bug</li>
        <li>Comando</li>
    </ol>
    <hr size="6" color="#000">
    <!--<ul> é uma lista que nao se importa com ordem, ao inves disso ela tem marcadores que podem ser usados de varias
            maneiras utilizando o atributo type="circle", type="square"-->
    <ul>Lista Nao Ordenada
        <li>Apple</li>
        <li>Microsoft</li>
        <li>Nvidia</li>
    </ul>
    <ul type="circle">Lista Nao Ordenada em Circulo
        <li>Alan Turing</li>
        <li>Dennis Richie</li>
        <li>Andrew S. Tanenbaun</li>
    </ul>
    <ul type="square">Lista Nao Ordenada em Quadrado
        <li>Marvel</li>
        <li>DC</li>
        <li>Amazon</li>
    </ul>
    <hr size="6" color="#000">
    <!--<dl> Pode ser associado como um titulo de uma serie de questoes e <dt> como o titulo da questao. E para ser bem especifico <dd> como a definicao do <dt> -->
    <dl align="center">
        <marquee behavior="scroll" scrollamount="14">Lista de Definicao</marquee>
    </dl>
    <dt>O Que é HTML:</dt>
    <dd> (HyperText Markup Language) é uma linguagem de marcação que define a estrutura e o significado do conteúdo web.
        É o componente básico da web, permitindo a construção de websites e a inserção de novos conteúdos, como imagens
        e vídeos, através de hipertextos.</dd>
    <dt>O Que é CSS:</dt>
    <dd>(Cascading Style Sheet) e é usado para estilizar elementos escritos em uma linguagem de marcação como HTML.</dd>
    <hr size="6" color="#000">
    <!--Uma simples demonstracao de listas integradas-->
    <ol>
        <li>Aparelhos</li>
        <ul>
            <li>Smartphone</li>
            <li>Notebook</li>
        </ul>
        <li>Carros</li>
        <ul>
            <li>BMW</li>
            <li>AUDI</li>
        </ul>
    </ol>

    <hr size="6" color="#000">
    <h1 align="center">
        <marquee direction="down" width="240" height="70" behavior="alternate" style="border:solid">FORMULARIOS
        </marquee>
    </h1>
    <hr size="6" color="#000">
    <!--<form> Cria um bloco para agrupar as tags de formulário e os seus dados. -->
    <!--<label> é um elemento que representa um rótulo ou legenda para um item de interface do usuário.-->
    <!--O atributo (action) define o local onde os dados de um formulário devem ser enviados, ou seja, a URL para a qual o conteúdo do formulário será submetido.-->
    <!--O atributo (method) especifica o método HTTP a ser usado para enviar os dados de um formulário. Os métodos mais comuns são GET e POST.-->
    <!--<for> Cria um link entre a label e o input. O for deve apontar para o ID do input-->
    <!--O atributo (name) serve para ser identificado-->
    <!--(ID) Serve para identificado de forma unica-->
    <!--(Type) Pode ser usado para definir texto e numeros(number) ou (text)-->
    <!--(maxlength) E (min) indica a quantidade maxima ou minima de caracteres permitidos-->
    <!--(required) Significa que e obrigatorio preencher aquela secao-->
    <!--<Select> Permite ao usuário escolher uma ou mais opções a partir de um menu-->
    <!--<option> Representa uma opção dentro de um menu de opções, que é criado pelo elemento <select>-->
    <!--(value)  Usado para especificar o valor de um input ou botão quando ele é selecionado-->
    <form name="login" action="#" method="post">
        <label for="name">NOME:</label>
        <input type="text" name="nome" id="nome" size="40" placeholder="Usuario" required>
        <br>
        <label for="senha">SENHA:</label>
        <input type="password" name="senha" id="senha" size="40" maxlenght="15" required placeholder="Senha">
        <br>
        <label for="idade">.IDADE:</label>
        <input type="number" name="idade" id="idade" size="40" step="1" min="0" max="150" placeholder="19">
        <br>
        <label for="nacionalidade">NACIONALIDADE</label>
        <br>
        <select for="nacionalidade" id="nacionalidade">
            <option value="br">brasileiro(a)</option>
            <option value="in">ingles(a)</option>
            <option value="am">americano(a)</option>
            <option value="al">alemao(a)</option>
        </select>
        <hr size="6" color="#000">
        <!--(Checkbox) E uma opcao em que pode ser selecionada as duas opcoes e (radio) apenas uma-->
        <!--(msg) e (textarea) E uma area reservada para escrever mensagens-->
        <!--(rown) seria praticamente a quantidade de linhas enquanto (cols) seria a quantidade de colunas (ex 1111=2cols)-->
        <!--Submit e o mesmo que enviar para outro endereco as informacoes armazenadas-->
        <h3>Transporte</h3>
        <label for="carro">CARRO</label>
        <input type="checkbox" name="carro" id="carro" value="car">
        <label for="moto">MOTO</label>
        <input type="checkbox" name="moto" id="moto" value="moto">
        <label for="bike">BICICLETA</label>
        <input type="checkbox" name="bike" id="bike" value="bike">
        <br>
        <h3>Sexo</h3>
        <label for="masc">Masculino</label>
        <input type="radio" name="sexo" id="masc" value="m">
        <label for="fem">Feminino</label>
        <input type="radio" name="sexo" id="fem" value="f">
        <br>
        <label for="msg">Caixa de Mensagens</label>
        <br>
        <textarea name="msg" id="msg" rows="5" cols="50" placeholder="ESCREVA SUA MENSAGEM AQUI!"></textarea>
        <br>
        <input type="submit" name="enviar" value="enviar">
    </form>
</body>

</html>
