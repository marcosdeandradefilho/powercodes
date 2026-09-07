# Power Codes — Trilogia HTML Premium

Três atlas standalone (Claude, ChatGPT, Gemini) com identidade visual própria por IA, mais um índice de lançamento. Sem build step, sem dependências de servidor — HTML/CSS/JS puro.

## Estrutura

```
index.html                              # índice / hub de lançamento
CLAUDE_POWER_CODES_ATLAS_PREMIUM.html   # atlas Claude (162 atalhos)
CHATGPT_POWER_CODES_ATLAS_PREMIUM.html  # atlas ChatGPT (111 atalhos)
GEMINI_POWER_CODES_ATLAS_PREMIUM.html   # atlas Gemini (132 atalhos)
assets/                                 # logos Power Codes (PNG)
vercel.json                             # config de headers/cache para deploy
```

## Deploy na Vercel

1. Suba esta pasta para um repositório no GitHub.
2. Em [vercel.com/new](https://vercel.com/new), importe o repositório.
3. Framework preset: **Other** (site estático). Build command: nenhum. Output directory: raiz (`.`).
4. Deploy — pronto, `index.html` é servido na raiz automaticamente.

Também funciona em qualquer host estático (GitHub Pages, Netlify, Cloudflare Pages) sem alterações.

## Local

Abra `index.html` direto no navegador, ou sirva a pasta com qualquer servidor estático (`npx serve .`).
