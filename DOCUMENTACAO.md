# Documentação rápida — VivaMente

## Tecnologias

- **HTML:** organiza textos, imagens, links e formulários.
- **CSS:** define cores, espaçamentos, tamanhos e responsividade.
- **Bootstrap:** usado apenas para colunas, campos, botões e tabela, pois reduz código nessas partes.

## Onde alterar cada coisa

- Textos: no arquivo `.html` da página.
- Cores, botões, cartões, menu e rodapé: `css/style.css`.
- Imagens: pasta `imagens/` e atributo `src` da imagem.
- Links: atributo `href` das tags `<a>`.

## Organização do CSS

O arquivo `css/style.css` está dividido por comentários `/* */`:

- cores e ajustes gerais;
- cabeçalho e menu;
- caixas e cartões;
- botões;
- página inicial;
- formulários;
- Área do Paciente;
- rodapé e celular.

## Perguntas para a apresentação

**O que é responsividade?** É quando o site se adapta a telas menores, como celulares.

**Por que usar Bootstrap?** Para não repetir CSS em colunas, formulários e tabelas. O visual principal continua sendo nosso, no `style.css`.

**O site funciona de verdade?** Não. É uma demonstração acadêmica e não salva dados nem realiza pagamentos.

**Onde mudar a cor dos botões?** Na classe `.botao-verde` do arquivo `css/style.css`.

**Onde mudar o menu?** Dentro da tag `<nav>` no começo de cada página HTML.

## Fluxo do site

`Início → Psicólogos → Perfil ou Pagamento → Confirmação`

O link “Minha Área” abre uma Área do Paciente apenas ilustrativa.
