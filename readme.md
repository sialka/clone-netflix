# :fire: Clone do NETFLIX em REACT

_By Bonieky Lacerda_

> **https://www.youtube.com/watch?v=tBweoUiMsDg**



## Área de Destaque

![image1](C:\Users\cat\Desktop\Ap\NETFLIX\image1.png)



## Lista de Filmes e Séries

![image1](C:\Users\cat\Desktop\Ap\NETFLIX\image2.png)



## :pen: API - JSON - Test API

> **API para base de dados de filmes e séries**

-  [x] **https://www.themoviedb.org** 

> **Manipular JSON**

- [x] **http://jsonviewer.stack.hu** 

> **Testar Requisições**

- [x] **http://resttesttest.com** 

> **Ícones do Material-UI**

- [x] **https://material-ui.com/pt/components/material-icons/**



## :tv: Projeto

Esse projeto trata-se de uma simples reprodução do **NetFlix** para estudo de React, não contem todas as funcionalidades. 

Para a área de destaque e lista de filmes e séries foi usado a API do **themoviedb**.

### :paperclip: **1. Criando e Adicionando Ícones**

```bash
$ npx create-react-app netflixclone
$ cd netflixclone
$ npm install @material-ui/core @material-ui/icons
$ npm start
```

### :paperclip: **2. Estrutura de arquivos e pastas**

```bash
$ src
	$ components
		FeaturedMovie.css
		FeaturedMovie.js
		Header.css
		Header.js
		MovieRow.css
		MovieRow.js
	App.css
	App.js
	index.css
	index.js
	Tmdb.js
```

### :computer: App.js

A tela principal foi dividida em **03 componentes**: 

* Cabeçario - **<Header />**
* Destaque - **<FeaturedMovie />**
* Lista de Filmes e Séries - **<MovieRow />**



### :paperclip: ​Tmdb.js

Este arquivo contém a comunicação com a **API** do *themoviedb.org* que devolve um catalogo onde encontramos informações de filmes e séries.



### :paperclip: Header

Este componente serve apenas para compor a tela principal. Contem apenas o **logo** e **ícone** do usuário logado, não possui eventos.



### :paperclip: FeaturedMovie

Este componente é responsavel por mostrar um filme ou uma série em destaque. 

Informando: *pontuação*, *ano de lançamento*, *total de temporadas* e *uma breve descrição*.

Toda vez que a página é carregada muda o destaque.



### :paperclip: **MovieRow**

Este componente é responsavel por mostrar as listas de:

* Originais da netflix;
* Recomendados ***trending***;
* Em alta ***melhores votados - top rated***
* Ação
* Comédia
* Terror
* Romance
* Documentários

