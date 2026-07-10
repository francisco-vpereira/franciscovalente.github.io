# Nome do Site

Site pessoal minimalista e leve — HTML e CSS puros, sem frameworks,
sem build step, sem fontes externas (usa as fontes do sistema).

## Estrutura

```
website/
├── index.html              → Página principal (thumbnails dos 3 artigos mais recentes)
├── articles/
│   ├── index.html           → Lista de todos os artigos (foto ligada + resumo)
│   ├── article-1.html       → Artigo individual
│   ├── article-2.html
│   └── article-3.html
├── links/
│   └── index.html           → Lista de links favoritos
├── about/
│   └── index.html           → Página "sobre" (foto 1/3 + texto 2/3)
└── assets/
    ├── css/
    │   └── style.css        → Todo o estilo do site, um único ficheiro
    └── img/
        ├── thumb-1.svg       → Placeholders — substitui pelas tuas fotos
        ├── thumb-2.svg
        ├── thumb-3.svg
        └── portrait.svg
```

## Como usar

1. Substitui as imagens em `assets/img/` pelas tuas fotografias
   (mantém os mesmos nomes, ou atualiza os caminhos no HTML).
2. Edita o texto diretamente em cada `.html` — não há sistema de templates,
   é tudo estático e simples de editar.
3. Para adicionar um novo artigo:
   - copia `articles/article-1.html` para `articles/article-4.html`
   - muda o título, data e texto
   - adiciona uma entrada em `articles/index.html`
   - se for um dos 3 mais recentes, atualiza também `index.html`
4. Abre `index.html` diretamente no browser para pré-visualizar
   (não precisa de servidor).

## Porque é "leve"

- Sem JavaScript, sem frameworks, sem build tools.
- Sem fontes externas — usa as fontes já instaladas no sistema do visitante.
- Imagens de exemplo em SVG (poucos KB); substitui por JPG/WebP otimizados
  quando tiveres fotos reais.
- Um único ficheiro CSS partilhado por todas as páginas.
