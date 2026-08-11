# ☕ Café Aroma & Cia — Exercício Prático de CSS / SASS

![Bolsa Futuro Digital](https://img.shields.io/badge/Curso-Bolsa%20Futuro%20Digital-482715?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![SASS](https://img.shields.io/badge/SASS-CC6699?style=for-the-badge&logo=sass&logoColor=white)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-003603?style=for-the-badge)

Projeto prático desenvolvido para o curso de **Front-End da Bolsa Futuro Digital** (Semana 10).

> 💡 **Nota Importante**: 
> - O projeto foi desenvolvido a partir de um **HTML pronto**, fornecido previamente pelas instruções do exercício.
> - Na folha de estilos (`estilo.css`), foi utilizada a **estrutura/sintaxe de aninhamento no estilo SASS** (CSS Nesting com pseudo-seletores como `&:hover`), facilitando a organização das regras para elementos-filhos de navegação e componentes.

---

## 📋 Sobre o Projeto

O **Café Aroma & Cia** é uma landing page para uma cafeteria artesanal. Partindo do código HTML base disponibilizado pela aula, realizou-se a estilização completa da página, que conta com apresentação da marca, cardápio formatado em tabela, seção de depoimentos de clientes e um formulário para reserva de mesas.

---

## 🎯 Requisitos Cumpridos (Baseados no PDF do Exercício)

### 📌 1. Análise da Estrutura HTML Fornecida
Estudo e mapeamento das seções semânticas do `index.html`:
- `<header>` e `<nav>` com links âncora (`#sobre`, `#cardapio`, `#depoimentos`, `#reservas`).
- `<section>` "Sobre o café" com imagem descritiva (`alt`).
- `<table>` de cardápio com `<thead>`, `<tbody>` e alinhamento de preços.
- `<ul>` com depoimentos e citações de clientes fictícios.
- `<form>` de reserva com inputs (`text`, `email`, `date`, `number`) e botão de envio.
- `<footer>` com dados de endereço e contato.

### 📌 2. Estilização com CSS & Estrutura SASS (Parte A — Base)
- [x] **Arquivo Externo**: Folha de estilos `estilo.css` desacoplada e vinculada via `<link rel="stylesheet">` (sem CSS inline ou `<style>` interno).
- [x] **Bloco `:root` com Variáveis CSS**: Declaração de variáveis globais para paleta de cores (tons de café e detalhes em verde), espaçamentos e fontes:
  ```css
  :root {
      --cor-primaria: #482715;
      --cor-secundaria: #fdf2d8;
      --cor-destaque: #003603;
      --spacing-root: clamp(1rem, 5vw, 3rem);
      --title-font: "Nunito", sans-serif;
      --secondary-font: "Comfortaa", sans-serif;
      --border-radius: 10px;
      --box-shadow: 0 8px 25px rgba(0, 0, 0, .12);
  }
  ```
- [x] **Sintaxe Estilo SASS (Nesting)**: Emprego de aninhamento de seletores (CSS Nesting) no cabeçalho e menu:
  ```css
  header {
      nav {
          a {
              text-decoration: none;
              color: var(--cor-secundaria);
              &:hover {
                  color: var(--cor-destaque);
                  text-shadow: 1px 1px 1px rgb(249, 249, 249);
              }
          }
      }# ☕ Café Aroma & Cia — Exercício Prático de CSS / SASS

![Bolsa Futuro Digital](https://img.shields.io/badge/Curso-Bolsa%20Futuro%20Digital-482715?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![SASS](https://img.shields.io/badge/SASS-CC6699?style=for-the-badge&logo=sass&logoColor=white)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-003603?style=for-the-badge)

Projeto prático desenvolvido para o curso de **Front-End da Bolsa Futuro Digital** (Semana 10).

> 💡 **Nota Importante**: 
> - O projeto foi desenvolvido a partir de um **HTML pronto**, fornecido previamente pelas instruções do exercício.
> - Na folha de estilos (`estilo.css`), foi utilizada a **estrutura/sintaxe de aninhamento no estilo SASS** (CSS Nesting com pseudo-seletores como `&:hover`), facilitando a organização das regras para elementos-filhos de navegação e componentes.

---

## 📋 Sobre o Projeto

O **Café Aroma & Cia** é uma landing page para uma cafeteria artesanal. Partindo do código HTML base disponibilizado pela aula, realizou-se a estilização completa da página, que conta com apresentação da marca, cardápio formatado em tabela, seção de depoimentos de clientes e um formulário para reserva de mesas.

---

## 🎯 Requisitos Cumpridos (Baseados no PDF do Exercício)

### 📌 1. Análise da Estrutura HTML Fornecida
Estudo e mapeamento das seções semânticas do `index.html`:
- `<header>` e `<nav>` com links âncora (`#sobre`, `#cardapio`, `#depoimentos`, `#reservas`).
- `<section>` "Sobre o café" com imagem descritiva (`alt`).
- `<table>` de cardápio com `<thead>`, `<tbody>` e alinhamento de preços.
- `<ul>` com depoimentos e citações de clientes fictícios.
- `<form>` de reserva com inputs (`text`, `email`, `date`, `number`) e botão de envio.
- `<footer>` com dados de endereço
  }
  ```
- [x] **Reset CSS Global**: Reset inicial simples (`* { box-sizing: border-box; margin: 0; padding: 0; }`).

### 📌 3. Aplicação & Estilização (Parte B — Aplicação)
- [x] **Cores e Espaçamento com `:root`**: Aplicação de backgrounds, paddings e margens no header, main e footer usando variáveis CSS.
- [x] **Navegação Interativa**: Links do menu (`nav a`) estilizados com estado `:hover` interativo.
- [x] **Tabela de Cardápio**: Células formatadas e preços alinhados.
- [x] **Tipografia & Legibilidade**: Tipografia para títulos e corpo de texto com fallbacks genéricos e ajuste de `line-height`.
- [x] **Formulário de Reserva**: Estilização de rótulos, campos de entrada e botão de envio, mantendo bom contraste.

---

## 📁 Estrutura de Arquivos

```text
Cafe-Aroma/
├── index.html           # Estrutura HTML5 pronta fornecida pelo exercício
├── estilo.css           # Folha de estilos com variáveis CSS e sintaxe SASS (Nesting)
├── exercicio-cafe.pdf   # Especificação original da atividade prática
├── exercicio1.html      # Exercício complementar da Semana 10
├── README.md            # Documentação completa do projeto
└── img/                 # Recursos visuais do projeto
    ├── background.png   # Imagem da seção 'Sobre'
    ├── fundo.png        # Imagem de plano de fundo do site
    ├── hr1.png          # Linhas decorativas
    ├── hr2.png          # Linhas decorativas
    └── logotipo.png     # Logotipo do Café Aroma
```

---

## 💻 Tecnologias Utilizadas# ☕ Café Aroma & Cia — Exercício Prático de CSS / SASS

![Bolsa Futuro Digital](https://img.shields.io/badge/Curso-Bolsa%20Futuro%20Digital-482715?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![SASS](https://img.shields.io/badge/SASS-CC6699?style=for-the-badge&logo=sass&logoColor=white)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-003603?style=for-the-badge)

Projeto prático desenvolvido para o curso de **Front-End da Bolsa Futuro Digital** (Semana 10).

> 💡 **Nota Importante**: 
> - O projeto foi desenvolvido a partir de um **HTML pronto**, fornecido previamente pelas instruções do exercício.
> - Na folha de estilos (`estilo.css`), foi utilizada a **estrutura/sintaxe de aninhamento no estilo SASS** (CSS Nesting com pseudo-seletores como `&:hover`), facilitando a organização das regras para elementos-filhos de navegação e componentes.

---

## 📋 Sobre o Projeto

O **Café Aroma & Cia** é uma landing page para uma cafeteria artesanal. Partindo do código HTML base disponibilizado pela aula, realizou-se a estilização completa da página, que conta com apresentação da marca, cardápio formatado em tabela, seção de depoimentos de clientes e um formulário para reserva de mesas.

---

## 🎯 Requisitos Cumpridos (Baseados no PDF do Exercício)

### 📌 1. Análise da Estrutura HTML Fornecida
Estudo e mapeamento das seções semânticas do `index.html`:
- `<header>` e `<nav>` com links âncora (`#sobre`, `#cardapio`, `#depoimentos`, `#reservas`).
- `<section>` "Sobre o café" com imagem descritiva (`alt`).
- `<table>` de cardápio com `<thea# ☕ Café Aroma & Cia — Exercício Prático de CSS / SASS

![Bolsa Futuro Digital](https://img.shields.io/badge/Curso-Bolsa%20Futuro%20Digital-482715?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![SASS](https://img.shields.io/badge/SASS-CC6699?style=for-the-badge&logo=sass&logoColor=white)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-003603?style=for-the-badge)

Projeto prático desenvolvido para o curso de **Front-End da Bolsa Futuro Digital** (Semana 10).

> 💡 **Nota Importante**: 
> - O projeto foi desenvolvido a partir de um **HTML pronto**, fornecido previamente pelas instruções do exercício.
> - Na folha de estilos (`estilo.css`), foi utilizada a **estrutura/sintaxe de aninhamento no estilo SASS** (CSS Nesting com pseudo-seletores como `&:hover`), facilitando a organização das regras para elementos-filhos de navegação e componentes.

---

## 📋 Sobre o Projeto

O **Café Aroma & Cia** é uma landing page para uma cafeteria artesanal. Partindo do código HTML base disponibilizado pela aula, realizou-se a estilização completa da página, que conta com apresentação da marca, cardápio formatado em tabela, seção de depoimentos de clientes e um formulário para reserva de mesas.

---

## 🎯 Requisitos Cumpridos (Baseados no PDF do Exercício)

### 📌 1. Análise da Estrutura HTML Fornecida
Estudo e mapeamento das seções semânticas do `index.html`:
- `<header>` e `<nav>` com links âncora (`#sobre`, `#cardapio`, `#depoimentos`, `#reservas`).
- `<section>` "Sobre o café" com imagem descritiva (`alt`).
- `<table>` de cardápio com `<thead>`, `<tbody>` e alinhamento de preços.
- `<ul>` com depoimentos e citações de clientes fictícios.
- `<form>` de reserva com inputs (`text`, `email`, `date`, `number`) e botão de envio.
- `<footer>` com dados de endereçod>`, `<tbody>` e alinhamento de preços.
- `<ul>` com depoimentos e citações de clientes fictícios.
- `<form>` de reserva com inputs (`text`, `email`, `date`, `number`) e botão de envio.
- `<footer>` com dados de endereço

- **HTML5**: Estrutura semântica fornecida na atividade.
- **CSS3 / SASS Structure**: Variáveis `:root`, CSS Nesting (sintaxe SASS), Flexbox e Posicionamento Sticky.
- **Git & GitHub**: Controle de versão e hospedagem do repositório.

---

## 🚀 Como Executar o Projeto

1. **Clonar o repositório:**
   ```bash
   git clone https://github.com/Fr# ☕ Café Aroma & Cia — Exercício Prático de CSS / SASS

![Bolsa Futuro Digital](https://img.shields.io/badge/Curso-Bolsa%20Futuro%20Digital-482715?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![SASS](https://img.shields.io/badge/SASS-CC6699?style=for-the-badge&logo=sass&logoColor=white)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-003603?style=for-the-badge)

Projeto prático desenvolvido para o curso de **Front-End da Bolsa Futuro Digital** (Semana 10).

> 💡 **Nota Importante**: 
> - O projeto foi desenvolvido a partir de um **HTML pronto**, fornecido previamente pelas instruções do exercício.
> - Na folha de estilos (`estilo.css`), foi utilizada a **estrutura/sintaxe de aninhamento no estilo SASS** (CSS Nesting com pseudo-seletores como `&:hover`), facilitando a organização das regras para elementos-filhos de navegação e componentes.

---

## 📋 Sobre o Projeto

O **Café Aroma & Cia** é uma landing page para uma cafeteria artesanal. Partindo do código HTML base disponibilizado pela aula, realizou-se a estilização completa da página, que conta com apresentação da marca, cardápio formatado em tabela, seção de depoimentos de clientes e um formulário para reserva de mesas.

---

## 🎯 Requisitos Cumpridos (Baseados no PDF do Exercício)

### 📌 1. Análise da Estrutura HTML Fornecida
Estudo e mapeamento das seções semânticas do `index.html`:
- `<header>` e `<nav>` com links âncora (`#sobre`, `#cardapio`, `#depoimentos`, `#reservas`).
- `<section>` "Sobre o café" com imagem descritiva (`alt`).
- `<table>` de cardápio com `<thead>`, `<tbody>` e alinhamento de preços.
- `<ul>` com depoimentos e citações de clientes fictícios.
- `<form>` de reserva com inputs (`text`, `email`, `date`, `number`) e botão de envio.
- `<footer>` com dados de endereçoanGnMoraes/Cafe-Aroma.git
   ```
2. **Acessar a pasta do projeto:**
   ```bash
   cd Cafe-Aroma
   ```
3. **Visualizar no navegador:**
   Abra o arquivo `index.html` diretamente em seu navegador preferido ou utilize a extensão **Live Server** no VS Code.

---

<div align="center">
  <sub>Atividade prática realizada para a Semana 10 do curso <b>Bolsa Futuro Digital — Front-End</b>.</sub>
</div>