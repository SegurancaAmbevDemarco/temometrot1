# Termômetro de Segurança T1 (versão GitHub)

Mesma aplicação do artifact, gravando os dados em arquivos JSON na pasta `data/` deste repositório.

## Publicar
1. Crie um repositório (privado recomendado) e envie estes arquivos na raiz.
2. Ative o GitHub Pages (branch `main`, pasta raiz).
3. Abra a página, clique em **GitHub**, informe dono, repositório, branch (`main`) e pasta (`data`).
4. Para gravar, gere um token fine-grained só para este repositório com **Contents: Read and write** e cole no campo Token. Ele fica só no navegador (localStorage) e nunca vai para o código.

Cada gravação (carregar bases, salvar apuração, alterar limiares) vira um commit.

## Dados
- `data/index.json` lista os meses com resultado, valores manuais e bases.
- `data/results/AAAA-MM.json`, `data/overrides/AAAA-MM.json`, `data/config/scoring.json` (limiares por mês), `data/inputs/AAAA-MM/*.json`.
- O histórico fev–ago (totais e posições oficiais) e as bases de ago e set já vêm embutidos no `index.html`.
