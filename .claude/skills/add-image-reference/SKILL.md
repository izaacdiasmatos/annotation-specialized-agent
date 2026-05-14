---
name: add-image-reference
description: Instruções para adicionar imagens como referência ao arquivo de anotações do curso Claude Code.
user-invocable: true
---

Quando uma imagem deve ser adicionada como referência ao arquivo `Anotações`, aplique estas regras:

- Use `Image-Reference-Example.md` como template genérico para qualquer imagem.
- Insira a imagem diretamente no bloco apropriado do arquivo `Anotações`.
- Use sintaxe Markdown relativa:
  - `![Texto alternativo](./images/nome-da-imagem.png)`
- Não adicione texto descritivo extra quando o usuário pedir apenas o anexo da imagem.
- Deixe a imagem visualmente separada do restante do bloco.
- Garanta que a pasta `images/` exista e o caminho seja relativo ao workspace.