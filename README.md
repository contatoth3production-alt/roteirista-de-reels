# Roteirista de Reels

**Um agente para o Claude Code que escreve os roteiros dos seus Reels no seu jeito de falar.**

Você conta do seu negócio uma vez. Depois é só pedir: ele te entrega **3 roteiros** com gancho, as falas divididas por respiração, o que aparece na tela, a legenda pronta e um **teleprompter** para você gravar no celular.

Feito pela [TH3](https://itsth3time.com.br): é uma versão do agente que escreve os roteiros dos Reels por aqui. Grátis e com o código aberto.

---

## O que ele faz

- **Aprende a sua marca:** faz 8 perguntas (uns 5 minutos) e guarda tudo em `marca/marca.md`.
- **Sugere temas** a partir das dores do seu cliente, se você não tiver ideia.
- **Escreve 3 versões** de cada vídeo, com ganchos diferentes: provocativo, racional e emocional.
- **Conta o tempo:** cada roteiro vem com a duração estimada (2,5 palavras por segundo).
- **Monta o teleprompter:** uma página que rola sozinha, com letra grande, para você ler enquanto grava.
- **Não inventa resultado:** número, depoimento e "antes e depois" só entram se você contou.

## Do que você precisa

- Uma conta no Claude com um plano pago que inclua o Claude Code (Pro ou superior).
- Um computador com Windows ou Mac.
- Não precisa saber programar.

## Como instalar (uns 10 minutos)

1. **Baixe o agente.** Nesta página, clique no botão verde **Code** e depois em **Download ZIP**. Descompacte o arquivo (no Windows: botão direito → Extrair tudo; no Mac: dois cliques) e guarde a pasta `roteirista-de-reels` num lugar fácil, como Documentos.
2. **Abra a pasta no Claude Code.** O jeito mais fácil é pelo app do Claude para computador ([claude.ai/download](https://claude.ai/download)): entre na sua conta, vá na aba **Code** e escolha a pasta `roteirista-de-reels`. Prefere o terminal? Instale o Claude Code pelo [guia oficial](https://claude.com/claude-code) e rode `claude` dentro da pasta.
3. **Confirme que confia na pasta**, se ele perguntar. É isso que deixa o agente salvar os roteiros ali dentro.
4. **Escreva `oi`.** Ele se apresenta e faz as 8 perguntas sobre o seu negócio.
5. **Peça os roteiros:** `faz 3 roteiros sobre [tema]`, ou digite `/roteiro`.

Os roteiros ficam em `roteiros/`. Para usar o teleprompter no celular, mande o arquivo `teleprompter.html` para você mesmo pelo WhatsApp ou e-mail e abra por lá.

## Veja um exemplo

- [A marca de exemplo](marca/marca.exemplo.md) (um negócio fictício de higienização de sofá)
- [Os 3 roteiros que ele entregou](exemplos/3-roteiros.md)
- [O roteiro escolhido](exemplos/roteiro-escolhido.md) e o [teleprompter](exemplos/teleprompter.html) (baixe e abra no navegador)

## Perguntas frequentes

**Preciso pagar pelo agente?** Não. Você só precisa do seu plano do Claude.

**Funciona no ChatGPT?** Ele foi feito para o Claude Code. Mas o método está todo escrito em [`.claude/skills/roteiro/SKILL.md`](.claude/skills/roteiro/SKILL.md): dá para ler e aplicar onde você quiser.

**É seguro?** Ele foi instruído a só ler e escrever arquivos de texto dentro desta pasta. As configurações (`.claude/settings.json`) bloqueiam comandos no computador e acesso a sites, e ele nunca pede senha, chave ou cartão. As suas respostas sobre o negócio ficam no seu computador. Se um dia você subir a sua cópia para o GitHub, o `.gitignore` já deixa a sua marca e os seus roteiros de fora.

**Posso mudar o jeito que ele escreve?** Pode. Edite o `marca/marca.md` (o seu tom, as palavras que você nunca usa, a chamada preferida) ou peça na conversa: "deixa mais curto", "troca o gancho", "mais engraçado".

## Quer o time completo?

O Roteirista é um dos agentes que trabalham na TH3. Lá, cada setor da empresa tem os seus: comercial, atendimento no WhatsApp, fábrica de conteúdo e sites.

Para montar a sua empresa virtual, fale com a Lia, a assistente da TH3: [WhatsApp (11) 94376-1875](https://wa.me/5511943761875?text=Vim%20pelo%20Roteirista%20de%20Reels).
Bastidores toda semana no Instagram: [@checo.ia](https://instagram.com/checo.ia).

---

Projeto independente da TH3. Não é afiliado nem endossado pela Anthropic. Claude e Claude Code são marcas da Anthropic.

Licença MIT: use, adapte e compartilhe à vontade.
