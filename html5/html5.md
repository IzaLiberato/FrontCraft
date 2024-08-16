# Conceitos Básicos de HTML

## 1. O que é HTML?
HTML (HyperText Markup Language) é a linguagem usada para criar e estruturar páginas web. Utiliza "tags" para definir e organizar o conteúdo de uma página.

## 2. Estrutura de um Documento HTML

### 2.1 Declaração do Tipo de Documento
- **Tag**: `<!DOCTYPE html>`
- **Descrição**: Declara que o documento é um HTML5, ajudando o navegador a renderizar a página corretamente.

### 2.2 Elemento Raiz
- **Tag**: `<html>`
- **Descrição**: O contêiner principal que engloba todo o conteúdo da página. Contém dois principais filhos: `<head>` e `<body>`.

## 3. Conceitos de Hierarquia e Estrutura

### 3.1 Hierarquia e Aninhamento
- **Descrição**: A estrutura hierárquica em HTML define como os elementos são organizados dentro de outros elementos. Essa organização determina como o conteúdo é exibido e interpretado pelos navegadores.

### 3.2 Elementos Pais e Filhos
- **Elemento Pai**: Um elemento que contém outros elementos. Exemplo: `<div>` que contém outros elementos como `<p>` ou `<span>`.
- **Elemento Filho**: Um elemento que está contido dentro de outro elemento. Exemplo: `<p>` dentro de um `<div>`.
- **Nós**: Em HTML, "nós" referem-se a elementos que podem ser pais ou filhos, dependendo da sua posição na árvore do DOM (Document Object Model).

  - **Exemplo**:
    ```html
    <div> <!-- Pai -->
      <p>Este é um parágrafo.</p> <!-- Filho -->
    </div>
    ```

## 4. Cabeçalho (`head`)
- **Tag**: `<head>`
- **Descrição**: Contém metadados e informações sobre o documento.

  - **Meta Tags**:
    - **Tag**: `<meta charset="UTF-8">`
      - **Descrição**: Define a codificação de caracteres para garantir a correta exibição de caracteres especiais.
    - **Tag**: `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
      - **Descrição**: Ajusta a visualização para diferentes tamanhos de tela, especialmente em dispositivos móveis.
  
  - **Título**:
    - **Tag**: `<title>`
      - **Descrição**: Define o título da página, exibido na aba do navegador.

## 5. Corpo (`body`)
- **Tag**: `<body>`
- **Descrição**: Contém o conteúdo visível da página web, como texto, imagens e links.

## 6. Tipos de Tags e Elementos

### 6.1 Tags de Abertura e Fechamento
- **Descrição**: Tags de abertura e fechamento, com o conteúdo situado entre as tags.
  - **Exemplo**:
    ```html
    <div>
        <p>Texto dentro de uma div.</p>
    </div>
    ```

### 6.2 Tags de Fechamento
- **Descrição**: A maioria dos elementos HTML requerem uma tag de fechamento para indicar o fim do conteúdo.
  - **Exemplo**: 
    ```html
    <p>Este é um parágrafo.</p>
    ```
  - **Tag de Fechamento**: `</p>`

### 6.3 Tags de Auto-Fechamento
- **Descrição**: Existem elementos HTML que não requerem uma tag de fechamento porque são auto-contidos.
  - **Exemplo**:
    ```html
    <img src="imagem.jpg" alt="Descrição da imagem">
    ```
  - **Descrição**: `<img>` é um elemento auto-fechado que não requer uma tag de fechamento.

## 7. Tipos de Elementos HTML

### 7.1 Estrutura Semântica
- **Tag**: `<header>`
  - **Descrição**: Contém elementos introdutórios e de navegação.
- **Tag**: `<footer>`
  - **Descrição**: Contém informações adicionais, geralmente no final da página.
- **Tag**: `<section>`
  - **Descrição**: Define seções temáticas do conteúdo.
- **Tag**: `<article>`
  - **Descrição**: Representa conteúdo independente e autocontido.

### 7.2 Estrutura de Conteúdo
- **Tag**: `<h1>`, `<h2>`, `<h3>`, etc.
  - **Descrição**: Define os níveis de cabeçalhos, com `<h1>` sendo o mais importante e `<h6>` o menos importante.
- **Tag**: `<p>`
  - **Descrição**: Define um parágrafo de texto.
- **Tag**: `<ul>`
  - **Descrição**: Define uma lista não ordenada.
- **Tag**: `<ol>`
  - **Descrição**: Define uma lista ordenada.
- **Tag**: `<li>`
  - **Descrição**: Define um item dentro de uma lista, seja ordenada ou não ordenada.

### 7.3 Imagens e Mídia
- **Tag**: `<img>`
  - **Descrição**: Insere uma imagem na página. Atributos comuns incluem `src` (caminho da imagem), `alt` (texto alternativo), `width`, e `height`.
- **Tag**: `<video>`
  - **Descrição**: Insere um vídeo na página. Atributos incluem `src` (caminho do vídeo), `controls` (controles de reprodução), `width`, e `height`.

### 7.4 Links e Referências
- **Tag**: `<a>`
  - **Descrição**: Define um link. Atributos comuns incluem `href` (destino do link), `target` (onde o link será aberto), e `title` (informações adicionais exibidas como tooltip).

### 7.5 Formulários
- **Tag**: `<form>`
  - **Descrição**: Define um formulário para coleta de dados.
- **Tag**: `<input>`
  - **Descrição**: Define um campo de entrada. Atributos incluem `type` (tipo de entrada), `name` (nome do campo), e `value` (valor inicial).

### 7.6 Contato e Informações
- **Tag**: `<address>`
  - **Descrição**: Fornece informações de contato, como endereço, telefone e e-mail.

## 8. Atributos HTML
- **Descrição**: Atributos fornecem informações adicionais sobre elementos HTML. Eles são definidos dentro da tag de abertura e geralmente seguem a forma `nome="valor"`.
  - **Exemplo**: 
    ```html
    <a href="https://example.com" title="Exemplo">Clique aqui</a>
    ```

## 9. Semântica HTML
- **Descrição**: Utilizar tags semânticas ajuda a descrever o papel e o significado do conteúdo, melhorando a acessibilidade e a SEO. Tags semânticas incluem `<header>`, `<footer>`, `<section>`, e `<article>`.

## 10. Boas Práticas
- **Descrição**: Manter a estrutura HTML clara e organizada, utilizar tags semânticas apropriadas e garantir a acessibilidade e responsividade.
