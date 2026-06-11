# 💌 Site Dia dos Namorados

## Estrutura

```
site-amor/
├── index.html      ← o site inteiro
├── musica.mp3      ← ADICIONE AQUI (veja abaixo)
└── fotos/          ← 21 fotos + 1 vídeo já otimizados
```

## 🎵 Música (Afrodite — Delacruz)

O site já está preparado: ao clicar no botão "Clica aqui, baby 💌", a música começa automaticamente.

1. Obtenha o MP3 da música (de uma compra digital ou do seu acervo).
2. Renomeie o arquivo para exatamente `musica.mp3`.
3. Coloque na mesma pasta do `index.html`.

Sem o arquivo, o site funciona normalmente — só fica sem som.

## ✏️ Personalizar legendas das fotos

Abra o `index.html` e procure por `SLIDES` (perto do final). Edite o campo `legenda` de qualquer foto:

```js
{src:'fotos/foto02.jpg', legenda:'Nossa primeira viagem 🏝️'},
```

A data do contador está em `DATA_INICIO` no mesmo bloco.

## 🚀 Publicar no GitHub Pages

1. Crie um repositório no GitHub (ex: `feliz-dia-dos-namorados`). Pode ser **público** — o link só será visto por quem você enviar.
2. Na pasta `site-amor`, rode:

```bash
git init
git add .
git commit -m "feliz dia dos namorados ❤️"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/feliz-dia-dos-namorados.git
git push -u origin main
```

3. No GitHub: **Settings → Pages → Source: Deploy from a branch → Branch: main / (root) → Save**.
4. Em 1–2 minutos o site estará em:
   `https://SEU_USUARIO.github.io/feliz-dia-dos-namorados/`

> Alternativa sem terminal: crie o repositório no GitHub, clique em **"uploading an existing file"** e arraste todos os arquivos da pasta (incluindo a pasta `fotos`). Depois ative o Pages do mesmo jeito.

## Railway (opcional)

Se preferir o Railway: New Project → Deploy from GitHub repo → selecione o repositório. Como é site estático, adicione um arquivo `Caddyfile` ou use o template "Static Site". Mas o GitHub Pages é mais simples e gratuito para esse caso.
