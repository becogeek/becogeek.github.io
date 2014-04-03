![BecoGeek][1]


[Beco Geek][2] é o mais novo portal para o mundo Geek 

----------


## Para nossa equipe
###Primeiros passos ;)

O **Beco Geek** é desenvolvido com [wintersmith][3], um gerador de conteúdo estático desenvolvido em coffeescript, utilizamos principalmente markdown para os posts, jade para os templates e javascript ou cofeescript para automações, o site encontra-se hospedado no GitHub Pages.

> **Importante!**
> 
> Se muito cuidado com seus commits, certifique-se de estar trabalhando no branch correto, os branchs são nossa principal organização de ambientes!
> Abaixo você encontra a atual lista de branchs:
>
> | Branch     | Finalidade                                           |
> | :----------| ----------------------------------------------------:|
> | gh-pages   | Produção publicada                                   |
> | master     | Versão estável - novos branchs pantem daqui          |
> | developer  | Ambiente de desenvolvimento de novas funcionalidades |
>
> Se você não esta familiarizado com essas tecnologias, não pense duas vezes em me procurar stark@becogeek.com.br

### O que fazer depois de baixar o projeto
> Todos os comandos abaixo devem ser executados no terminal, se você usa windows é melhor que abra o terminal como **administrador** se usa linux ou mac pode precisar usar **sudo** em alguns comandos.

1- Certifique-se de ter no [node.js][4] instalado na sua máquina.
2- Instale o [wintersmith][3] via pelo npm:
```
npm install -g wintersmith
```
3- Entre na pasta do projeto e baixe as dependências:
```
npm install
```
Isso vai criar uma pasta **node_modules** dentro do seu projeto, o github já esta configurado para não sincronizar esta pasta
4- Teste se esta tudo funcionando ligue o modo preview
```
wintersmith preview
```
Depois de executar este comando acesse [localhost:8080][5], se o site abrir normalmente, parabéns deu tudo certo **:)**

[]'s

--
**Stark** <br/>
Mecânico e Funileiro no BecoGeek <br/>
stark@becogeek.com.br <br/>
[@Stark_BecoGeek][6]



  [1]: http://imagizer.imageshack.us/a/img856/3841/qlrp.png 
  [2]: http://becogeek.com.br/ "Acesse o BecoGeek"
  [3]: http://wintersmith.io/ "Home page oficial do Wintersmith"
  [4]: http://nodejs.org/ "Install node.js"
  [5]: http://localhost:8080 "Preview"
  [6]: http://twitter.com/stark_becogeek/ "Twitter @Stark_BecoGeek"
