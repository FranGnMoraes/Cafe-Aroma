# ☕ Café Aroma & Cia

![Bolsa Futuro Digital](https://img.shields.io/badge/Curso-Bolsa%20Futuro%20Digital-482715?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![SASS](https://img.shields.io/badge/SASS-CC6699?style=for-the-badge&logo=sass&logoColor=white)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-003603?style=for-the-badge)

Projeto finalizado de uma landing page para uma cafeteria artesanal, desenvolvida em HTML, CSS e Sass, com ajustes visuais refinados para um resultado mais premium e profissional.

---

## 📌 Visão geral do projeto

A página foi construída a partir de um HTML base e evoluiu para uma composição com:
- header fixo com logo + identidade da marca
- seção Sobre com imagem + texto lado a lado
- cardápio em grid responsivo
- seção de depoimentos em carrossel horizontal
- formulário de reserva com estilo refinado
- layout mais equilibrado em desktop e mobile

O foco principal foi aprender a organizar a interface visual com boa consistência de espaçamento, hierarquia tipográfica e alinhamento estrutural.

---

## 🧠 Aprendizados principais

### Flexbox
O uso de `display: flex` foi essencial para:
- alinhamento do logo e nome da marca no header
- organização da seção Sobre em imagem + texto
- ajustes de alinhamento vertical e horizontal
- responsividade em telas menores

Desafio principal:
- ajustar o comportamento do conteúdo ao reduzir a largura, sem que o texto ficasse "esticado" ou desbalanceado.

### Grid
O cardápio foi reorganizado com `display: grid`, o que permitiu:
- manter colunas responsivas sem quebrar o layout
- criar blocos de card com estrutura mais clara
- controlar espaçamento e largura de forma mais consistente

Desafio principal:
- encontrar o equilíbrio ideal entre largura dos cards, gaps e responsividade, para manter a visual premium.

### Carrossel com JavaScript
A seção de depoimentos foi pensada como carrossel horizontal para simular uma experiência mais dinâmica, com navegação por setas.

Foi usado JavaScript simples com `scrollBy()` para mover o container horizontalmente:

```js
const trilho = document.querySelector('.carrossel');

document.querySelector('.next').onclick = () => {
  trilho.scrollBy({ left: 320, behavior: 'smooth' });
};

document.querySelector('.prev').onclick = () => {
  trilho.scrollBy({ left: -320, behavior: 'smooth' });
};
```

Desafios principais:
- manter o carrossel visualmente alinhado com o restante do layout
- evitar que as setas “puxassem” o visual para longe do bloco
- reduzir o peso visual dos botões sem perder a legibilidade

---

## 🎨 Refinamentos de design aplicados

Entre os refinamentos mais importantes, destacam-se:
- padronização de espaçamentos com variáveis CSS
- criação de uma escala visual mais consistente
- ajuste de margens para evitar sensação de desalinhamento
- uso de blocos com largura controlada para deixarem os elementos mais harmoniosos
- refinamento do carrossel para que as setas sobressaiam sem parecer “decorativas demais”

---

## 🧩 Estrutura de arquivos

```text
Cafe-Aroma/
├── index.html              # Estrutura da landing page
├── estilo.css              # CSS compilado final
├── scss/
│   └── style.scss          # Arquivo principal em Sass
├── img/                    # Imagens do projeto
├── package.json            # Scripts do Sass
├── package-lock.json
├── README.md               # Documentação do projeto
├── exercicio1.html
├── exercicio-cafe.pdf
└── .gitignore
```

---

## ⚙️ Como rodar o projeto

1. Abra a pasta do projeto:
   ```bash
   cd Cafe-Aroma
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. Rode o compilador Sass para atualizar o CSS automaticamente:
   ```bash
   npm run sass
   ```

4. Ou compile uma vez:
   ```bash
   npm run build
   ```

5. Abra `index.html` no navegador.

---

## 📝 Observações finais

Esse projeto foi um ótimo exercício para praticar:
- organização visual com CSS
- uso de Flexbox para composição de layouts
- uso de Grid para menus, cards e blocos responsivos
- detalhamento de pequenos ajustes visuais que fazem muita diferença no resultado final
- integração de um carrossel simples com JavaScript

O maior aprendizado foi perceber que, em front-end, o visual mais profissional vem de detalhes pequenos e consistentes: espaçamento, alinhamento, proporção e equilíbrio.

---

<div align="center">
  <sub>Projeto finalizado como estudo prático de HTML, CSS, Sass, Flexbox, Grid e interação com JavaScript.</sub>
</div>
