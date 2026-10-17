# Regras do projeto: landing page estática

Esta é uma landing page estática. Ela é publicada no WordPress pelo plugin
"Lovable Pages Publisher", que recebe um ZIP com o conteúdo da pasta `site/`.
Siga estas regras em toda tarefa, sem exceção.

## Escopo
1. Tudo da página fica dentro de `site/`. Não crie nem altere arquivos fora de `site/`.
2. Leia `briefing.md` antes de começar. Ele é a fonte de verdade de textos, cores, fontes e seções.
3. Use os textos do briefing exatamente como estão. Não reescreva, não resuma, não invente promessas, preços ou depoimentos.

## Tecnologia
4. Somente HTML, CSS e JavaScript puros. Sem frameworks, sem npm, sem build, sem Tailwind, sem bibliotecas por CDN.
5. A única dependência externa permitida é Google Fonts, via `<link>` no `<head>`.
6. Proibido criar arquivos `.php`.
7. Não crie back-end. Formulários e botões devem apontar para a URL externa indicada no briefing.

## Estrutura de arquivos
8. `site/index.html` é obrigatório e fica na raiz de `site/`.
9. CSS em `site/css/style.css`. JavaScript em `site/js/main.js`, somente se houver interação.
10. Imagens em `site/assets/`. Nomes em minúsculas, sem espaços (ex.: `logo.png`, `hero.jpg`).
11. Todos os caminhos são relativos e sem barra inicial: `css/style.css`, `assets/logo.png`.
    Nunca use `/assets/...`, `http://localhost` ou caminhos absolutos do computador.

## Qualidade
12. Mobile-first e totalmente responsivo. Teste mentalmente em 375px, 768px e 1280px.
13. HTML semântico (`header`, `main`, `section`, `footer`), `lang="pt-BR"`, atributos `alt` nas imagens, contraste legível.
14. Performance: sem imagens gigantes, `loading="lazy"` nas imagens abaixo da dobra, fontes com `display=swap`.

## Cabeçalho obrigatório (`<head>`)
15. Inclua: `charset`, `viewport`, `title`, `meta description`, favicon (`assets/favicon.png`) e Open Graph
    (`og:title`, `og:description`, `og:type`, `og:url`, `og:image`).
    Em `og:url` e `og:image`, escreva `PREENCHER_URL_COMPLETA` (precisam de URL completa, que será preenchida depois).
16. Deixe estes comentários nos locais indicados:
    - dentro do `<head>`: `<!-- META PIXEL AQUI -->` e `<!-- GTM HEAD AQUI -->`
    - logo após abrir o `<body>`: `<!-- GTM BODY AQUI -->`

## Imagens que não foram enviadas
17. Use blocos de cor em CSS ou SVG inline como espaço reservado. Não use imagens de bancos externos.

## Atualizações
18. Em pedidos de ajuste, altere somente o que foi pedido. Não reescreva nem reorganize o restante.

## Ao terminar, sempre informe
- A lista dos arquivos criados ou alterados.
- As imagens que preciso colocar em `site/assets/`, com os nomes exatos.
- Qualquer decisão que você tomou por conta própria.
