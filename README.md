# Prestô – serviços autônomos (front-end)

Site estático (HTML/CSS/JS) com PWA. Pronto para a Vercel.

## Publicar
**Pelo GitHub (recomendado):** suba esta pasta em um repositório, entre em vercel.com > Add New > Project, importe o repositório e clique em Deploy. Não precisa de build (Framework Preset: Other).

**Pela CLI:** `npm i -g vercel` e, dentro da pasta, `vercel --prod`.

## Estrutura
- `public/index.html` – app (dados em `PROS`, camada de dados no topo do script)
- `public/manifest.webmanifest`, `sw.js`, `icon.svg` – PWA
- `vercel.json` – cabeçalhos de segurança (CSP, nosniff, frame-ancestors)

## Próximos passos
Backend NestJS + PostgreSQL em outro projeto Vercel/Render/AWS, com JWT, hash argon2 e webhooks de pagamento. Ao integrar, adicione o domínio da API em `connect-src` no `vercel.json`.
