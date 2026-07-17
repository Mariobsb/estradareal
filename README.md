# ☀️ Família SOL na Estrada Real

Blog de viagem da Família SOL — julho/2026, Brasília → Paraty pelo Caminho Velho.

## Publicar (primeira vez)

1. No GitHub: **Settings → Pages → Source: GitHub Actions** (uma vez só).
2. Local:
```bash
git clone https://github.com/Mariobsb/estradareal.git
# copie TODO o conteúdo deste zip para dentro da pasta estradareal/
cd estradareal
git add -A && git commit -m "estrutura do blog" && git push
```
3. Aguarde a Action (~2 min): o site sobe em **https://mariobsb.github.io/estradareal**

## Como escrever um dia

- Edite `src/pages/dias/dia-XX.md` (pode ser pelo site do GitHub, até do celular: abra o arquivo → ✏️ → Commit).
- Fotos: suba para `public/fotos/dia-XX/` (GitHub web: Add file → Upload files). Nomeie `capa.jpg` a foto do card.
- Redimensione fotos para ~1600px antes de subir (o site fica rápido). No Windows: selecionar → botão direito → Redimensionar imagens.
- Vídeos: suba no YouTube (não listado) e cole o link no post.

## Rodar localmente (opcional)

```bash
npm install
npm run dev   # http://localhost:4321/estradareal
```

## Estrutura

- `src/pages/dias/*.md` — os 13 posts (um por dia, já com a história preenchida)
- `src/pages/index.astro` — a home com os cards
- `public/guia.html` — o guia offline completo da viagem
- `public/fotos/dia-XX/` — fotos de cada dia
- `.github/workflows/deploy.yml` — publica sozinho a cada push
