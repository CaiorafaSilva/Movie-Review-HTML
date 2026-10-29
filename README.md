# 🎬 Movie Review Page

Página de resenha do filme **Onde os Fracos Não Têm Vez** (*No Country for Old Men*, 2007), feita apenas com **HTML**.

## 📚 Sobre o exercício

Este é um **exercício** do freeCodeCamp (*Design a Movie Review Page*), feito para praticar a estrutura de uma página com título, imagem, texto, nota em estrelas e lista de elenco, incluindo um cuidado de acessibilidade com o atributo `aria-hidden`.

## 🧱 Estrutura da página

```text
html (lang="en")
├── head
│   ├── meta charset="UTF-8"
│   ├── meta viewport
│   └── title: Movie Review
└── body
    └── main
        ├── h1: título da resenha
        ├── img: pôster do filme (com alt)
        ├── p: descrição do filme
        ├── p
        │   ├── b: "Movie Rating:"
        │   ├── span aria-hidden="true": 10 estrelas
        │   └── texto: (10/10)
        ├── h2: "Cast Members"
        └── ul
            └── li (8 itens): b (ator) + "as" + personagem
```

## 🏷️ Elementos e atributos utilizados

### Estrutura do documento

| Elemento / atributo | Para que serve |
| --- | --- |
| `<!DOCTYPE html>` | Declara que o documento é HTML5 |
| `<html lang="en">` | Raiz da página. O `lang` informa o idioma do conteúdo (inglês) a navegadores e leitores de tela |
| `<head>` | Informações sobre a página, que não aparecem na tela |
| `<meta charset="UTF-8">` | Codificação de caracteres, para exibir acentos e símbolos corretamente |
| `<meta name="viewport" ...>` | Faz a página se adaptar a telas de celular |
| `<title>` | Título exibido na aba do navegador |
| `<body>` | Todo o conteúdo visível da página |
| `<main>` | Conteúdo principal da página. Leitores de tela usam para pular direto ao conteúdo |

### Conteúdo

| Elemento / atributo | Para que serve |
| --- | --- |
| `<h1>` | Título principal da página |
| `<img src="..." alt="...">` | Pôster do filme. O `src` é o endereço da imagem e o `alt` é o texto alternativo para quem não vê a imagem |
| `<p>` | Parágrafos: a descrição do filme e a linha da nota |
| `<b>` | Negrito: o rótulo "Movie Rating:" e o nome de cada ator |
| `<span>` | Contêiner em linha, sem significado próprio. Aqui envolve só as estrelas, para poder receber um atributo |
| `aria-hidden="true"` | Esconde as estrelas dos leitores de tela (explicação abaixo) |
| `<h2>` | Título da seção "Cast Members" |
| `<ul>` | Lista não ordenada com o elenco |
| `<li>` | Cada item da lista, com um ator e seu personagem |

> 💡 O `<img>` é um elemento vazio: não tem tag de fechamento.

## ♿ Acessibilidade

- **`alt` na imagem:** descreve o pôster para quem usa leitor de tela ou quando a imagem não carrega.
- **`lang="en"`:** o leitor de tela escolhe a pronúncia correta para o texto em inglês.
- **`<main>`, `<h1>` e `<h2>`:** organizam a página e permitem navegar por seções.
- **`aria-hidden="true"` nas estrelas:** um leitor de tela leria cada emoji, um por um. Como o valor numérico já aparece em texto ao lado, as estrelas são só decoração visual.

```html
<p><b>Movie Rating:</b>
  <span aria-hidden="true">⭐⭐⭐⭐⭐⭐⭐⭐⭐☆</span> (10/10)
</p>
```

Com isso, quem usa leitor de tela ouve "Movie Rating" e o valor numérico, e quem enxerga continua vendo as estrelas.

## 📋 Elenco

| Ator | Personagem |
| --- | --- |
| Tommy Lee Jones | Ed Tom Bell |
| Javier Bardem | Anton Chigurh |
| Josh Brolin | Llewelyn Moss |
| Woody Harrelson | Carson Wells |
| Kelly Macdonald | Carla Jean Moss |
| Garret Dillahunt | Wendell |
| Tess Harper | Loretta Bell |
| Barry Corbin | Ellis |

Cada item segue este formato:

```html
<li><b>Tommy Lee Jones</b> as Ed Tom Bell</li>
```

## 💡 Conceitos praticados

- **Estrutura de uma página:** `html`, `head`, `body` e `main`.
- **Imagens:** `img` com `src` e `alt`.
- **Texto:** títulos (`h1`, `h2`), parágrafos (`p`) e negrito (`b`).
- **Contêiner genérico:** `span` para marcar só um trecho dentro de um parágrafo.
- **Acessibilidade básica:** `alt`, `lang` e `aria-hidden`.
- **Listas:** `ul` com vários `li`, cada um com conteúdo misto (elemento `b` + texto).

## ▶️ Como usar

1. Baixe ou clone este repositório.
2. Abra o arquivo `index.html` no navegador.

> ℹ️ A imagem é carregada de um endereço externo, então é preciso estar conectado à internet para ver o pôster.

## 🛠️ Tecnologias

- HTML5

## 👤 Autor

**Caio Rafael-dev**, estudante de Full Stack e InfoSec.