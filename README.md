# klm-hub.github.io

Projeto Astro configurado para deploy automático no GitHub Pages via GitHub Actions.

## Desenvolvimento

```sh
npm install
npm run dev
```

## Build

```sh
npm run build
npm run preview
```

## Deploy

O workflow em `.github/workflows/deploy.yml` roda em todo push para a branch `main` e publica o conteúdo gerado em `dist/` no GitHub Pages.

No GitHub, confirme em `Settings > Pages` que a origem está configurada como `GitHub Actions`.

## Estrutura

- `src/pages/`: páginas do site.
- `public/`: arquivos estáticos servidos na raiz.
- `astro.config.mjs`: configuração do Astro, incluindo a URL do site.

## Observacao

Como este repositório se chama `klm-hub.github.io`, ele está configurado como site raiz em `https://klm-hub.github.io`. Se ele for publicado como project page em outro repositório, adicione a opção `base` no `astro.config.mjs`.
