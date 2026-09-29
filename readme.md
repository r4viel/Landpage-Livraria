# Planejamento do projeto

1. Qual é o tema do projeto?
    O tema escolhido foi uma livraria

2. Qual é o objetivo da página?
    criar uma pagina destinada a compra de livros 

3. Para quem essa página está sendo criada?
    Leitores de diversos generos literarios e faixas etarias

4. Quais seções a página terá?
    uma seção pra cada estilo de livro, contato e carrinho

5. Quais componentes simples serão necessários?
    botões, links, imagens, paragrafos, etc.

6. Quais componentes compostos serão necessários?
    Navbar, sections para cada genero literario, 

7. Quais componentes terão variantes visuais?
    Os "cards" dos livros de cada genero literario diferente terá uma cor de destaque diferente

8. Quais componentes serão reutilizados em mais de uma parte da interface?
    Os "cards" dos livros de cada categoria  

9. Como será a organização geral da página no wireframe?
    Pagina principal
    ┌─────────────────────────────────────┐
    │ Navbar: logo | links | botão        │
    ├─────────────────────────────────────┤
    │ Hero: título | texto | botão        │
    ├─────────────────────────────────────┤
    │ Cards de livros em destaque         │
    │ [Card] [Card] [Card]                │
    ├─────────────────────────────────────┤
    │ Rodapé                              │
    └─────────────────────────────────────┘
    Formulario de contato
    ┌─────────────────────────────────────┐
    │ Navbar: logo | links | botão        │
    ├─────────────────────────────────────┤
    │ Hero: título | texto | botão        │
    ├─────────────────────────────────────┤
    │ Formulario para contato|            │
    │            botão de enviar          │
    ├─────────────────────────────────────┤
    │ Rodapé                              │
    └─────────────────────────────────────┘



# Projeto Livraria entre Páginas

Este projeto consiste numa plataforma web para uma biblioteca digital, desenvolvida com HTML5 e CSS3 puro, focada em semântica, responsividade e componentização (BEM).

## Funcionalidades e Estrutura

- **`index.html`**: Página principal contendo o cabeçalho de navegação, destaques da biblioteca, seções de livros categorizadas por género literário, formulário de subscrição (CTA) e rodapé.
- **`componentes.html`**: Guia de estilos (Style Guide / Mini Design System) demonstrando todos os componentes simples (botões, badges, alertas, inputs) e compostos isoladamente.

## Componentes e Variantes

- **Botões (`.btn`)**: Criados com a variante base e extensões para ações específicas (`.btn--primary`, `.btn--secondary`, `.btn--danger`).
- **Cards Por Género**:
  - **Terror (`.cardTerror`)**: Fundo avermelhado suave (`#fff5f5`) e detalhes em vermelho escuro.
  - **Romance (`.cardRomance`)**: Fundo rosa suave (`#fcf0f8`) e detalhes em tons de violeta.
  - **Mistério (`.cardMistério`)**: Fundo azul-noite suave (`#f2f0f9`) e detalhes em índigo.
  - **Fantasia (`.cardFantasia`)**: Fundo dourado/creme suave (`#fffdf0`) e detalhes em roxo/amarelo.

## Tecnologias e Conceitos Aplicados

1. **CSS Grid**: Aplicado no layout das seções de livros para criar grelhas responsivas automáticas (`repeat(auto-fit, minmax(280px, 1fr))`).
2. **Flexbox**: Utilizado na estrutura do cabeçalho (`.header`), nas listas de navegação, no alinhamento interno dos cards e no formulário.
3. **Position**: Uso de `position: sticky` no menu superior para acompanhamento do scroll e `position: relative`/`absolute` em badges sobrepostas.
4. **Float**: Aplicado na classe `.destaque__image--float` para fazer o texto fluir ao redor da imagem nos cards em destaque.
5. **Responsividade**: *Media queries* aplicadas a breakpoints móveis (`768px`), reorganizando a navegação e ajustando formulários e grelhas para telas menores.
6. **Metodologia BEM**: Nomenclatura baseada em *Block__Element--Modifier* para manter o código modular e legível.
