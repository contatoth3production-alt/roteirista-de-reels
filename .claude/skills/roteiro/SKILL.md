---
name: roteiro
description: Escreve 3 roteiros de Reels (ou TikTok e Shorts) no tom da marca, com gancho, falas por bloco, o que aparece na tela, legenda pronta e um teleprompter em HTML para gravar. Use quando a pessoa pedir roteiro, ideia de vídeo, gancho, legenda de Reels ou digitar /roteiro.
---

# Roteiro de Reels

## 1. Antes de escrever
- Leia `marca/marca.md`. Se não existir, pare e faça a entrevista do `CLAUDE.md` primeiro.
- Descubra três coisas (pergunte só o que não estiver claro, uma pergunta por vez):
  - **Tema.** Se a pessoa não tiver, sugira 5 temas a partir das dores e desejos do cliente que estão na marca, numerados, e deixe ela escolher.
  - **Objetivo.** Atrair gente nova, fazer salvar, ou vender (chamar no WhatsApp, comentar uma palavra).
  - **Duração.** Padrão: 30 segundos.

## 2. A conta do tempo
- Fala natural = **2,5 palavras por segundo**. 30 s ≈ 75 palavras. 45 s ≈ 110 palavras. 60 s ≈ 150 palavras.
- Conte **por bloco** e escreva a contagem ao lado de cada fala. Some no fim. Contar bloco a bloco evita erro.
- Número conta como é falado: "4,9" = quatro vírgula nove (3 palavras); "2021" = dois mil e vinte e um (5 palavras).
- Divisão do tempo, em proporção: gancho até 10%, tensão uns 20%, virada uns 45%, prova (opcional) uns 10%, chamada uns 15%. Em 30 s: gancho 0 a 3 s, tensão 3 a 9 s, virada 9 a 22 s, prova 22 a 25 s, chamada 25 a 30 s.

## 3. A estrutura (todo roteiro segue)
1. **Gancho (até 3 s, no máximo 8 palavras).** É o bloco 1 do roteiro. Uma frase que para o dedo. Nunca comece com "Oi, gente" nem com o nome da marca. Tipos que funcionam:
   - número da sua prova ("[número] clientes me fizeram a mesma pergunta.");
   - crença desafiada ("Treinar todo dia não te faz emagrecer mais rápido.");
   - pergunta que dói ("Quanto você perdeu esse mês por demorar pra responder?");
   - antes e depois ("Essa vitrine não vendia nada às terças.");
   - o erro ("O erro que faz o cliente sumir depois do orçamento.").
   Os exemplos acima mostram o formato. Escreva o gancho com o assunto e a prova da marca, nunca copiando os exemplos.
2. **Tensão.** O problema como ele aparece na vida real do cliente.
3. **Virada.** O que muda, o que fazer, o jeito certo. Uma ideia só.
4. **Prova (opcional).** Um número, um caso, um bastidor. Só o que estiver na marca.
5. **Chamada.** Uma ação só e específica: "comenta [PALAVRA] que eu te mando a tabela", "chama no WhatsApp do perfil". Nunca "saiba mais".

Uma etapa pode ocupar mais de um bloco. Marque a etapa de cada bloco no roteiro.

## 4. Entregar 3 versões
Escreva 3 roteiros com **ganchos de tipos diferentes**:
- **A · provocativo** (crença desafiada ou erro);
- **B · racional** (número ou passo a passo);
- **C · emocional** (história ou antes e depois).

Formato de cada um (é o que você mostra na conversa):

````
### Roteiro A · provocativo · ~30 s (74 palavras)

1. (gancho) fala do bloco 1 · 6 palavras
   [tela: o que aparece: rosto, close no produto, texto na tela...]
2. (tensão) fala do bloco 2 · 10 palavras
   [tela: ...]
...

**Legenda** (pronta para copiar):
```text
1ª linha = o gancho.
2 a 4 linhas curtas.
A mesma chamada do vídeo.
#ate #cinco #hashtags
```

**Dica de gravação:** uma dica prática (luz, ângulo, o que mostrar).
````

Regras de escrita:
- Um bloco = uma respiração (no máximo 2 frases curtas).
- Escreva como a pessoa fala, usando o tom e as frases da marca. Leia em voz alta na cabeça: se travar, reescreva.
- Respeite as palavras proibidas da marca.
- Nada de número, depoimento ou resultado inventado. Se a marca não tem uma história real para o roteiro emocional, use uma cena hipotética e deixe claro que é cena ("Imagina..."), nunca como caso real. Na dica de gravação, sugira usar um antes e depois real.
- Se uma frase da marca prometer resultado sem prova, use como opinião do dono ("eu sempre digo que...") ou pergunte antes.

Depois dos três, pergunte: "Qual você quer gravar? Posso ajustar o gancho, encurtar ou mudar o tom."

## 5. Salvar o escolhido e montar o teleprompter
Quando a pessoa escolher:
1. Crie a pasta `roteiros/AAAA-MM-DD-tema-curto/`: data de hoje, tema em minúsculas, **sem acento**, com hífen (ex.: `2026-11-03-sofa-antes-das-festas`).
2. Salve `roteiro.md` com: no topo, data, tema, objetivo e duração; depois o roteiro escolhido no formato acima, a legenda e a dica de gravação.
3. Monte `teleprompter.html`: copie `.claude/skills/roteiro/teleprompter-modelo.html` e troque:
   - **todas** as ocorrências de `{{TITULO}}` por "Tema · Roteiro A" (com o tema e a letra certos);
   - `{{BLOCOS}}` por um bloco assim para cada fala:
     `<section class="bloco"><div class="n">BLOCO 1 · GANCHO</div><p>fala do bloco</p><div class="tela">tela: ...</div></section>`
   - Em cada bloco, destaque 1 ou 2 trechos fortes com `<b>...</b>`.
   - Confira no fim: não pode sobrar nenhum `{{` no arquivo.
4. Diga onde ficou e como usar: "Abra `roteiros/.../teleprompter.html` no computador ou num tablet e deixe perto da câmera do celular. O botão Rolar faz o texto subir sozinho. Se quiser abrir no próprio celular, use o navegador (Chrome ou Safari), não a prévia do WhatsApp: na prévia o botão Rolar não funciona."

## 6. Conferir antes de entregar
- [ ] Gancho no bloco 1, até 8 palavras, sem "oi, gente".
- [ ] Uma ideia por vídeo e uma chamada só.
- [ ] Contagem por bloco e duração total mostradas.
- [ ] Tom e palavras da marca; nenhuma palavra proibida.
- [ ] Nenhum número, depoimento ou resultado inventado.
- [ ] Acentuação completa (hashtag pode ficar sem acento).
