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
> | :----------| :----------------------------------------------------|
> | gh-pages   | Produção publicada                                   |
> | master     | Versão estável - novos branchs pantem daqui          |
> | developer  | Ambiente de desenvolvimento de novas funcionalidades |


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

### Adicionando novos posts
E agora que você tem o ambiente todo configurado como adicionar novos posts?

Como utilizamos o [wintersmith][3] a adição de posts é bem simples, basta seguir os passos abaixo:
1- Se você nunca postou precisa criar seu arquivo de autor dentro da pasta */contents/authors/* na duvida pode usar o meu como exemplo:
```json
{
  "name": "Stark",
  "email": "stark@becogeek.com.br",
  "twitter": "https://twitter.com/stark_becogeek",
  "bio": "Idealizador do BecoGeek e um completo viciado em HQ's, CardGames, Vídeo Games, também conhecido como o macânico e funileiro do Beco Geek"
}
```
Este arquivo deve ser salvo como "nome-do-autor.json"

2- Dentro da pasta **contents** na raiz do projeto você vai encontrar a pasta **articles**, o primeiro passo é criar uma nova pasta que sera a urls do seu post, por exemplo:
```
/contents/articles/ola-becogeek/
```
3- Dentro dessa nova pasta você vai salvar todas as imagens que deseja utilizar em seu post, isso facilita muito na hora de referenciá-las no seu post.

4- Crie um arquivo **index.md** dentro da pasta do seu post é nele que você vai escrever o conteúdo, utilizando [Markdown][7] e/ou HTML, mas sempre de preferencia a Markdown, sério ela pode ser bem legal :)

Se preferir você pode utilizar um editor de Markdown, Stark recomenda o [StackEdit][8], mas existem várias outras opções, online, offline, mobile e desktop, eu particularmente uso muito o [StackEdit][8] e o [Sublime Text][9].

5- Nas primeiras linhas do seu novo arquivo index.md você precisa informar algumas coisas para o [wintersmith][3] entender o que você quer fazer :)

Veja um exemplo de cabeçalho:
```markdown
---
title: Titulo do Post
author: nome-do-arquivo-json-do-autor
date: 2014-04-05
template: article.jade
tags: readme, tutorial, passo-a-passo
---
``` 
Não se esqueça do ***---*** antes e depois das variáveis do post.

6- Escreva, escreva e escreva mais ;)

7- Para visualizar o resultado do post basta executar o preview que expliquei na configuração do ambiente.
```
wintersmith preview
```
E acessar a url do seu post e veja como ficou ^^

7- Faça o commit dos seus novos arquivos para o GitHub
> **Importante!**
> 
> **NUNCA** faça commit para os branchs de produção que são o master e o gh-pages, utilize o branch de developer ou crie um novo branch para você.
> Depois de postar entre em contato comigo para validar-mos o conteúdo e agendar a publicação :)
>
> Se você não esta familiarizado com essas tecnologias, ou ficou com alguma dúvida não pense duas vezes em me procurar stark@becogeek.com.br


[]'s

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
  [7]: http://daringfireball.net/projects/markdown/syntax "Documentação de Markdown Syntax"
  [8]: https://stackedit.io/ "StackEdit – markdown editor"
  [9]: http://www.sublimetext.com/ "Sublime Text: The text editor you'll fall in love with"