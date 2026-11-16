# projeto-integrador-frontend-Arthur-Melo
O objetivo desse projeto é desenvolver um website informativo sobre o conflito Russo-Ucrâniano, mantendo as boas práticas do desenvolvimento em HTML

# Avaliação por Pares - Aulas 1 a 6

**Revisor:** Ryan Marques Monteiro Falcão
**Data da revisão:** 16/11/2026
**Projeto avaliado:** projeto-integrador-frontend-Arthur-Melo
**O que olhei:** a branch `main` (aulas 1 a 5) e a branch `refatoracao-css` (aula 6)
---

## Aula 1 - Git e GitHub

| Critério | Resultado |
|---|---|
| Repositório público e documentado | Atende Plenamente |
| Histórico de commits | Atende Plenamente |
| Uso de branch e Pull Request | Atende Plenamente |
| .gitignore presente | Atende Plenamente |

O repositório é público e o README explica que o projeto é um site informativo sobre o conflito Russo-Ucraniano. Os commits da maior parte do trabalho descrevem bem o que foi feito, como "feat: semântica HTML, formulário e reorganização". Os PRs #1, #2 e #3 saíram de branches separadas da main. O `.gitignore` tem `node_modules/` e `.env`.

---

## Aula 2 - Conceitos Fundamentais da Web

| Critério | Resultado |
|---|---|
| HTML mínimo válido | Atende Plenamente |
| Página abre sem erros | Atende Plenamente |
| Meta tags básicas | Atende Plenamente |

O arquivo tem `<!DOCTYPE html>`, `<html>`, `<head>` e `<body>` certinhos. Os caminhos das imagens e do vídeo existem no repositório. `charset` e `viewport` estão no `<head>`.

---

## Aula 3 - HTML5 - Semântica e Formulários

| Critério | Resultado |
|---|---|
| Elementos semânticos | Atende Plenamente |
| Labels associados aos campos | Atende Plenamente |
| Validação nativa usada | Atende Plenamente |

O site usa `header`, `main`, `section` e `footer` em vez de `div` para tudo. (O `nav` só aparece na branch nova.) Todos os campos do formulário têm `label` ligado por `for` e `id`. A idade usa `type="number"`, e o nome e as perguntas obrigatórias usam `required`.

---

## Aula 4 - HTML5 - Recursos Multimídia

| Critério | Resultado |
|---|---|
| Fallback de formato | Atende Plenamente |
| Atributo controls presente | Atende Plenamente |
| preload configurado com critério | Atende Plenamente |

O vídeo tem dois formatos (`mp4` e `webm`), tem `controls` e não tem autoplay. O `preload="metadata"` foi usado com um comentário explicando o motivo, o que achei muito bom.

A avaliação da Aula 4 que está no README ("Não atende" nos três itens) é de 30/08. O vídeo só foi adicionado em 20/09 (commit `d5bc64f`), então ela se refere a uma versão anterior. Também não encontrei PR para a Aula 4, e esse trabalho entrou direto na main.

---

## Aula 5 - HTML5 - Recursos Gráficos (Canvas/SVG)

| Critério | Resultado |
|---|---|
| Escolha da tecnologia justificada | Não Atende |
| Elemento renderiza corretamente | Não Atende |
| Acessibilidade básica em SVG | Não Atende |

Não encontrei nenhum `<svg>` ou `<canvas>` no projeto, nem PR dessa aula. Por isso não consegui verificar os três critérios.

---

## Aula 6 - CSS3 - Sintaxe, Seletores e Box Model

| Critério | Resultado |
|---|---|
| Seletores eficientes | Não Atende |
| Box model consistente | Não Atende |
| CSS organizado | Não Atende |

O `index.html` da branch `refatoracao-css` está ligado a um `style.css`, mas esse arquivo não está no repositório. Ao abrir a página ela aparece sem estilo, então não deu para verificar nenhum dos três critérios. Também não encontrei PR dessa branch.

Meu palpite é que o `style.css` ficou só no seu computador.

---

## O que gostei
- O HTML está bem organizado e a semântica está bem aplicada.
- As imagens têm texto alternativo.
- O comentário explicando o `preload` mostra que você entendeu o motivo da escolha.
- A ideia da linha do tempo com botões de ano é criativa. Estou curioso para ver como fica com o CSS.

## Sugestões
1. Subir o `style.css` e abrir o PR da Aula 6.
2. Abrir PR também para as próximas aulas. A Aula 4 entrou direto na main.
3. O `id="não"` do botão de rádio está com acento. Talvez seja melhor usar `nao`.
4. Os botões "Sim" e "Não" do formulário não têm `value`, então o envio não diferencia as duas respostas.
5. A linha do tempo, as visões da Rússia e da Ucrânia e o vídeo estão fora do `<main>`.
6. Os vídeos são pesados (cerca de 25 MB e 34 MB). Se o site ficar lento, talvez valha comprimir.
7. Commits menores ajudam a entender o que mudou. O último juntou navbar e linha do tempo num commit só.
