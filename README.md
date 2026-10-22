# Studio 404 · Moema

Landing page do Studio 404 (Mercure São Paulo Moema Times Square), com reserva via Airbnb.

- Página estática: `index.html` + pasta `images/` (sem build, sem dependências).
- 25 fotos organizadas por ambiente (Sala, Cozinha, Quarto, Banheiro, Prédio, Academia, Lavanderia), com filtros e visualizador em tela cheia (setas do teclado, deslizar no celular, Esc para fechar).
- Bilíngue PT/EN (botão no topo; detecta o idioma do navegador).
- Variante para viajante a trabalho: adicione `?v=exec` à URL.
- Google Analytics `G-QTF5HE0FZC` com os eventos `reservar_airbnb_click` e `galeria_abrir`.

## Estrutura

```
index.html
images/
  flat-1.avif … flat-26.avif   fotos do studio e do prédio
  og.jpg                       imagem de compartilhamento (WhatsApp, Facebook)
```

Para trocar ou incluir fotos, edite a lista `ROOMS` no início do `<script>` do `index.html`.

## Publicar no GitHub Pages

1. Crie um repositório no GitHub e envie `index.html`, `README.md` e a pasta `images/` para a raiz.
2. No repositório: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, pasta `/ (root)`.
3. Em 1–2 minutos o site fica em `https://<usuario>.github.io/<repositorio>/`.

Depois de publicar, troque no `index.html` a linha `og:image` pelo endereço completo (ex.: `https://seudominio.com/images/og.jpg`) para a prévia aparecer ao compartilhar o link.
