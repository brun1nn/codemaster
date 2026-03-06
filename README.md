# Projeto CodeMaster DEV

## Estado Inicial🏗️

#### Ao abrir o arquivo, é notável o uso de HTML e CSS para a criação do site, mas apenas isso. Minha missão é criar uma base back-end e front-end afim de mudar o site por completo, dando-lhe vida, movimento e cérebro. E pra isso preciso identificar/analisar o que devo fazer com os recursos que possuo.

## Ponto de vista💭

#### Dando uma olhada mais afundo no site, percebo que o mesmo deve ser aprimorado nos seguintes aspectos e componentes:

- Seção **sobre/about** vazia;

- Ferramenta para trocar o modo de tela entre **Dark-Mode** e **Light-Mode** infuncionável;

- Fundo vazio que carece de elementos visuais;

- **Carroussel/Slider** com falta de **script/JS** em relação à intercalação entre as imagens presentes no mesmo;

- **Menu hambúrguer** para *mobile* com falta de **script/JS** em relação à abertura e fechamento do mesmo.

## Tarefas a serem feitas📋

#### Diferentemente da minha análise pessoal de *problemas* do site, foi me passado os seguintes pontos a serem consertado/implementados:

1. Menu Mobile✔️
2. Links Ativos✔️
3. Formulário com API✔️
4. Animação de Scroll✔️

---

> “Não é a linguagem de programação que define o programador, mas sim sua lógica.” 
> - David Ribeiro Guilherme

---

#### Resumo das alterações/aprimoramentos📖

#### Firstly, devo começar com o ***Menu Mobile***. Coloquei um `EventListener` para ser possível a abertura e fechamento do menu, adicionei um `overflow` ao navList, afim de bloquear o scroll quando o menu estiver aberto, outro `EventListener` foi introduzido agora afim de fechar o menu quando quaisquer um dos links presentes forem clicados, também foi necessário outro `EventListener` para fechar o menu ao rolar a página.

#### Já na ***navegação ativa*** foi colocado um `function activeLink` para adicionar o status de 'ativo' ao link clicado e podemos ver como isso se comporta juntamente com `.navlist a` no CSS que modifica o estilo dos links 'ativos'.

#### Falarei de ***modo claro e escuro*** agora, nesta parte foi adicionada ao código uma `function toggleMode` que serve para adicionar uma função diretamente conectada à troca entre o Modo Claro e Escuro. Juntamente disso, `localStorage` foi um complelementar ajudando a salvar a opção Light ou Dark no armazenamento local do navegador do computador acessador.

#### Sobre a ***animação do título*** foi adicionado outra `function` junto de alguns `if's` para possibilitar uma animação de fade-in e fade-out além de ter sua cor mudada, principalmente sendo permitido por `index < text.legth` e `isTyping = true/false` que identifica quando a ação de surgir acaba para começar a outra ação, que é de apagar.

#### Outro detalhe é a ***animação da seção home*** que possui o `section.style.transition` junto de `opacity 1s` e `transform 1s`. Além disso as outras ***seções*** não ficam por fora, também possuindo `scale`, `rotateY`, `translateY` e etc.

#### Um plus adicional, foi o ***botão de voltar ao topo*** localizado no canto inferior direito que fica disponível logo após alcançar o fim da página, sendo caracterizado por `window.scrollTo - *top*`.

#### O ***carrossel de projetos*** foi marcado por `functions` para realizar quase todo tipo de atividade desejada, ir para o próximo, voltar para o último e etc.

#### O ***formulário de contato*** é definido por alguns códigos como `EventListener` para o envio do forms, `fetch` para enviar dados por API e um `alert` caso o usuário tenha feito algo 'indesejado'

#### O último mas não menos importante é a ***animação da seção "sobre mim"***, também com uma animação fade-in, esta seção é reconstituída por uma `function` para redirecioná-la ao centro da tela e um `if` para caso a seção esteja dentro da tela ela de exibição ela ficaria vísivel.

#### **Estas foram as mudanças feitas por cima da lista de tarefas requisitadas.**