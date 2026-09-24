# Projeto: CSS Box Model & Flexbox Conceitos

Projeto didático e interativo desenvolvido para demonstrar e fixar os conceitos fundamentais do **CSS Box Model** e as propriedades do **CSS Flexbox** de forma totalmente responsiva.

O projeto agora conta com **duas versões completas**:
1. **Versão Vanilla CSS** (CSS puro externo com variáveis e media queries).
2. **Versão Tailwind CSS v4** (Classes utilitárias compiladas via `@tailwindcss/cli`).

---

## 🚀 Estrutura de Arquivos

```
projeto-css-box-conceitos/
├── index.html            # Versão em Vanilla CSS puro
├── style.css             # Folha de estilo externa (Vanilla CSS)
├── index-tailwind.html   # Versão em Tailwind CSS v4
├── src/
│   └── input.css         # Ponto de entrada do Tailwind (@import "tailwindcss";)
├── dist/
│   └── output.css        # CSS compilado e minificado pelo Tailwind CLI
├── package.json          # Dependências (@tailwindcss/cli) e scripts de build
└── README.md             # Documentação do projeto
```

---

## ⚡ Como rodar a versão em Tailwind CSS

### 1. Pré-requisitos
Certifique-se de ter o [Node.js](https://nodejs.org/) instalado.

### 2. Instalação das Dependências
```bash
npm install
```

### 3. Compilar o Tailwind CSS

- **Modo Desenvolvimento (com auto-rebuild / watch):**
  ```bash
  npm run dev:css
  ```

- **Modo Produção (compilar e minificar):**
  ```bash
  npm run build:css
  ```

### 4. Visualizar no Navegador
- Basta abrir o arquivo [`index-tailwind.html`](./index-tailwind.html) em qualquer navegador ou via Live Server no VS Code / Antigravity IDE.
- É possível alternar entre as duas versões a qualquer momento através da barra no topo da página.

> **Nota:** O `@import "tailwindcss";` é uma diretiva que vai dentro de um arquivo `.css` (como em `src/input.css`), e **não** um comando para ser digitado diretamente no terminal PowerShell.

---

## 📦 Box Model: 20 Elementos Personalizados

Cada um dos 20 elementos possui valores explícitos atribuídos para:
1. **Content**: `width` (`w-[px]`), `height` (`h-[px]`), `box-sizing` (`box-border`)
2. **Padding**: Espaçamento interno (`padding` / `p-[px]`)
3. **Border**: Espessura, estilo e cor da borda (`border-[px]`, `border-solid`, `border-dashed`, `border-double`, etc.)
4. **Margin**: Espaçamento externo (`margin` / `m-[px]`)

---

## ⚡ Flexbox: Mais de 20 Propriedades e Valores Utilizados

| # | Propriedade CSS Nativa | Classe no Tailwind CSS | Descrição |
|---|------------------------|-------------------------|-----------|
| 01 | `display: flex;` | `flex` | Contêiner flexível de bloco |
| 02 | `display: inline-flex;` | `inline-flex` | Contêiner flexível inline |
| 03 | `flex-direction: row;` | `flex-row` | Eixo horizontal padrão |
| 04 | `flex-direction: column;` | `flex-col` | Eixo vertical (de cima para baixo) |
| 05 | `flex-direction: row-reverse;` | `flex-row-reverse` | Eixo horizontal invertido |
| 06 | `flex-direction: column-reverse;` | `flex-col-reverse` | Eixo vertical invertido |
| 07 | `flex-wrap: wrap;` | `flex-wrap` | Permite quebra de linhas |
| 08 | `flex-wrap: nowrap;` | `flex-nowrap` | Impede quebra de linhas |
| 09 | `flex-wrap: wrap-reverse;` | `flex-wrap-reverse` | Quebra de linha no sentido oposto |
| 10 | `flex-flow: row wrap;` | `flex-row flex-wrap` | Shorthand de direção e quebra |
| 11 | `justify-content: center;` | `justify-center` | Centraliza no eixo principal |
| 12 | `justify-content: space-between;` | `justify-between` | Espaçamento uniforme até as bordas |
| 13 | `justify-content: space-around;` | `justify-around` | Espaçamento igual ao redor de cada item |
| 14 | `justify-content: space-evenly;` | `justify-evenly` | Espaçamento estritamente idêntico |
| 15 | `align-items: center;` | `items-center` | Alinha no centro do eixo transversal |
| 16 | `align-items: stretch;` | `items-stretch` | Estica os itens no eixo transversal |
| 17 | `align-content: space-between;` | `content-between` | Distribui linhas quebradas |
| 18 | `gap: 24px;` | `gap-6` | Espaçamento entre itens flexíveis |
| 19 | `order: 1; / order: -1;` | `order-1` / `-order-1` | Reordena visualmente o item |
| 20 | `flex-grow: 1;` | `grow` / `grow-[2]` | Capacidade de preencher o espaço restante |
| 21 | `flex-shrink: 0;` | `shrink-0` | Impede encolhimento do item |
| 22 | `flex-basis: 75px;` | `basis-[75px]` | Tamanho base inicial antes do flex |
| 23 | `flex: 1 1 auto;` | `flex-1` / `flex-initial` | Shorthand (grow, shrink, basis) |
| 24 | `align-self: flex-end;` | `self-end` / `self-start` | Sobrescreve alinhamento transversal do filho |

---

## 📱 Responsividade Total

Ambas as versões contam com suporte completo a todas as resoluções de tela:
- **Desktop (> 1024px)**: Layout amplo e distribuído.
- **Tablets (≤ 768px)**: Adaptação fluida e reorganização de contêineres.
- **Smartphones (≤ 480px)**: Empilhamento vertical total e espaçamentos otimizados.