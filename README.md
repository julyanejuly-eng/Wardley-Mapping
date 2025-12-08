# Wardley Mapping (Demo GitHub Pages)

Este repositório publica um site estático via **GitHub Pages** com um mapa simples.
- O arquivo inicial é **`index.html`**.
- Os dados do mapa ficam em **`data.json`**.

## Como visualizar
1. Ative o GitHub Pages em **Settings → Pages → Source: _Deploy from a branch_**, **Branch: `main`**, **Folder: `/ (root)`** → **Save**.
2. Acesse o link gerado (ex.: `https://SEUUSUARIO.github.io/NOMEDOREPO/`).

## Como editar o mapa
1. Abra o arquivo **`data.json`** e clique no ícone de lápis (**Edit**).
2. Ajuste a lista `nodes`:
   ```json
   [
     { "label": "Nome do item", "x": 0.50, "y": 0.65 }
   ]
   ```
   - `x`: posição horizontal (0 = gênesis, 1 = commodity)
   - `y`: visibilidade (0 = baixo, 1 = alto)

3. Clique em **Commit changes**. Atualize a página do site para ver as mudanças.

## Dicas
- O arquivo **`index.html`** precisa ser um **HTML de verdade** (com `<html> ... </html>`). Renomear `.docx`/`.pptx` para `.html` não funciona.
- Se o site abrir com caracteres estranhos, substitua o arquivo **`index.html`** por este aqui e confirme que existe um **`data.json`** válido na raiz.
