# beacademy-devstart-gitgithub

## EM DESENVOLVIMENTO

Este espaço é destinado a compartilhar comandos de produtividade usando GIT e GITHUB, esse repositório foi elaborado durante a imersão da DevtStart PayLivre organizada pela be.Academy, nosso primeiro desafio da semana, criar um repositório onde listaremos alguns comandos de produtividade nescessários para trabalhar com projetos.
Com isso optei em entregar um conteudo diferente, este repositorio será dedicado a quem está iniciando na programação, ou seja, terá um mini tutorial, um passo a passo para você já ir praticando no decorrer da leitura.

O sistema operacional utilizado: Debian - distro LINUX

No decorrer do turorial apenas o teminal será utilizado.

Caso você seja usuário Windows recomendo olhar a documentação do git.

[user windows](https://git-scm.com/download/win)
## Informações importante

[Documentação git](https://git-scm.com/)

<details>
<summary> O que é git?</summary>
  <br>

Antes de ser direto na resposta, o git surgiu de uma nescessidade, se você ja é familiarizado com os sistemas operacionais disponiveis no mercado como Microsoft, Apple, Android, Linux e outros, todos passaram por processos de desenvolvimento para se tornarem o que são hoje, varias frentes de desenvolvimento foram construidas para estruturar as funcionalidades disponiveis tanto para hadware como software, para que fosse possivel todas as equipes poderem trabalhar em conjunto organizando-se, dividindo tarefas, interligando cada parte desenvolvida separadamente, controlar melhorias e outras coisas que envolvem esses processos, outras ferramentas eram nescessárias para organizar isso tudo.

O GIT é um sistema de versionamento, foi desenvolvido pelo próprio idealizador do LINUX, **Linus Torvalds** durante o desenvolvimento do KERNEL(nucleo) do LINUX em conjunto com outros desenvolvedores, na época,surgiram vários softwares que prometiam agilizar os processos dentro desses times de desenvolvimento, essas ferramentas eram conhecidas como software proprietários, ou seja, se pagava pelo uso, e muitos desses softwares acabavam sendo descontinuados, não recebiam atualizações, cancelavam assinaturas e por ai vai, uma caos total para as equipes de desenvolvimento.

Então o próprio Linus Torvalds depois de ter feito engenharia reversa no sistema de controle usado na época, uma tentativa de pedir ajuda a quem estivesse monitorando o uso do sistema em algum lugar, ele e sua equipe iniciaram o desenvolviento de um sistema que fosse melhor e que suprisse as nescessidades do time de desnvovlimento.

>De qualquer forma, os SCVs que olhei dificultam as coisas. Uma delas (a maior delas, na verdade) que estive trabalhando é fazer este processo ser realmente eficiente. Se leva meio minuto para aplicar um patch e ainda lembrar o que mudou, etc (e francamente, isso é rápido para a maioria dos SCVs por aí para um projeto do tamanho do Linux), daí uma série de 250 e-mails (que não é estranho acontecer quando eu sincronizo com o Andrew, por exemplo) demora duas horas. Se um dos patches no meio do processo não é aplicado, as coisas ficam realmente muito feias.
>
>Agora, o BK (BitKeeper) não era um inferno também (na verdade, comparado com todo o resto, o BK é um inferno em velocidade, geralmente em uma ou duas ordens de magnitude), e levou cerca de 10-15 segundos por e-mail quando mesclei meus arquivos com o Andrew. MESMO ASSIM, com o BK isso não era um problema tão grande, visto que mesclas de arquivos de BK←>BK eram tão fáceis, eu nunca precisei das lentas mesclas por e-mail com nenhum dos outros desenvolvedores principais. Então um "mesclador" de um SCV baseado em patches precisaria ser realmente mais rápido que o BK. O que realmente é extremamente difícil.
>
>Então eu estou escrevendo alguns scripts para tentar alinhar tudo mais rápido. Indicações iniciais são de que eu poderei fazer isso tão rápido quanto eu aplico patches, mas para ser franco, estou no máximo com metade pronto, e se eu estiver na direção errada, talvez essa não seja a mais pura verdade. De qualquer forma, a razão de que eu consigo criar tudo isso tão rápido é que meus scripts não serão um SCV, serão tipo um "registro de estado do Linus" bem específico. Isso vai fazer minhas mesclas lineares de patches muito mais eficientes no tempo, e nestas condições, possível.
>
>(Se a aplicação de um patch demora três segundos, até mesmo uma série grande de patches não é um problema: se eu for notificado em um minuto ou dois que falhou na metade do caminho, sem problemas, eu posso então simplesmente arrumar manualmente. É por isso que a latência é crítica - se eu tivesse que fazer as coisas efetivamente "desconectado", eu não poderia, por definição, arrumar as coisas quando problemas aparecessem).
  
</details>

[Repoditório github](https://github.com)

<details>
  
<summary> O que é github? </summary>
  <br>
  
É dificil definir o que se tornou o github, mas de fato é definida como uma platforma de trabalho para qualquer um com conexão a internet e que precise guardar seus projetos e compartilha-los com o mundo, github tembém é conhecida como repositório, já que a mesma armazena uma serie de coisas.
  
Uma plataforma para times criarem seus projetos emm um unico lugar, a plataforma possui inumeras ferramentas para produção, aprendizagem, monitoramento, também é usada como uma rede social para desenvolvedores enfim é um montão de coisa juntas.
</details>

## Recursos usados

- Coputador com sitema operacional **Debian** 

- Terminal Bash

- Git

- Github


## Mini-Tutorial

>**Downloard Git**
- [Baixar Git](https://git-scm.com/downloads)

  Não tem segredo, é só abrir a pasta de dowloard em sua maquina apos baixar, clicar no executavél e seguir clicando em next.

> Abra seu terminal: CMD,PROMPT, BASH, ETC...

- Como saber se a instalação foi bem sucedida?
```bash
    git --version
```
> Configuração do git
Este passo é para configurarmos o Git, é preciso informar ao git quem está operando o sistema.

- Passamos o nosso nome de usuário

```bash
    git config --global user.name = 'nome_usuario'
```
- Passamos o nosso e-mail principal

```bash
    git config --global user.email = 'meu_email@exemplo.com'
```
Agora toda vez que usarmos o git, ele registrarar o usuário que estava operando.

```bash
    git config --global user.email = 'meu_email@exemplo.com'
```
> Caso queira explorar os comando do git basta digitar em seu terminal.```git```

O terminal listará varios comandos relacionados ao git

```
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone             Clone a repository into a new directory
   init              Create an empty Git repository or reinitialize an existing one

...

```
> Lista de alguns comandos mais usados

- [x] ```git init``` : Cria um repositório Git vazio ou reinicializa um existente

Para esse comando é preciso criar uma pasta ou ter uma com arquivos do projeto, terá que abrir essa pasta no termminal e depois é só digitar esse comando. Uma Vez iniciado o repositorio não precisa passar o mesmo commando init na mesma pasta.

```
neres@debian:~/Documentos/development/teste$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint: 
hint: 	git config --global init.defaultBranch <name>
hint: 
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint: 
hint: 	git branch -m <name>
Initialized empty Git repository in /home/neres/Documentos/development/teste/.git/

```

- [x] ```git status``` : Mostra o status da árvore de trabalho.

Seguinte mensagem deve aparecer caso tenha alguma alteração no repositório.

```
On branch main
Your branch is behind 'origin/main' by 1 commit, and can be fast-forwarded.
  (use "git pull" to update your local branch)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```
- [x] ```git add .``` : Adiciona todos os conteúdos do arquivo ao índice.
- [x] ```git add nome_diretorio``` : Adiciona um diretorio em especifico ao índice.
- [x] ```git add nome_arquivo.txt``` : Adiciona um arquivo em especifico ao índice.

> ***Branch : Lista, cria ou exclui branches***
> Atenção, o git como monitora tudo que é feito quando se cria o repositorio, ele cria pontos que lingam a cada nova alteração feita no projeto, geralmente cada projeto e dividido em varias frentes de trabalho onde existe o projeto principal e suas copias que chamamos de filhos, e que esses compões o projeto.
> Como a prática você entenderá seu funcionamento.
> ![branch](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQVxS88B_YU0CueV2bv_34pDmdPXv3RCJgB0A&usqp=CAU)


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/neresfabio)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/fabioneresdejesus/)

## Referência

 - [O que é git](https://pt.wikipedia.org/wiki/Git)
 - [O que é github](https://www.hostinger.com.br/tutoriais/o-que-github)
