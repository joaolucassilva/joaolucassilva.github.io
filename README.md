# JL Soluções em TI

Landing page estática (HTML + CSS, sem etapa de build) publicada no Cloudflare Pages.

## Publicar no Cloudflare Pages

1. No painel do Cloudflare: **Workers & Pages → Create → Pages → Connect to Git** e escolha este repositório.
2. Configuração de build:
   - Framework preset: **None**
   - Build command: *(vazio)*
   - Build output directory: `public`
3. Salve e faça o deploy. Depois, em **Custom domains**, aponte o seu domínio.

Sem Git: `npx wrangler pages deploy public --project-name jl-solucoes`.

## Estrutura

- `public/index.html` – a landing page
- `public/404.html` – página de erro (usada automaticamente pelo Pages)
- `public/_headers` – cabeçalhos de segurança e cache do Cloudflare
- `public/robots.txt`, `public/favicon.svg`

Para trocar o WhatsApp, procure por `5532998417455` no `index.html`.
