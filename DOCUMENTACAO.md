# Guia de estudo — VivaMente

O VivaMente é um projeto acadêmico. Não possui login, agenda, pagamento,
banco de dados ou envio de formulário reais.

## Arquivos importantes

- `index.html`: página inicial.
- `resultados.html`: profissionais fictícios.
- `css/style.css`: visual de todas as páginas.
- `imagens/`: imagens do projeto.

## Tecnologias

- **HTML:** organiza textos, links, imagens e formulários.
- **CSS:** define cores, fontes, bordas e espaçamentos.
- **Bootstrap:** usado apenas em colunas, campos e botões simples.

## Como alterar o visual

### Cor do fundo

No `css/style.css`, procure `body`:

```css
background: #f5f3ee; /* Cor do fundo. */
```

Troque `#f5f3ee` pela cor desejada.

### Cor da fonte

```css
color: #333; /* Cor dos textos. */
```

Troque `#333` pela nova cor de texto.

### Fonte e tamanho

```css
font-family: Arial, sans-serif; /* Fonte do site. */
font-size: 26px; /* Tamanho do texto. */
```

`font-family` muda a fonte; `font-size` muda o tamanho.

### Borda e cantos das caixas

Procure `.caixa, .cartao`:

```css
border: 1px solid #e2e2e2; /* Linha da borda. */
border-radius: 12px; /* Arredonda os cantos. */
```

O primeiro número é a espessura da borda. A cor vem depois de `solid`.

### Botões

```css
background: #739987; /* Cor do botão. */
border: 1px solid #739987; /* Borda do botão. */
color: #fff; /* Cor do texto. */
```

Para trocar a cor, altere `background` e `border` para a mesma cor.

### Espaçamentos

```css
padding: 24px; /* Espaço dentro da caixa. */
margin-bottom: 24px; /* Espaço abaixo do elemento. */
gap: 16px; /* Espaço entre itens lado a lado. */
```

### Menu

Os links estão dentro da tag `<nav>` de cada página:

```html
<a class="menu-link" href="resultados.html">Psicólogos</a>
```

O texto aparece na tela. O `href` indica a página aberta ao clicar.

### Imagens

```html
<img src="imagens/carolina-mendes.webp" alt="Descrição da imagem">
```

`src` indica o arquivo e `alt` descreve a imagem.

## Conceitos de CSS

- `display: flex`: deixa itens lado a lado.
- `display: grid`: cria colunas e linhas.
- `gap`: espaço entre itens.
- `padding`: espaço dentro de um elemento.
- `margin`: espaço fora de um elemento.
- `@media`: ajusta o site para celular.

## Perguntas da apresentação

**O que é HTML?** A estrutura do site.

**O que é CSS?** A aparência do site.

**O projeto funciona de verdade?** Não. É uma demonstração acadêmica.

**Onde muda tudo do visual?** No arquivo `css/style.css`.
