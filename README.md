# Mapa Foresight CAIXA — Painel Fixo (GitHub Pages)

Publica um **Wardley Map** com:
- **6 pilares** na lateral (eixo vertical)
- **Gênese · Custom · Produto · Commodity** no eixo horizontal
- **Pílulas clicáveis** (tendências) com **painel fixo** à direita (conteúdo atualiza ao clicar)
- **Drag-and-drop** para reposicionar tendências
- **Grade interna** (linhas horizontais e verticais) no canvas

## Como publicar (Pages)
1. Em **Settings → Pages**, selecione:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
   - **Save**
2. Abra a URL do Pages (ex.: `https://SEU_USUARIO.github.io/SEU_REPO/`).

## Como editar
- **Posições e textos:** edite `data.json`.
  - `x` = maturidade (0 = Gênese ... 1 = Commodity)
  - `y` = visibilidade/viabilidade (0 = baixo ... 1 = alto)
  - campos do painel: `impact`, `risks`, `opportunities`, `status`, `levers` (lista)
- **Cores e pilares:** no `index.html`, altere as variáveis `--c1..--c8` e a lista `PILARES`.

## Dicas
- **Clique** numa pílula para atualizar o painel fixo.  
- **Arraste** para ajustar posições, e clique em **“Copiar posições (JSON)”** (no canto do canvas) para colar de volta no `data.json`.  
