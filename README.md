# Desafio prático — Página de Sistema com HTML e CSS

## Objetivo

Construir uma página web responsiva que represente a interface inicial de um sistema de cadastro. O exercício deve consolidar o uso de HTML semântico, classes CSS, Flexbox, Grid, formulários, paleta de cores, estados de interação e responsividade.

## Arquivos do projeto

```text
desafio_html_css/
├── index.html
├── style.css
└── imagem-cabecalho.svg
```

## Estrutura obrigatória da página

### 1. Cabeçalho

Utilizar a tag `<header>` com:

- uma imagem ocupando toda a área;
- um título principal;
- um pequeno subtítulo;
- texto sobreposto à imagem.

### 2. Navbar superior

Utilizar a tag `<nav>`, uma lista `<ul>` e links `<a>` contendo:

- Home;
- Produtos;
- Clientes;
- Contato.

Os links devem ficar lado a lado em telas maiores e poderão quebrar linha em telas menores.

### 3. Área de conteúdo em duas colunas

Criar uma `<div class="layout">` usando CSS Grid:

- coluna esquerda com largura aproximada de `240px`;
- coluna direita ocupando o espaço restante;
- espaçamento de aproximadamente `28px` entre as colunas.

### 4. Menu lateral

Utilizar a tag `<aside>` contendo:

- Dashboard;
- Clientes;
- Produtos;
- Relatórios.

O menu deverá ter fundo branco, cantos arredondados e efeito visual ao passar o mouse.

### 5. Área principal

Utilizar a tag `<main>` contendo uma introdução e um formulário.

O formulário deve possuir:

- campo Nome;
- campo E-mail;
- campo Senha;
- botão Salvar cadastro.

Cada campo deverá ser colocado dentro de sua própria `<div class="formulario__grupo">`.

### 6. Rodapé

Utilizar a tag `<footer>` com a frase:

> Sistema desenvolvido pelos alunos

## Paleta de cores sugerida

| Finalidade | Cor | Código |
|---|---|---|
| Cabeçalho e rodapé | Azul-escuro | `#16324F` |
| Links e destaques | Azul principal | `#2563EB` |
| Fundos de destaque | Azul-claro | `#DBEAFE` |
| Botão principal | Verde | `#16A34A` |
| Fundo da página | Cinza-claro | `#F1F5F9` |
| Bordas | Cinza médio | `#CBD5E1` |
| Texto secundário | Cinza escuro | `#475569` |
| Cartões e campos | Branco | `#FFFFFF` |

As cores devem ser criadas como variáveis dentro do seletor `:root`.

## Recursos CSS que devem ser praticados

- seletor universal `*`;
- variáveis CSS;
- `display: flex`;
- `display: grid`;
- `gap`;
- `padding` e `margin`;
- `border-radius`;
- `box-shadow`;
- `hover` e `focus`;
- `transition`;
- `object-fit`;
- `position: relative` e `position: absolute`;
- media query com `@media`.

## Divisões sugeridas

```html
<body>
    <header class="cabecalho">...</header>

    <nav class="navbar">...</nav>

    <div class="layout">
        <aside class="menu-lateral">...</aside>

        <main class="conteudo-principal">
            <section class="apresentacao">...</section>
            <section class="cartao-formulario">
                <form class="formulario">
                    <div class="formulario__grupo">...</div>
                </form>
            </section>
        </main>
    </div>

    <footer class="rodape">...</footer>
</body>
```

## Requisitos de responsividade

Quando a largura da tela for menor que `760px`:

- o menu lateral deve ficar acima do conteúdo principal;
- o layout deve passar de duas colunas para uma coluna;
- o botão deve ocupar toda a largura;
- a navbar poderá quebrar linha.

## Critérios de avaliação sugeridos

| Critério | Pontuação |
|---|---:|
| Estrutura HTML semântica | 2,0 |
| Organização das classes e divs | 1,5 |
| Formulário completo | 1,5 |
| Aplicação da paleta de cores | 1,0 |
| Uso de Flexbox e Grid | 1,5 |
| Efeitos de hover e focus | 1,0 |
| Responsividade | 1,0 |
| Comentários e organização do código | 0,5 |
| **Total** | **10,0** |

## Desafio adicional

Acrescentar:

- ícones aos menus;
- campo de confirmação de senha;
- checkbox para aceitar os termos;
- mensagem de sucesso após o envio;
- modo escuro;
- validação com JavaScript.
