# Changelog

Todas as mudanças notáveis deste projeto são documentadas aqui.

## [Não lançado]

### Corrigido
- Botões "Copiar" não respondiam a cliques físicos do mouse nas 3 páginas de atlas. Causa: `.card` usa `backdrop-filter`, que no Chromium cria uma camada de composição que interfere no hit-testing de ponteiro em filhos sem stacking context próprio — o clique era roteado para o card em vez do botão. Corrigido com `position:relative;z-index:1` na regra `.copy`.

### Adicionado
- Acessibilidade: `aria-live` no feedback "COPIADO", `:focus-visible` customizado e `aria-label` descritivo nos botões de cópia, nas 3 páginas de atlas.
- SEO/GEO: `robots.txt`, `sitemap.xml`, `llms.txt`, meta tags Open Graph e Twitter Card, dados estruturados JSON-LD (schema.org) e `<link rel="canonical">` no hub e nas 3 páginas de atlas.

### Alterado
- Compressão lossless dos 3 logos PNG em `assets/` (mesma resolução e aparência, arquivos ~4% menores).
- `Cache-Control` das páginas HTML reduzido de 1h para 5 minutos, para que atualizações de conteúdo cheguem mais rápido aos visitantes.

## [Inicial]

### Adicionado
- Estrutura do projeto: `index.html` (hub de lançamento), três atlas standalone (`CLAUDE_POWER_CODES_ATLAS_PREMIUM.html` com 162 atalhos, `CHATGPT_POWER_CODES_ATLAS_PREMIUM.html` com 111, `GEMINI_POWER_CODES_ATLAS_PREMIUM.html` com 132), design system de referência `Classical` em `_ds/`, `README.md`, `vercel.json` e logos em `assets/`.
