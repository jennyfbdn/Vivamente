# Documentação do projeto VivaMente

## 1. O que foi usado

O projeto foi feito com:

- HTML: cria o conteúdo das páginas;
- CSS: muda cores, tamanhos, bordas e espaçamentos;
- Bootstrap 5: ajuda na estrutura, responsividade, formulários, botões e pequenos espaçamentos.

Não foram usados JavaScript, banco de dados, servidor ou pagamento verdadeiro.

## 2. Estrutura das pastas

```text
vivamente/
├── como-funciona.html
├── resultados.html
├── perfil-psicologo.html
├── login.html
├── cadastro.html
├── pagamento.html
├── confirmacao.html
├── css/
│   └── style.css
└── imagens/
    └── carolina-mendes-ficticia.png
```

## 3. Função de cada página

### como-funciona.html

Explica as três etapas da plataforma: escolher o profissional, agendar e começar o acompanhamento.

### resultados.html

Apresenta três psicólogos fictícios. O botão "Agendar" abre a página de pagamento.

### perfil-psicologo.html

Mostra a foto e as informações da personagem fictícia Dra. Carolina Mendes.

### login.html

Mostra os campos de e-mail e senha. O login não é verdadeiro.

### cadastro.html

Mostra os campos de nome, e-mail, senha e confirmação de senha. Nenhum dado é salvo.

### pagamento.html

Mostra campos visuais de cartão e um resumo da consulta. Nenhum pagamento é realizado.

### confirmacao.html

Mostra uma confirmação ilustrativa da consulta.

## 4. Estrutura básica de uma página

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <!-- Configurações da página -->
</head>
<body>
    <header><!-- Cabeçalho e menu --></header>
    <main><!-- Conteúdo principal --></main>
    <footer><!-- Rodapé --></footer>
</body>
</html>
```

- `head`: contém o título, a configuração de caracteres e os arquivos CSS;
- `header`: contém o cabeçalho;
- `nav`: contém os links do menu;
- `main`: contém o assunto principal da página;
- `section`: separa partes do conteúdo;
- `footer`: contém o rodapé.

## 5. O que é Bootstrap

Bootstrap é um arquivo CSS pronto que oferece classes para organizar e formatar páginas. Neste projeto, ele foi usado em poucas partes para facilitar a explicação durante a apresentação.

Ele é carregado em cada página por esta linha:

```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
```

O CSS do projeto é carregado logo depois:

```html
<link rel="stylesheet" href="css/style.css">
```

O `style.css` vem depois para aplicar as cores e a identidade da VivaMente. O Bootstrap fornece algumas estruturas prontas; o CSS próprio personaliza o visual.

## 6. Classes do Bootstrap usadas

O Bootstrap foi usado onde ele deixa o código menor e fácil de explicar:

```text
Estrutura:       container, row e colunas
Formulários:     form-label e form-control
Botões:          btn e w-100
Alinhamento:     text-center
Espaçamentos:    g-4 e mb-3
```

Não existe uma regra dizendo que Bootstrap só pode ser usado nessas partes. A escolha foi feita para evitar repetição sem esconder todo o projeto atrás de classes prontas.

### container

Centraliza o conteúdo e cria espaço nas laterais.

```html
<main class="container">
```

### row

Cria uma linha para receber colunas.

```html
<div class="row">
```

### col-md-4

Cria uma coluna que ocupa 4 das 12 partes da linha em telas médias ou grandes.

Três colunas `col-md-4` ocupam a linha inteira:

```text
4 + 4 + 4 = 12
```

No celular, as colunas ficam uma abaixo da outra.

### Outras colunas

- `col-6`: ocupa metade da linha em qualquer tamanho de tela;
- `col-md-6`: ocupa metade da linha em telas médias ou maiores;
- `col-md-8`: ocupa 8 das 12 partes em telas médias ou maiores.

### form-label e form-control

Formatam os textos e campos dos formulários:

```html
<label class="form-label">E-mail</label>
<input class="form-control">
```

### btn

Fornece o formato básico do botão. A cor continua no CSS próprio:

```html
<a class="btn botao-verde">Agendar</a>
```

### text-center

Centraliza o texto:

```html
<h1 class="text-center">Pagamento</h1>
```

### g-4 e mb-3

- `g-4`: cria espaço entre as colunas;
- `mb-3`: cria margem abaixo de um campo.

### w-100

Faz um botão ocupar toda a largura disponível.

## 7. CSS próprio do projeto

O arquivo `css/style.css` está dividido por comentários objetivos.

As principais classes próprias são:

- `.menu`: organiza o cabeçalho;
- `.links-menu`: organiza os links;
- `.caixa`: cria as caixas brancas;
- `.botao-verde`: aplica as cores da VivaMente nos botões;
- `.titulo-pagina`: cria espaço abaixo do título;
- `.secao`: cria espaço entre seções.

### Mudar a cor do fundo

Procure por:

```css
/* COR DO FUNDO */
body {
    background-color: #F5F3EE;
}
```

Troque `#F5F3EE` pela nova cor.

Exemplo de fundo azul-claro:

```css
background-color: #EAF4FF;
```

### Mudar a cor de todos os textos

Procure por:

```css
/* COR DOS TEXTOS */
body {
    color: #333333;
}
```

### Mudar a cor do nome VivaMente

Procure por `.marca`:

```css
.marca {
    color: #5F806F;
    font-size: 26px;
}
```

### Mudar a cor dos botões

Procure por:

```css
/* COR DOS BOTÕES */
.botao-verde {
    background-color: #739987;
    border: 1px solid #739987;
    color: #FFFFFF;
}
```

É importante mudar `background-color` e `border` para a mesma cor.

### Mudar a cor das caixas

Procure por `.caixa`:

```css
.caixa {
    background-color: #FFFFFF;
}
```

Todas as páginas usam essa mesma classe. Uma única mudança altera cartões, formulários e resumos.

### Mudar o tamanho da foto

Procure por:

```css
/* TAMANHO DA FOTO */
.foto-perfil {
    max-width: 320px;
    width: 100%;
}
```

Troque `320px` pelo tamanho desejado.

## 8. Cores usadas

```text
Fundo bege:       #F5F3EE
Verde principal:  #739987
Verde escuro:     #5F806F
Branco:           #FFFFFF
Texto escuro:     #333333
Texto secundário: #666666
```

## 9. Diferença entre classe do Bootstrap e classe própria

Neste exemplo:

```html
<a class="btn botao-verde">Agendar</a>
```

- `btn` pertence ao Bootstrap e fornece o formato básico;
- `botao-verde` pertence ao projeto e define as cores.

Neste outro exemplo:

```html
<div class="col-md-4">
    <div class="caixa">Conteúdo</div>
</div>
```

- `col-md-4` pertence ao Bootstrap;
- `caixa` pertence ao projeto.

Assim, o Bootstrap cuida da coluna e o CSS próprio cuida da aparência.

## 10. Perguntas que a professora pode fazer

### O que é HTML?

É a linguagem que organiza o conteúdo da página, como títulos, parágrafos, imagens, links e formulários.

### O que é CSS?

É a linguagem que muda a aparência do HTML, como cores, fontes, tamanhos, bordas e espaços.

### O que é Bootstrap?

É um conjunto de estilos CSS prontos. No projeto, ele ajuda com contêineres, colunas responsivas, campos, botões, alinhamentos e alguns espaçamentos.

### O que significa responsividade?

É a capacidade do site de se adaptar a celulares, tablets e computadores.

### Onde muda a cor do fundo?

No arquivo `css/style.css`, na parte marcada com `/* COR DO FUNDO */`.

### Onde muda a cor dos botões?

No arquivo `css/style.css`, na classe `.botao-verde`.

### Onde muda um texto?

No arquivo HTML da página em que o texto aparece.

### Onde muda uma imagem?

No atributo `src` da tag `img`:

```html
<img src="imagens/carolina-mendes-ficticia.png" alt="Descrição da imagem">
```

### Para que serve href?

Indica qual página será aberta por um link:

```html
<a href="login.html">Entrar</a>
```

### Para que serve class?

Liga um elemento a estilos do Bootstrap ou do arquivo CSS.

### O login funciona de verdade?

Não. O formulário é apenas visual e não possui servidor ou banco de dados.

### O pagamento funciona de verdade?

Não. Os campos e a confirmação são apenas ilustrativos.

## 11. Fluxo entre as páginas

```text
Como Funciona → Resultados → Perfil ou Pagamento → Confirmação
                         ↘ Login ↔ Cadastro
```

Os links mudam de página, mas não existe processamento de dados.

## 12. Como abrir o projeto

Abra o arquivo `como-funciona.html` no navegador.

É necessário ter internet para carregar o Bootstrap pelo endereço CDN. O projeto não precisa de `npm`, Node.js ou servidor.
