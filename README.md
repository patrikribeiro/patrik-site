# Patrik Darlan Ribeiro — Site Profissional

Site estático multipágina para apresentar a atuação profissional de Patrik Darlan Ribeiro em consultoria, docência, estratégia, operações e conteúdo aplicado.

O projeto foi desenvolvido para publicação no GitHub Pages, Netlify ou outra hospedagem estática.

## O que o site inclui

* Página inicial com posicionamento profissional, áreas de atuação, método e contato.
* Página de blog com busca e filtro por categoria.
* Página individual para leitura de cada artigo.
* Arquivo simples para inclusão e edição de artigos.
* Layout responsivo para computador, tablet e celular.
* Identidade visual executiva com azul, grafite, branco e vermelho discreto.
* Botão **E-mail de contato**, sem exibição direta do endereço de e-mail.
* Links para WhatsApp e Instagram.

## Estrutura do projeto

```text
.
├── index.html       # Página inicial
├── blog.html        # Listagem de artigos
├── post.html        # Página de leitura de um artigo
├── posts.js         # Arquivo editável com os artigos do blog
├── .nojekyll        # Compatibilidade com publicação estática
└── README.md        # Este arquivo
```

## Como colocar no GitHub

### Repositório novo

1. Crie um repositório novo no GitHub.
2. Descompacte este projeto no seu computador.
3. Envie os arquivos para a **raiz do repositório**.
4. Confirme o commit.
5. Verifique se `index.html` está diretamente na raiz, e não dentro de outra pasta.

### Repositório existente

Substitua os arquivos atuais pelos arquivos deste projeto e faça um novo commit.

## Como adicionar um artigo ao blog

Todos os artigos ficam no arquivo `posts.js`, dentro de `window.BLOG_POSTS`.

Copie este modelo e altere as informações:

```javascript
{
  slug: "meu-novo-artigo",
  title: "Título do meu novo artigo",
  excerpt: "Resumo curto que aparecerá na listagem do blog.",
  category: "Estratégia",
  dateLabel: "20 out 2026",
  readingTime: "4 min de leitura",
  published: true,
  content: `
    <p>Primeiro parágrafo do artigo.</p>

    <h2>Um subtítulo</h2>
    <p>Desenvolvimento do conteúdo.</p>

    <ul>
      <li>Primeiro ponto</li>
      <li>Segundo ponto</li>
    </ul>
  `
}
```

### Campos do artigo

* `slug`: identificador exclusivo usado no endereço do artigo. Use letras minúsculas e hífens.
* `title`: título principal.
* `excerpt`: resumo exibido na página do blog.
* `category`: categoria usada no filtro.
* `dateLabel`: data exibida para o leitor.
* `readingTime`: tempo estimado de leitura.
* `published`: use `true` para publicar ou `false` para manter o artigo oculto.
* `content`: conteúdo do artigo em HTML simples.

### Tags HTML recomendadas

Dentro de `content`, utilize principalmente:

* `<p>` para parágrafos.
* `<h2>` e `<h3>` para subtítulos.
* `<ul>` e `<li>` para listas.
* `<blockquote>` para uma frase de destaque.
* `<strong>` para dar ênfase a uma expressão.

Depois de salvar o arquivo, faça o commit no GitHub. O novo artigo aparecerá automaticamente quando o site for republicado.

## Publicação no Netlify

### Usando GitHub

1. Acesse o Netlify.
2. Escolha **Add new project**.
3. Selecione **Import an existing project**.
4. Conecte o GitHub e escolha este repositório.
5. Deixe o comando de build vazio.
6. Deixe o diretório de publicação vazio ou use a raiz do repositório.
7. Clique em **Deploy**.

Depois disso, cada novo commit no GitHub poderá gerar uma nova publicação automaticamente.

### Usando upload manual

1. Descompacte o projeto.
2. Acesse o recurso de deploy manual do Netlify.
3. Envie a pasta que contém diretamente `index.html`, `blog.html`, `post.html` e `posts.js`.

## Links de contato

O site exibe somente o texto **E-mail de contato**. O endereço não aparece visualmente na página.

Os demais links configurados são:

* WhatsApp: https://wa.me/5511978757549
* Instagram: https://www.instagram.com/patrikdarlan/

## Tecnologias

* HTML5
* CSS3
* JavaScript puro
* Blog alimentado por arquivo local
* Hospedagem estática compatível com GitHub e Netlify

## Licença

Conteúdo, textos e identidade visual destinados ao uso pessoal e profissional de Patrik Darlan Ribeiro.
