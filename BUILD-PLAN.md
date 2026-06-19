# BUILD-PLAN — Curso "HARNESS" (método Matt Pocock)

Fonte de verdade do build. courseId = **`harness`**. Formato **INEMA curso v2**.
Emoji do curso: 🏎️ · Título: **HARNESS — Engenharia Agêntica (o método Matt Pocock)**.
Base: transcrição do vídeo `nQwJVHCtDDY` (David Ondrej × Matt Pocock).

## Decisões travadas
- Assets compartilhados: `assets/learn.css` + `assets/learn.js` via `<link>`/`<script src>` relativo.
  REL: landing = `.` ; trilha index e módulos = `../..`.
- Manifesto idêntico em TODA página (`<script type="application/json" data-inema-manifest>`).
- `<meta name="inema-course" content="harness">` em toda página.
- Agentes REPLICAM o exemplar-ouro (`curso/trilha1/modulo-1-1.html`), não re-derivam do MASTER.
- 27 módulos, 6 tópicos cada (162 tópicos). Heros raster: flux2-klein (não-comercial).
- Referências visuais: `refs/moodboard/` (telas reais do vídeo).

## Cores por trilha
T1 emerald · T2 blue · T3 purple · T4 amber · T5 teal.

## Mapa dos módulos (id · emoji · título · subtítulo punchy · 6 tópicos)

### T1 — Fundamentos do Harness (emerald 🏎️)
- **1-1** 🏎️ Motor × Chassi — *"O modelo não é tudo"*
  1. O que é o harness 2. A analogia da Fórmula 1 3. Por que você controla o harness
  4. O erro de focar no modelo 5. Modelo e harness são 50/50 6. Onde está sua alavanca
- **1-2** ⏳ O Bitter Lesson — *"Não espere o modelo"*
  1. O que é o Bitter Lesson 2. A tentação de esperar a AGI 3. Compute vence otimização (e o limite)
  4. Por que agir agora 5. O equilíbrio de Pocock 6. Aplicar sem cair na armadilha
- **1-3** 🧭 Setup agent-agnostic — *"Fundamentos de 30 anos"*
  1. Manter-se agnóstico 2. O custo de otimizar pra um modelo só 3. Fundamentos que não expiram
  4. O vibe coder que troca de ferramenta toda semana 5. Blindar seu setup 6. Checklist de agnosticismo
- **1-4** 🤝 DX × AX — *"Projete para o agente"*
  1. O que é Agent Experience 2. O overlap DX/AX 3. Guard rails e navegabilidade
  4. Documentação que aponta o caminho 5. O codebase como ambiente do agente 6. Medindo boa AX
- **1-5** 💸 Economia de tokens — *"Codebase fácil = modelo barato"*
  1. Arquitetura reduz tokens 2. Guard rails poupam cabeçadas 3. Quando um modelo mais burro basta
  4. O custo real de um codebase ruim 5. Refatorar pra baratear 6. Métrica: tokens por mudança
- **1-6** 🪟 Context window escasso — *"Cada skill cobra"*
  1. O que vaza no contexto 2. O custo de 100 skills 3. disable model invocation
  4. Bloat de instruções 5. O reset radical (prévia) 6. Higiene de contexto

### T2 — Habilidades Humanas (blue 🧠)
- **2-1** ♟️ Tático × Estratégico — *"A IA comeu o tático"*
  1. Ousterhout e os dois modos 2. Programação tática 3. Programação estratégica
  4. Por que a IA dominou o tático 5. Subir de nível 6. O general no topo
- **2-2** 📈 Suas skills são o teto — *"Você é o multiplicador"*
  1. O efeito multiplicador 2. Por que o sênior ganha 10x 3. Por que o júnior ganha pouco
  4. Skill baixa achata a IA 5. Upskill em você 6. Como crescer o teto
- **2-3** 🧩 Conhecimento × Habilidade × Sabedoria — *"Os três pilares"*
  1. Conhecimento: entender 2. Habilidade: músculo 3. Sabedoria: quando
  4. Por que sabedoria precisa de contexto 5. Empacotar os dois primeiros 6. O que não dá pra delegar
- **2-4** 📦 Fundamentos de delegação — *"Delegar bem"*
  1. Desenhar as partes difíceis 2. Escopo nítido 3. Interfaces entre módulos
  4. Testes e cenários 5. Documentação suficiente 6. Delegar como a um júnior
- **2-5** 🎙️ Comunicação & ditado — *"Falar é overpowered"*
  1. Verbalizar a visão 2. Ditado como velocidade 3. Brain → tokens → brain
  4. A skill de comunicar 5. Ferramentas de dictation 6. Treinar a fala
- **2-6** 🧭 Você no controle do produto — *"A visão é sua"*
  1. IA é ruim em ideia original 2. Você escolhe as features 3. Pergunte o que remover
  4. Product design não mudou 5. Falar com clientes 6. Construir negócio com IA

### T3 — Habilidades de IA / Skills (purple 🧰)
- **3-1** 🧬 Anatomia de uma skill — *"Procedure × Ability"*
  1. O que é uma skill 2. Frontmatter e corpo 3. Procedures (você invoca)
  4. Abilities (o modelo invoca) 5. As duas portas 6. Qual usar quando
- **3-2** 🫥 Custo de contexto da skill — *"Quando esconder"*
  1. A descrição vaza 2. 100 skills, 100 descrições 3. disable model invocation
  4. Conhecimento no humano 5. Skills enxutas 6. Auditar o que vaza
- **3-3** 🎓 A Teach skill por dentro — *"Skill com memória"*
  1. Stateful × stateless 2. mission.md 3. Learning record
  4. Lições em HTML 5. Estado local que lembra 6. Recriar o conceito
- **3-4** 🌳 Ensino que retém — *"ZDP + recall"*
  1. Zona de desenvolvimento proximal 2. Conhecimento como grafo 3. Caminho linear no grafo
  4. Quizzes e recall 5. Spaced repetition 6. Personalização
- **3-5** 🔬 Grill-me & skills adversariais — *"Entreviste-me"*
  1. O que a grill-me faz 2. Substituir o plan mode 3. Curta e poderosa (4-5 frases)
  4. Alinhar antes de codar 5. Shared understanding 6. Adaptar pra você
- **3-6** 🔗 Encadear skills + DRY humano — *"Pipeline de pensamento"*
  1. grill-me → PRD → issues 2. Procedures em sequência 3. Você no volante
  4. Repetiu 3x? Vira skill 5. Distribuir pro time 6. Contribuir de volta

### T4 — Técnicas Avançadas (amber 🛰️)
- **4-1** 🕹️ Human-in-the-loop × AFK — *"Saia do loop"*
  1. Human-in-the-loop 2. O que é AFK 3. O destravamento do AFK
  4. Quando ficar no loop 5. Permissões e fricção 6. Dois, três, quatro de você
- **4-2** 📦 Paralelizar & sandboxes — *"Agentes isolados"*
  1. Por que paralelizar 2. O risco de rodar sem sandbox 3. Sand Castle
  4. Docker / Podman 5. Vercel sandboxes 6. Frota em paralelo
- **4-3** ⚙️ GitHub Actions + agentes — *"AFK na nuvem"*
  1. Agentes em CI 2. Review action 3. Labels que disparam
  4. Pull request como saída 5. Sem travar a máquina local 6. Montar a sua
- **4-4** 🧮 Loops × Filas — *"Fila, não loop"*
  1. O Ralph loop (Huntley) 2. Por que loop ≠ resposta 3. A fila de tarefas
  4. Triagem e escopo 5. O rei medieval 6. Múltiplos nós na fila
- **4-5** ♻️ Sistemas auto-melhoráveis — *"Compre o cadeado"*
  1. Não precisa do modelo caro 2. Cron de security review 3. Telemetria → issue → fix
  4. A causa raiz do bug 5. Loops de auto-melhoria 6. Revisar o sistema
- **4-6** 🎬 Checkpoints & review fluido — *"Review sem dor"*
  1. O que o review te dá 2. Empurrar o checkpoint pra direita 3. Quando remover o humano
  4. Quem revisa o agente 5. Vídeo walkthrough + TTS 6. Review mais rápido com IA

### T5 — Soluções Prontas pra Copiar (teal 📋)
- **5-1** 🧹 O reset de 2 passos — *"Volte ao zero"*
  1. Por que resetar 2. Deletar tudo 3. Observar o agente puro
  4. Recamadar com procedures 5. Trazer de volta só o que falta 6. Customizar pra experimentar
- **5-2** 🔍 grill-me + 10 decisões — *"Alinhe antes de codar"*
  1. A skill grill-me (texto) 2. O prompt das 10 decisões 3. "Me entreviste até 98%"
  4. Quando usar 5. Adaptar ao seu projeto 6. Erros comuns
- **5-3** 🔗 Pipeline grill-me → PRD → issues — *"Do brain ao backlog"*
  1. Visão geral 2. grill-me 3. two-PRD 4. to-issues 5. Encadeamento 6. Onde fica o humano
- **5-4** 🛰️ Setup AFK completo — *"Como o Matt roda"*
  1. Claude Code + Opus 4.8 medium 2. AFK via sandbox 3. Sand Castle setup
  4. Paralelizar com segurança 5. Puxar commits de volta 6. Seu setup mínimo
- **5-5** 🤖 Action de review + cron de security — *"Automação que se cuida"*
  1. Esqueleto da Action 2. checkout → type check → review 3. Comentar no PR
  4. Cron diário rotativo 5. Estruturar dados do explore 6. Auto-merge com cautela
- **5-6** 🎥 Review fluido + onde achar — *"Feche o ciclo"*
  1. Vídeo walkthrough + TTS 2. Otimizar review humano 3. mattpocock/skills
  4. aihero.dev/skills 5. npx skills latest add 6. Os 2 primeiros passos hoje

## STATUS DO BUILD — ✅ COMPLETO (verificado no browser)
- [x] Fundação (dirs + assets learn.css/js + plano + brief + transcrição)
- [x] 6 heros inemaimg (landing + 5 trilhas)
- [x] Landing index.html
- [x] 5 índices de trilha (T1..T5) — todos com 36 acordeões, hero img+SVG, mapa
- [x] 30 módulos (6 por trilha) — 6 tópicos, marcar-lido, dúvida, SVG, check
- [x] Verificação headless: 36 páginas, 0 erros de console, cores corretas
- [x] Link integrity: 489 refs locais, 0 quebrados
