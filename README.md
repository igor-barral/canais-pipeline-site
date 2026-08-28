# canais-pipeline-site

Site estático (HTML/CSS puro, sem build) com a página da aplicação, a
Política de Privacidade e os Termos de Uso do **canais-pipeline** — usado
como URLs públicas para a análise/auditoria de apps (TikTok, YouTube/Google
OAuth, etc.).

## Publicar no GitHub Pages

1. Crie um repositório novo no GitHub (pode ser público, ex.: `canais-pipeline-site`).
2. Suba estes arquivos pra branch `main`:
   ```
   git init
   git add .
   git commit -m "Site inicial: app, privacidade e termos"
   git branch -M main
   git remote add origin git@github.com:<seu-usuario>/canais-pipeline-site.git
   git push -u origin main
   ```
3. No GitHub: **Settings → Pages → Source** → selecione a branch `main` e a
   pasta `/ (root)`.
4. O site fica disponível em `https://<seu-usuario>.github.io/canais-pipeline-site/`
   (leva alguns minutos pra ativar na primeira vez).

## URLs pra usar nos formulários de análise

- **App homepage:** `https://<seu-usuario>.github.io/canais-pipeline-site/`
- **Privacy Policy URL:** `.../privacy.html`
- **Terms of Service URL:** `.../terms.html`

## Estrutura

- `index.html` — página da aplicação (o que é, canais operados, como funciona).
- `privacy.html` — Política de Privacidade (escopos do YouTube e do TikTok, retenção, contato).
- `terms.html` — Termos de Uso.
- `styles.css` — estilo compartilhado pelas três páginas.

## Manter atualizado

Se um canal novo for adicionado ao `canais-pipeline` (repo do app), ou um
escopo de OAuth novo passar a ser pedido, atualize a lista de canais em
`index.html` e a tabela de escopos em `privacy.html` de acordo.
