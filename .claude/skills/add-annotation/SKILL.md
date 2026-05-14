---
name: add-annotation
description: Skill para adicionar anotações organizadas e formatadas no arquivo `Anotações` de um curso ou estudo específico, seguindo regras de estrutura e estilo para manter a consistência.
user-invocable: true
---

# Composição da Criação de Anotações

Quando o usuário solicitar a adição de uma anotação, siga as regras e o formato descritos abaixo para garantir que o conteúdo seja organizado de maneira clara e consistente no arquivo `Anotações` dentro da pasta do curso ou estudo correspondente.

## Fluxo de Criação de Anotações

1. Identifique qual o curso ou estudo sendo abordado e localize o arquivo `Anotações` correspondente.
2. Caso seja um contexto não existe, crie uma nova pasta no formato `<nome-do-curso-ou-estudo><Annotations>` e dentro dela um arquivo `Anotações` para armazenar as anotações futuras.
3. Identifique o tipo de anotação a ser adicionada baseado na descrição fornecida. Use uma categoria existente ou crie uma nova seção se necessário.
4. Sempre escreva diretamente no arquivo `Anotações` seguindo a estrutura e o estilo já estabelecidos.
Regras para adicionar uma anotação:
5. Siga a organição estrutural do arquivo `Anotações`:
   - Use os cabeçalhos de nível `##` para seções principais e `###` para subseções.
   - Mantenha a formatação consistente com o estilo do arquivo existente.

- Preserve o estilo do arquivo existente:
  - Use `---` para separar blocos quando apropriado.
  - Mantenha o texto limpo e coerente.
  - Não remova ou resuma conteúdo existente sem motivo.
- Se o conteúdo não se encaixar nas seções existentes, crie uma nova seção de nível `###` e adicione subseções com `####` apropriadas.
- Quando o usuário fornecer uma imagem de referência, invoque a skill `add-image-reference` para inserir a imagem usando sintaxe Markdown relativa.
- Se houver imagem de referência, garanta que a imagem fique visualmente separada do restante do bloco e use o padrão de `Image-Reference-Example.md`.
- Quando for necessário, ajuste a numeração ou o título do item (`Exemplo prático 1`, `Dica rápida 1`, etc.) para manter a sequência lógica.

## Formatação das Anotações

1. Cada nota deve começar com um cabeçalho de nível `####` no formato `#### Título — descrição breve`.
  - `Título` é o nome principal do conceito, exemplo prático, dica ou ponto de revisão.
  - `descrição breve` contextualiza o item em poucas palavras.
2. Use listas com `-` para descrever cada propriedade e mantenha a formatação limpa e consistente.

3. Todas as anotações sevem usar as seguintes propriedades quando aplicável:
  - `Conceito:` nome do conceito ou termo principal.
  - `Definição:` explicação clara e direta do que o conceito significa.
  - `Aplicação:` como ou quando usar o conceito na prática; diga para que serve.
  - `Nota prática:` dica rápida de uso, atalho ou recomendação de aplicação.
  - `Exemplo:` detalhe real ou fictício que ajuda a entender o conceito.

## Exemplo de formato de anotação:

### Code Assistant — visão geral do assistente de código
- Definição: assistentes de código que ajudam a revisar, corrigir, completar e explicar trechos de programação.
- Aplicação: usados para acelerar tarefas de desenvolvimento e reduzir erros.

### Para exemplos práticos, utilize:
- `Descrição:` resumo do caso.
- `Situação:` contexto ou problema que gerou o exemplo.
- `Passo-chave:` ação principal tomada.
- `Resultado esperado:` objetivo ou aprendizado do exemplo.

### Para dicas rápidas, utilize:
- `Descrição:` breve explicação da dica.
- `O que lembrar:` ponto principal que deve ser memorizado.
- `Por que é útil:` benefício ou vantagem de aplicar a dica.

### Para revisão, utilize:
- `Descrição:` qual é o ponto a revisar.
- `Resumo:` síntese rápida do conteúdo.
- `Por que é importante:` motivo pelo qual esse ponto merece atenção.

## Imagens de Referência
- Quando uma imagem de referência for informada, adicione após os campos acima com a sintaxe Markdown: `![Texto alternativo](./images/nome-da-imagem.png)`.

Esta skill deve ser usada sempre que o usuário solicitar a adição de uma anotação no arquivo `Anotações`.