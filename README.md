# logica-de-programacao-web
Trata-se de um repositório onde o principal objetivo é servir de armazenamento de informação relacionadas a conteúdo de html , css e javascript.  

Este curso é uma regravação do primeiro curso de Lógica.

Com uma didática diferente e mais de 100 exercícios, deixamos o treinamento ainda melhor!

Se você está iniciando agora, seja bem-vindo ao treinamento Lógica de Programação I , porta de entrada no mundo da programação.

Caso você já tenha feito o curso antigo, esta é uma boa hora de revisar os conceitos aprendidos e exercitar seus conhecimentos com novos exercícios.

Sucesso e bom estudo para todos!

--------------------------------------------------------------------------------------------------------------------------------------------------

Olá!

Este exercício obrigatório lhe poupará muita dor de cabeça ao longo do curso. Vamos lá?!

Qual editor de texto usar?
Você pode usar qualquer editor de texto simples que já venha com seu sistema operacional, exceto o do Windows. Se você é usuário do Windows é recomendável utilizar outros editores de texto. Contudo, antes de disponibilizar o link (endereço) para que eles sejam baixados, ressalto a importância de seguir as instruções de instalação de ambos. Primeiro, é baixar o programa, executá-lo e, depois, seguir o assistente até o fim sem alterar qualquer configuração.

1 - Sublime: é o editor utilizado durante o treinamento. É interessante usá-lo para obter paridade visual ao longo do curso, mas não é obrigatório. Para baixá-lo clique aqui e na tela de download que aparecer escolha a versão para Windows.

2 - Notepad++: existe apenas para Windows é uma alternativa interessante ao Sublime. Você pode baixá-lo clicando aqui.

Caso o sistema operacional utilizado seja Linux ou MAC, pode-se usar o editor de texto padrão ou baixar o Sublime, que por ser multiplataforma tem versões para Windows, Linux e MAC.

Qual navegador utilizar?
É possível usar qualquer navegador que tenha um depurador (debugger). Contudo, é fortemente recomendável que o Chrome seja utilizado, justamente, para obter paridade visual com o instrutor ao longo do treinamento. Caso não se tenha o Chrome, baixe aqui e siga as instruções de instalação até o fim.

A partir da versão 68 do Google Chrome esta paridade não ocorre, pois o menu de barra de tarefas e as ferramentas de desenvolvedor foram removidas do layout do browser.

Portanto, torna-se necessário o emprego dos comandos "CTRL+O" para abrir o arquivo HTML, quando necessário, e F12 para abrir a janela das ferramentas de desenvolvedor (DevTools). Este recurso irá abrir em uma nova janela para utilização de depurador e demais utilidades.

Estes comandos serão reiterados nas transcrições dos próximos videos.

Agora vamos começar os estudos de lógica de programação!

------------------------------------------------------------------------------------------------------------------------------------------------------------------

O Chrome, a partir da versão 55, passou a detectar automaticamente o encoding dos arquivos. Então, é possível pensar que não é mais necessária a tag <meta charset="UTF-8">.

No entanto, ela deve continuar a ser usada, porque nem todos os navegadores detectam o encoding automaticamente, sendo assim, é uma boa prática manter a tag <meta> indicando o charset usado na hora de criar o arquivo.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Quando começamos a programar é comum ocorrer uma explosão de arquivos e cada arquivo equivale a um programa. Se salvarmos cada um dos arquivos diretamente na área de trabalho teremos todos eles espalhados. Você vai querer perder aquele código todo especial que fez porque apagou um arquivo por engano?

É por isso que um dos primeiros pedidos do curso foi para criar a pasta "logica". Ela servirá para armazenar todos os arquivos que forem criados ao longo do treinamento. Programar requer disciplina e organização e por mais simples que seja esse ato, é o mínimo que podemos fazer para termos um ambiente organizado.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

Extensão de arquivos

Você já utilizou um processador de texto ou planilha? Por exemplo, arquivos do Microsoft Word possuem a extensão .doc ou .docx. Assim, caso você tenha salvo um arquivo chamado "receitas", dentro do computador ele será "receitas.docx". A mesma coisa serve para as planilhas do Excel, por exemplo, uma planilha chamada "custos" quando salva no computador agrega a extensão .xls, sendo assim, o nome completo do arquivo é custos.xls.

A extensão do arquivo é importante, pois confere ao Sistema Operacional uma pista de qual programa deve ser usado para abrir o arquivo em questão. Assim, todo arquivo que criarmos até o final do curso utilizará a extensão .html.

Convenção (sendo politicamente correto)

Assim como o condomínio de um prédio possui uma convenção, o mundo da programação é repleto delas. Por exemplo, uma convenção muito utilizada é criar arquivos com letras minúsculas e se houver mais de uma palavra usamos um "_" como separador. Além disso, não usamos acentos no nome dos arquivos. É claro que, assim como a convenção de um condomínio pode não ser seguida, nada impede que o programador crie o arquivo do jeito que quiser. E, da mesma forma que um morador que comete infrações não será bem visto pelos demais condôminos, o mesmo ocorre com o programador.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------

Quando salvamos um arquivo texto no disco ele é salvo usando uma cadeia de caracteres (character set encoding). Se no editor de texto salvamos o arquivo contendo charset UTF-8, precisamos dar uma pista para o navegador de como ele deve ser processado. Se não fizermos isso, ele não conseguirá exibir corretamente qualquer texto acentuado.

Contudo, muito cuidado! Vamos supor que acidentalmente seu editor de texto não salvou o arquivo como UTF-8, mas em latin1. Se colocarmos a tag <meta charset="UTF-8"> estaremos dando uma dica errada para o navegador e isso nos trará problemas na acentuação. Para resolver esse tipo de situação, podemos usar <meta charset="latin"> ou mudar nosso arquivo para UTF-8, o que é mais difícil.

Pode ser que o editor de texto escolhido não siga o padrão UTF e utilize outro qualquer que nem eu ou você sabemos.

Mais do que os caracteres saírem certos ou errados, o importante é aprender a lógica de programação. O que estamos abordando serve para tornar sua experiência melhor e seu programa mais bonito. Afinal, quem não gosta de ver os acentos todos bonitinhos? :)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------

Para você avançar no treinamento com passos firmes, precisamos consolidar bem nosso conhecimento sobre alguns processos. Sendo assim, nada mais indicado do que praticar. Vamos criar um programa simples que talvez não faça muita coisa, mas é a base necessária para nossa evolução.

1 - Crie o arquivo texto_puro.html em seu editor de texto favorito salvando-o dentro da pasta logica. Depois, escreva o seguinte texto dentro deste arquivo (inclusive você pode copiar os dois parágrafos abaixo e colá-los dentro do arquivo):

A convenção que usaremos para criar nosso programa é adotar letras minúsculas e não usar acentos e, claro, usar a extensão .html.

Outro ponto importante é que toda alteração feita no arquivo .html deve ser salva e, além disso, o navegador precisa recarregar a página para que a última alteração do arquivo entre em vigor.COPIAR CÓDIGO
2 - Agora que você tem o arquivo texto_puro.html criado dentro da pasta logica abra-o em seu navegador. Por exemplo, se você esta usando o Chrome, vá até o menu "Arquivo -> Abrir arquivo ..." se sua versão do Google Chrome não possui mais o menu utilize o atalho CTRL + O. O navegador solicitará que você escolha qual arquivo deseja abrir. Selecione o arquivo texto_puro.html que criamos. Este procedimento será repetido diversas vezes ao longo do treinamento, por isso, revisá-lo é importante.

Quando o arquivo for aberto, o navegador irá interpretar cada linha que você escreveu nele exibindo o conteúdo. Contudo, veja na prática que os acentos não são exibidos corretamente e que não houve pulo de linha entre um parágrafo e outro.

3 - Com base no que aprendeu neste capítulo, altere o arquivo para que ele exiba corretamente a acentuação e pule uma linha.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Este exercício é mais reflexivo que prático e abordará a linguagem HTML e o conteúdo estático.

Apesar da maneira como é escrito, o HTML não é uma linguagem de programação propriamente dita. Inclusive, veja que em seu nome (Hyper Text Markup Language) não há a presença da palavra "programming". O HTML foi criado apenas para apresentar informações, isto é, sem dinamismo. Por exemplo, temos o seguinte código:

<h1>Sejam bem-vindos</h1>
<br>
Seria isso um programa?COPIAR CÓDIGO
E se quisermos fazer cálculos que variam de acordo com a entrada do usuário? Não podemos, pois o HTML no máximo será o responsável em exibir o resultado do cálculo, mas não realizá-lo.

Mas, o navegador não é bobo, ele conhece além da linguagem HTML outra que é totalmente dinâmica. Esta linguagem chama-se JavaScript. Com ela podemos realizar cálculos e diversas operações úteis. Mas, você pode estar se perguntando: deixaremos de usar o HTML? Não! É claro que não! Usaremos HTML e JavaScript para criar programas interessantes, portanto, não se preocupe como isso será feito.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Olá!

Este exercício obrigatório lhe poupará muita dor de cabeça ao longo do curso. Vamos lá?!

Qual editor de texto usar?
Você pode usar qualquer editor de texto simples que já venha com seu sistema operacional, exceto o do Windows. Se você é usuário do Windows é recomendável utilizar outros editores de texto. Contudo, antes de disponibilizar o link (endereço) para que eles sejam baixados, ressalto a importância de seguir as instruções de instalação de ambos. Primeiro, é baixar o programa, executá-lo e, depois, seguir o assistente até o fim sem alterar qualquer configuração.

1 - Sublime: é o editor utilizado durante o treinamento. É interessante usá-lo para obter paridade visual ao longo do curso, mas não é obrigatório. Para baixá-lo clique aqui e na tela de download que aparecer escolha a versão para Windows.

2 - Notepad++: existe apenas para Windows é uma alternativa interessante ao Sublime. Você pode baixá-lo clicando aqui.

Caso o sistema operacional utilizado seja Linux ou MAC, pode-se usar o editor de texto padrão ou baixar o Sublime, que por ser multiplataforma tem versões para Windows, Linux e MAC.

Qual navegador utilizar?
É possível usar qualquer navegador que tenha um depurador (debugger). Contudo, é fortemente recomendável que o Chrome seja utilizado, justamente, para obter paridade visual com o instrutor ao longo do treinamento. Caso não se tenha o Chrome, baixe aqui e siga as instruções de instalação até o fim.

A partir da versão 68 do Google Chrome esta paridade não ocorre, pois o menu de barra de tarefas e as ferramentas de desenvolvedor foram removidas do layout do browser.

Portanto, torna-se necessário o emprego dos comandos "CTRL+O" para abrir o arquivo HTML, quando necessário, e F12 para abrir a janela das ferramentas de desenvolvedor (DevTools). Este recurso irá abrir em uma nova janela para utilização de depurador e demais utilidades.

Estes comandos serão reiterados nas transcrições dos próximos videos.

Agora vamos começar os estudos de lógica de programação!

---------------------------------------------------------------------------------------------------------------------------------------------------------------------


Toda linguagem de programação possui ferramentas que nos auxiliam a descobrir o que há de errado com o código, principalmente no que diz respeito a erros de sintaxe, aquele tipo de erro que ocorre quando deixamos de seguir regras que a linguagem de programação utiliza.

Vejamos o seguinte código escrito por Tio Ben:

<meta charset="UTF-8">
<script>
    alert("Isso");
    alert("é");
    alert("um");
    alert("programa);
    alert("sim");
</script>COPIAR CÓDIGO
Apesar de Tio Ben jurar que verificou o código mil vezes, nada de errado é encontrado. Ajude Tio Ben a identificar o local no qual ele cometeu um erro de sintaxe. DICA: experimente criar o programa tio_ben.html e cole nele o código acima. Rode e peça ajuda do depurador (debugger), o melhor amigo do programador na busca de erros.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

O programa de Penelope está assim:

<meta charset="UTF-8">

<script>
</script>

alert("Olá, este é meu primeiro programa!");
alert("Gostaram?");COPIAR CÓDIGO
As duas instruções alert são feitas fora do mundo JavaScript, ou seja, estão sendo feitas fora da TAG <script>..</script>. Isso faz com que o HTML entenda as instruções como texto comum exibindo-as no navegador.

Para resolver esse problema, basta mover as duas instruções para dentro da TAG script, ou seja, elas serão parte do conteúdo da TAG. Alterando teremos:

<meta charset="UTF-8">
<script>
    alert("Olá, este é meu primeiro programa!");
    alert("Gostaram?");
</script>COPIAR CÓDIGO
Agora, os dois alertas são exibidos como pop up e assim a página é carregada.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------


