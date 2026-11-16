# Portfólio Profissional Web

## Título do projeto
Portfólio Profissional com HTML e Bootstrap

## Desenvolvedor
Matheus Henrique de Souza

## Descrição do portfólio
O portfólio é um Single Page Application (SPA) que reúne de forma visual o meu perfil profissional, meus conhecimentos em programação, uma listagem dos meus projetos em Python, C++ e Desenvolvimento Web, e links diretos para contato e networking. O objetivo principal do projeto foi demonstrar na prática conceitos de design responsivo e a organização de código utilizando frameworks modernos.

## Tecnologias utilizadas

<div style="display: inline_block"><br>
  <img align="center" alt="HTML5" src="https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white" />
  <img align="center" alt="CSS3" src="https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white" />
  <img align="center" alt="Bootstrap" src="https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white" />
  <img align="center" alt="C++" src="https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white" />
  <img align="center" alt="Python" src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" />
  <img align="center" alt="GitHub" src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white" />
</div><br>

- **HTML5:** Para estruturação semântica de todo o conteúdo (linguagem de marcação).
- **CSS3:** Para a personalização do design e implementação das animações de estilo.
- **Bootstrap 5:** Framework utilizado extensivamente para garantir a responsividade (Grid System) e fornecer componentes prontos (Navbars, Cards, Carousel e Botões).
- **Devicon:** Biblioteca de ícones (CDN) usada para representar graficamente as tecnologias estudadas no site.
- **GitHub Pages:** Para hospedagem e publicação online do projeto.

## Link do site publicado
[LINK DO GITHUB PAGES AQUI - ex: https://Matheushidra.github.io/Apresentacao]

## Explicação do funcionamento do projeto
O funcionamento segue a lógica de um site estático. A estrutura utiliza o elemento `<nav>` como um menu fixo no topo (`sticky-top`) que direciona o usuário por meio de links de ancoragem local (`href="#projetos"`). O corpo (body) contém 4 seções principais separadas por `<section>`.

O projeto é inteiramente *mobile first*: graças à classe `navbar-expand-lg` e à propriedade de coluna `col-md-6`, todos os elementos de grid e menu que aparecem alinhados lateralmente em telas de computador se convertem automaticamente em listas e botões em formato empilhado para telas de celulares.

## Descrição do recurso novo adicionado
Com o objetivo de ir além da estrutura base, o projeto foi estendido através de **dois novos recursos baseados em CSS**:
1. **Smooth Scroll (Rolagem Suave):** Adiciona uma fluidez melhorada à navegação via menu âncora.
2. **Interação Visual e Animações de Hover:** Criação de uma animação fluida baseada em transformações nos cards da seção de projetos.

## Explicação de como esse recurso foi implementado
Para implementar estes recursos complementares, foi criado o arquivo `style.css` (Externo). 
- O **Smooth Scroll** foi aplicado inserindo a propriedade de comportamento `scroll-behavior: smooth` diretamente sobre o elemento raiz `html`. Também foi necessário declarar a propriedade `scroll-margin-top: 70px` nas tags `section` para impedir que o título de cada categoria ficasse coberto pelo menu de topo fixo após a conclusão da rolagem.
- Para o **Hover Animado**, foi inventada uma classe CSS independente chamada `.card-animado`. Nela, definiu-se a regra de comportamento `transition: 0.3s ease`. Posteriormente, através da pseudo-classe `:hover` (que captura o cursor sobre o elemento), as propriedades `transform: translateY(-10px)` e `box-shadow` foram ativadas simultaneamente. Dessa forma, quando o usuário explora a aba de projetos, os cards "saltam", fornecendo feedback visual imediato de que a área é interativa.
