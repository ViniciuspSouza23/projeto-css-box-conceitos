# Projeto: CSS Box Model & Flexbox Conceitos

Projeto prático desenvolvido para demonstrar e fixar os conceitos fundamentais do **CSS Box Model** e as propriedades do **CSS Flexbox** de forma totalmente responsiva.

---

## 🚀 Estrutura de Arquivos

- [`index.html`](./index.html): Documento HTML5 semântico com a marcação dos 20 elementos, áreas de demonstração prática e catálogo de propriedades. Inclui a folha de estilos externa através da tag `<link rel="stylesheet" href="style.css">`.
- [`style.css`](./style.css): Folha de estilo externa com variáveis CSS, estilização individual do Box Model para os 20 elementos, contêineres Flexbox e regras de responsividade com Media Queries.

---

## 📦 Box Model: 20 Elementos Personalizados

Cada um dos 20 elementos (`.item-01` até `.item-20`) possui valores explícitos atribuídos para:
1. **Content**: `width`, `height`, `box-sizing`
2. **Padding**: Espaçamento interno (`padding` / `padding-top`, `right`, `bottom`, `left`)
3. **Border**: Espessura, estilo e cor da borda (`border-width`, `border-style`, `border-color`, `border-radius`)
4. **Margin**: Espaçamento externo (`margin` / `margin-top`, `right`, `bottom`, `left`)

---

## ⚡ Flexbox: Mais de 20 Propriedades e Valores Utilizados

1. `display: flex`
2. `display: inline-flex`
3. `flex-direction: row`
4. `flex-direction: column`
5. `flex-direction: row-reverse`
6. `flex-direction: column-reverse`
7. `flex-wrap: wrap`
8. `flex-wrap: nowrap`
9. `flex-wrap: wrap-reverse`
10. `flex-flow: row wrap`
11. `justify-content: center`
12. `justify-content: space-between`
13. `justify-content: space-around`
14. `justify-content: space-evenly`
15. `justify-content: flex-start`
16. `justify-content: flex-end`
17. `align-items: center`
18. `align-items: stretch`
19. `align-items: flex-start`
20. `align-items: flex-end`
21. `align-content: space-between`
22. `gap` (`row-gap` e `column-gap`)
23. `order` (`order: 1`, `order: -1`)
24. `flex-grow` (`flex-grow: 1`, `flex-grow: 2`)
25. `flex-shrink: 0`
26. `flex-basis: 260px`
27. `flex: 1 1 240px` (shorthand)
28. `align-self: flex-start`, `align-self: center`, `align-self: flex-end`

---

## 📱 Responsividade

O projeto se adapta dinamicamente a qualquer tamanho de tela:
- **Desktop (> 1024px)**: Exibição fluida em múltiplas colunas e layouts distribuídos.
- **Tablets (≤ 768px)**: Adaptação de contêineres e reorganização em colunas responsivas.
- **Smartphones (≤ 480px)**: Empilhamento vertical total e espaçamentos otimizados para toque.