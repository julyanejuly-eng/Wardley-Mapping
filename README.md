# Mapa Foresight CAIXA — Interativo (GitHub Pages)

Este repositório publica um **Wardley Map** simplificado com:
- **6 pilares** na lateral (eixo vertical)
- **Gênese · Custom · Produto · Commodity** no eixo horizontal
- **Pílulas clicáveis** (tendências) com painel de detalhes
- **Drag-and-drop** para movimentar as tendências e copiar as posições
- **Grade completa** (horizontal + vertical) **apenas na área interna** entre os eixos

## Como publicar (Pages)
1. Vá em **Settings → Pages** e escolha:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
   - **Save**
2. Abra o link gerado (`https://SEU_USUARIO.github.io/SEU_REPO/`).

## Como editar
- **Posições e textos:** edite o arquivo `data.json`.
  - `x` = maturidade (0 = Gênese ... 1 = Commodity)
  - `y` = visibilidade/viabilidade (0 = baixo ... 1 = alto)
  - campos do painel: `impact`, `risks`, `opportunities`, `status`, `levers` (lista)
- **Cores e pilares:** no `index.html`, altere as variáveis `--c1..--c8` e a lista `PILARES`.

## Dicas
- Arraste as pílulas para testar posições. Clique em **Copiar posições (JSON)** e cole no `data.json` para salvar a nova geometria.
- Se quiser reduzir/aumentar a densidade da **grade**, ajuste `rows` e `cols` na função `drawGrid` dentro do `index.html`.
