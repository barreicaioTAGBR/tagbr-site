TAGBR SITE - Estrutura para edição
====================================

PASTA: tagbr-site/
├── index.html         ← arquivo principal do site
├── images/
│   ├── logo.webp      ← logo do topo (nav)
│   ├── logo.png       ← versão PNG do logo (fallback)
│   ├── z1.webp        ← página 1 (HOME - hero)
│   ├── z1.jpg         ← fallback JPG da página 1
│   ├── z2.webp        ← página 2 (PRODUTOS)
│   ├── z3.webp        ← página 3
│   ...
│   └── z10.webp       ← página 10 (TUTORIAL)
└── README.txt         ← este arquivo


COMO EDITAR
-----------

1. TROCAR UMA IMAGEM DA PÁGINA:
   - Substitua o arquivo em images/zN.webp (mesma altura x largura)
   - Também substitua zN.jpg com a mesma imagem em JPG

2. MUDAR TEXTO DO MENU (HOME, PRODUTOS, etc):
   - Abra index.html
   - Procure por <div class="nav-links">
   - Edite os textos dentro das tags <a>

3. MUDAR O QUE ACONTECE AO CLICAR NUM BOTÃO DA IMAGEM:
   - Cada botão invisível sobreposto na imagem é um <a class="ob">
   - O href="#sec-N" faz rolar até outra seção
   - href="mailto:email@..." abre o email
   - href="https://..." abre um link externo

4. AJUSTAR POSIÇÃO DE UM BOTÃO:
   - Encontre o <a class="ob"> e mude os valores:
     left: posição horizontal (%)
     top: posição vertical (%)
     width: largura (%)
     height: altura (%)


COMO COLOCAR NO AR (DEPLOY)
---------------------------

Opção gratuita mais fácil (Vercel):
1. Crie conta em vercel.com
2. Arraste a pasta tagbr-site para o painel
3. Em Settings → Domains, adicione www.tagbr.app.br
4. Aponte o DNS do seu domínio pro Vercel

Outras opções grátis: Netlify, GitHub Pages, Cloudflare Pages
