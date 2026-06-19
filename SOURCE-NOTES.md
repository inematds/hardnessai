# SOURCE-NOTES — conteúdo por módulo (T2–T5) + troca de cor

Fiel ao vídeo Matt Pocock × David Ondrej. Use como substância dos módulos. Tom INEMA: direto, prático, confiante, didático, PT-BR.

## TABELA DE TROCA DE COR (a partir do exemplar emerald)
Ao replicar `curso/trilha1/modulo-1-1.html` (emerald), troque TODA ocorrência de emerald pela cor da trilha. No fim, faça `grep -c emerald` no seu arquivo → deve dar **0**.

| Trilha | classe Tailwind | nav ativo (rótulo) | light text | light rgb (bg/border) | SVG stroke / forte / fill caixa |
|---|---|---|---|---|---|
| T2 | blue | "Humano" | #2563eb | 37,99,235 | #60a5fa / #3b82f6 / #0e1622 |
| T3 | purple | "Skills" | #7c3aed | 124,58,237 | #c084fc / #a855f7 / #1a1230 |
| T4 | amber | "Avançado" | #92400e | 217,119,6 | #fbbf24 / #f59e0b / #1f1604 |
| T5 | teal | "Soluções" | #0d9488 | 13,148,136 | #2dd4bf / #14b8a6 / #0c1f1c |

Trocas: `text-emerald-400`→`text-COR-400`; `bg-emerald-500/20`→`bg-COR-500/20`; `bg-emerald-500/10`; `border-emerald-500/30`; `hover:bg-emerald-500/30`; `from-emerald-900/30` e `from-emerald-900/40`; `emerald-600`→`COR-600`; `emerald-500`→`COR-500`. No bloco CSS light-mode "acento": troque os valores emerald (#059669 / rgba(5,150,105,…)) pelos da tabela. No nav, a aba da SUA trilha fica ativa (text-COR-400 bg-COR-500/10) e as outras neutras. Mantenha o ciano #38bdf8 nos SVGs. Mantenha `data-inema-track="N"` correto.

REL continua `../..`. O `<script data-inema-manifest>` e o anti-FOUC são COPIADOS VERBATIM do exemplar (idênticos em toda página). `data-accent` no anti-FOUC pode ficar 'emerald' (default global) — não impacta a cor da página, que vem das classes Tailwind.

---

## T2 — Habilidades Humanas (blue 🧠)
**2-1 ♟️ Tático × Estratégico** — 1)Ousterhout e os dois modos 2)Programação tática 3)Programação estratégica 4)Por que a IA dominou o tático 5)Subir de nível 6)O general no topo.
John Ousterhout, "A Philosophy of Software Design": **tático** = o dia a dia — escrever código, sintaxe, achar bugs, criar commits. **estratégico** = ganhar a guerra, não a batalha; pensamento de longo prazo; como o codebase deve ficar; aumentar velocidade; o general no topo. A IA "comeu" a programação tática (faz mais barato e melhor). Você precisa ser ótimo no estratégico pra extrair o máximo da frota infinita de programadores táticos (a IA). Aplicar: gaste seu tempo em arquitetura, velocidade, roadmap.

**2-2 📈 Suas skills são o teto** — 1)O efeito multiplicador 2)Sênior 10x 3)Júnior ganha pouco 4)Skill baixa achata a IA 5)Upskill em você 6)Crescer o teto.
"Suas habilidades são o teto do que a IA consegue." A IA torna seniores 10x melhores; juniores ganham só um empurrãozinho; não compensa contratar muitos juniores. Ficar bom com IA = ficar bom no seu domínio. Um professor melhor usa IA pra ensinar melhor. Aplicar: melhorar você é melhorar a IA (multiplicador).

**2-3 🧩 Conhecimento × Habilidade × Sabedoria** — 1)Conhecimento: entender 2)Habilidade: músculo 3)Sabedoria: quando 4)Sabedoria precisa de contexto 5)Empacotar os dois primeiros 6)O que não dá pra delegar.
**Conhecimento** = entendimento fundamental na cabeça. **Habilidade** = ter feito muitas vezes, memória muscular. **Sabedoria** = saber QUANDO fazer, como encaixa no mundo real; quase impossível sem fazer no contexto exato (pra ser como alguém da Anthropic, você precisaria ir à Anthropic pra ganhar a sabedoria). Dá pra empacotar conhecimento+habilidade em skills reutilizáveis; sabedoria não. Aplicar.

**2-4 📦 Fundamentos de delegação** — 1)Partes difíceis 2)Escopo nítido 3)Interfaces 4)Testes e cenários 5)Doc suficiente 6)Delegar como a um júnior.
Iguais a delegar pra júnior/pleno: desenhar as partes difíceis na frente; escopar muito bem; pensar nas interfaces entre módulos; cenários de teste e bons testes; um codebase fácil de trabalhar; documentação suficiente que aponta a IA pros lugares certos. Aplicar.

**2-5 🎙️ Comunicação & ditado** — 1)Verbalizar a visão 2)Ditado como velocidade 3)Brain→tokens→brain 4)A skill de comunicar 5)Ferramentas de dictation 6)Treinar a fala.
Ditado é "overpowered" — "a velocidade com que você joga tokens do cérebro pra fora e de volta pra dentro". Matt é falante fluido; usa Whisper Flow. Comunicar/falar é ridiculamente overpowered no mundo dev. É uma skill que dá pra treinar. Aplicar: verbalizar a visão, usar dictation.

**2-6 🧭 Você no controle do produto** — 1)IA ruim em ideia original 2)Você escolhe as features 3)Pergunte o que remover 4)Product design não mudou 5)Falar com clientes 6)Negócio com IA.
A IA é notoriamente ruim em ideias originais. Você escolhe as features; "você deve estar no comando do produto"; precisa da visão, do porquê, do problema que resolve. Pergunte à IA o que REMOVER, como simplificar, melhorar a UX — não "qual a próxima grande feature". Negócio: fundamentos não mudaram — falar com clientes, descobrir o que precisam, fazer protótipos; livros de product design continuam valendo; a IA só dá vantagem na execução. Aplicar.

---

## T3 — Habilidades de IA / Skills (purple 🧰)
**3-1 🧬 Anatomia de uma skill — Procedure × Ability** — 1)O que é uma skill 2)Frontmatter e corpo 3)Procedures 4)Abilities 5)As duas portas 6)Qual usar quando.
Dois tipos. **Abilities** = o MODELO invoca sozinho (ex.: padrões de código — o agente puxa "padrões React", lê, sabe "não usar useEffect"). **Procedures** = VOCÊ invoca pra fazer o modelo se comportar de um jeito (ex.: grill-me, two-PRD). Matt prefere procedures (humano no volante, não delegar o pensamento). Aplicar: escolha pelo quem-invoca.

**3-2 🫥 Custo de contexto da skill** — 1)A descrição vaza 2)100 skills 3)disable model invocation 4)Conhecimento no humano 5)Skills enxutas 6)Auditar o que vaza.
Cada skill VAZA sua descrição no context window; 100 skills = 100 descrições. `disable model invocation: true` → descrição não vaza (skill "engineering zoom out", só invocável pelo usuário). Matt prefere esconder a maioria das descrições e manter o conhecimento no humano. Aplicar: esconder abilities, skills enxutas.

**3-3 🎓 A Teach skill por dentro** — 1)Stateful × stateless 2)mission.md 3)Learning record 4)Lições em HTML 5)Estado local que lembra 6)Recriar o conceito.
Skill **stateful** (vs stateless). Salva estado local: checa workspace vazio; cria `mission.md` (quem é, o que quer construir, por que importa, como é o sucesso); learning record (lista do que aprendeu, missão, ponto de partida, ZDP, estimativas); reference cheat sheet; lições em **HTML** (ricas, abrem no browser — terminal é brutal); personalizado (checa seu setup, ex.: git instalado). Um professor lembra o que você fez. Aplicar: recriar o conceito (lição HTML, estado local) — no INEMA dark, não no papel claro.

**3-4 🌳 Ensino que retém** — 1)ZDP 2)Conhecimento como grafo 3)Caminho linear 4)Quizzes e recall 5)Spaced repetition 6)Personalização.
Princípios: **zona de desenvolvimento proximal**; conhecimento como um grafo/floresta que você explora, e a skill cria um **caminho linear** por ele; quizzes/recuperação ("storage strength", spaced repetition) são absurdamente eficazes; "aprender = te orientar no mundo, te colocar num lugar novo". Personalização. Aplicar.

**3-5 🔬 Grill-me & skills adversariais** — 1)O que faz 2)Substituir plan mode 3)Curta e poderosa 4)Alinhar antes de codar 5)Shared understanding 6)Adaptar pra você.
grill-me transforma o modelo em **entrevistador adversarial** — faz perguntas, levanta ideias que você não considerou, até chegar a entendimento compartilhado. 4-5 frases, absurdamente eficaz. Substitui o plan mode: "aqui está minha ideia, me entreviste, vamos eliminar estranhezas antes de implementar". É uma procedure. Aplicar.

**3-6 🔗 Encadear skills + DRY humano** — 1)grill-me→PRD→issues 2)Procedures em sequência 3)Você no volante 4)Repetiu 3x? Vira skill 5)Distribuir pro time 6)Contribuir de volta.
Fluxo do Matt: grill-me → escrever um PRD (two-PRD) → transformar o PRD em issues individuais (to-issues) pra resolver. Você no volante; não delegar o pensamento. DRY: como uma função repetida 3× extraída pra função compartilhada — pegue "já fiz esse plano 100 vezes" e vire uma skill, distribua pro time, todos planejam igual, contribuem de volta. Elevar o piso do que engenheiros conseguem. Aplicar.

---

## T4 — Técnicas Avançadas (amber 🛰️)
**4-1 🕹️ Human-in-the-loop × AFK** — 1)Human-in-the-loop 2)O que é AFK 3)O destravamento 4)Quando ficar no loop 5)Permissões e fricção 6)Dois, três, quatro de você.
**Human-in-the-loop** = você junto do agente, conversando, descobrindo (planejar, implementação complexa, trabalho sem escopo). **AFK** = away from keyboard, dispara e ele vai. "O momento em que descobri o AFK foi quando entrei de verdade no AI coding" — aumentou muito o output; ao se remover de permissões/perguntas → dois/três/quatro/cinco de você. Aplicar.

**4-2 📦 Paralelizar & sandboxes** — 1)Por que paralelizar 2)Risco sem sandbox 3)Sand Castle 4)Docker/Podman 5)Vercel sandboxes 6)Frota em paralelo.
Sem sandbox o agente faz coisa estranha (apagar o home, exfiltrar env vars pra sites ruins). **Sand Castle** = ferramenta que o Matt construiu pra rodar agentes em sandboxes (Docker/Podman) ou Vercel sandboxes (remoto), puxando os commits de volta pro local. Paralelizar vários agentes na sua máquina ou remoto. Aplicar.

**4-3 ⚙️ GitHub Actions + agentes** — 1)Agentes em CI 2)Review action 3)Labels que disparam 4)PR como saída 5)Sem travar o local 6)Montar a sua.
Matt roda agentes via Sand Castle no GitHub Actions. A **review action** roda num PR: faz checkout do branch, roda o agente de review (um prompt local), type check + lint, responde "tá bom". Labels (`agent:explore`, `agent:implement`, `agent:in-progress`) disparam trabalho; qualquer dev pode pôr um label e disparar. PR como saída. Aplicar: monte sua review action.

**4-4 🧮 Loops × Filas** — 1)O Ralph loop 2)Loop ≠ resposta 3)A fila de tarefas 4)Triagem e escopo 5)O rei medieval 6)Múltiplos nós.
**Ralph loop** (Geoffrey Huntley, 14 de julho): um while loop passando o prompt pro claude code de novo e de novo. Matt: não precisa rodar como loop; o que você precisa é o agente AFK pegar uma tarefa específica. Pense em **filas**, não loops — o backlog de tarefas; triagem, escopo, implementa, review; sai da fila quando o PR é mergeado. Vários nós tiram da fila (como times de dev). Analogia do **rei medieval**: ministro numa região distante em loop (pode dar errado) vs o rei com uma fila de problemas, priorizando (50 bugs, 3 críticos primeiro). Aplicar.

**4-5 ♻️ Sistemas auto-melhoráveis** — 1)Não precisa do modelo caro 2)Cron de security 3)Telemetria→issue→fix 4)Causa raiz 5)Loops de auto-melhoria 6)Revisar o sistema.
Você não precisa do modelo caro pra achar bugs profundos — rode um cron diário que faz security review numa parte nova do repo, com modelo mais barato + harness/prompt certo. "Se roubam sua bike, compre um cadeado." Descubra POR QUE o bug aconteceu, corrija a causa raiz. Construa sistemas que se checam (test suites, reviews, refactor). Telemetria/Sentry → cria issue → agente explora (dado estruturado: corrige já ou precisa de humano?) → implementa → review → auto-merge ou ping. Aplicar.

**4-6 🎬 Checkpoints & review fluido** — 1)O que o review dá 2)Empurrar pra direita 3)Quando remover o humano 4)Quem revisa o agente 5)Vídeo + TTS 6)Review mais rápido com IA.
O que o review te dá: bloquear coisas perigosas (segurança, vazamento) + insight do seu sistema (fez bom trabalho? melhora o harness com o tempo). Empurre os checkpoints human-in-the-loop pra mais perto da saída final. Remova alguns (refactor interno que não muda comportamento) mas "quem revisa a IA que revisa?" — ainda cheque alguns PRs que o agente diz estarem ok. Revise o **sistema** que produz o código, não só o código. Torne o review fluido: a IA grava um vídeo walkthrough da mudança + narração TTS sobreposta no PR. Use IA pra ajudar a revisar. Aplicar.

---

## T5 — Soluções Prontas pra Copiar (teal 📋)
**5-1 🧹 O reset de 2 passos** — 1)Por que resetar 2)Deletar tudo 3)Observar o agente puro 4)Recamadar com procedures 5)Trazer só o que falta 6)Customizar.
Conselho de fechamento do Matt: delete toda skill, plugin, MCP server, claude.md, agents.md; volte ao blank slate; observe o agente (todo mundo incha o contexto). Depois recamade por cima, como procedures (não abilities), coisas que VOCÊ decide; instale de forma customizável pra experimentar; traga de volta só o que sentir falta (ex.: brainstorming do superpowers). Aplicar: passo a passo do reset.

**5-2 🔍 grill-me + 10 decisões** — 1)A skill grill-me (texto) 2)O prompt das 10 decisões 3)"Me entreviste até 98%" 4)Quando usar 5)Adaptar 6)Erros comuns.
Texto da grill-me: "Me entreviste implacavelmente sobre cada aspecto deste plano até chegarmos a um entendimento compartilhado. Percorra cada ramo da árvore de decisão, resolvendo dependências uma a uma. Para cada pergunta, dê sua resposta recomendada. Faça uma pergunta de cada vez. Se uma pergunta pode ser respondida explorando o codebase, explore." O prompt das 10 decisões (David): "descreva minha visão, liste as 10 decisões mais consequentes [design/arquitetura/produto] que vão moldar este projeto e me entreviste até entender 98%." Aplicar: cole no início do projeto. Inclua estes textos em **box de código mono copiável**.

**5-3 🔗 Pipeline grill-me → PRD → issues** — 1)Visão geral 2)grill-me 3)two-PRD 4)to-issues 5)Encadeamento 6)Onde fica o humano.
grill-me (alinhar) → two-PRD (documento de requisitos de produto) → to-issues (quebrar o plano/PRD em issues "independently-grabbable" via vertical slices / tracer bullets). Onde o humano permanece. Aplicar.

**5-4 🛰️ Setup AFK completo** — 1)Claude Code + Opus 4.8 medium 2)AFK via sandbox 3)Sand Castle setup 4)Paralelizar com segurança 5)Puxar commits 6)Seu setup mínimo.
Claude Code + Opus 4.8 effort medium pra planejar + alguma implementação local; a maior parte AFK via Sand Castle (Docker/Podman/Vercel sandboxes); GitHub Actions; puxar commits de volta. Matt em geral não se preocupa com modelos. Aplicar: setup AFK mínimo.

**5-5 🤖 Action de review + cron de security** — 1)Esqueleto da Action 2)checkout→type check→review 3)Comentar no PR 4)Cron diário rotativo 5)Dado estruturado do explore 6)Auto-merge com cautela.
Esqueleto de GitHub Action (roda no PR: checkout → type check → roda o prompt do agente de review → comenta). Cron diário de security review, rodando numa parte nova do repo, modelo mais barato. Dado estruturado do explore (corrige já / precisa de humano). Auto-merge com cautela (ainda revise alguns). Aplicar: copie os esqueletos. Use **boxes de código mono** (YAML da Action / bash do cron).

**5-6 🎥 Review fluido + onde achar** — 1)Vídeo + TTS 2)Otimizar review humano 3)mattpocock/skills 4)aihero.dev/skills 5)npx skills latest add 6)Os 2 primeiros passos hoje.
Vídeo walkthrough + TTS no PR; otimizar o review humano, usar IA pra revisar. Onde achar: github.com/mattpocock/skills; aihero.dev e aihero.dev/skills; `npx skills latest add` (escolher a teach skill). Os 2 passos de hoje: (1) deletar tudo → blank slate → observar; (2) recamadar procedures que você decide, delegar a implementação a agentes AFK. Aplicar.
