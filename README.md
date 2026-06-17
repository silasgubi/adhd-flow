# 🧠 ADHD Flow

**EN:** An ADHD-friendly daily productivity PWA integrating Google Keep, Tasks, Calendar and Claude AI.

**PT:** Um PWA de produtividade diária para TDAH, integrando Google Keep, Tasks, Calendar e o Claude.

**Demo:** [https://silasgubi.github.io/adhd-flow/](https://SEU-USUARIO.github.io/adhd-flow/)

---

## 🇧🇷 Português

### O que é

Sistema de leitura matinal e foco diário pensado para pessoas com TDAH. Substitui qualquer anotação perdida no celular, anexo esquecido no gerenciador de tarefas, ou documento que nunca é aberto.

Funciona como um **app instalado na tela inicial do iPhone** — 1 toque, abre fullscreen, sem distrações.

### Por que existe

Pessoas com TDAH não têm falta de vontade — têm déficit de dopamina. O cérebro precisa de **sistema externo**, não de força de vontade interna. Este app codifica as estratégias no lugar da memória.

### Features

| Feature | O que faz |
|---------|-----------|
| **Mantra rotativo** | 1 frase diferente a cada abertura (20 frases) |
| **Checklist matinal** | Reset automático à meia-noite |
| **Pomodoro 45/10min** | Timer com alerta sonoro |
| **Hierarquia de vida** | Saúde → Família → Trabalho → Admin → Hobbies |
| **Fluxo do sistema** | Keep → Tasks → Claude → Calendar |
| **Atalhos Claude** | Prompts prontos para copiar no Chrome |
| **Botão Travado** | Protocolo de 3 passos para destravar |
| **Offline** | Funciona sem internet após primeiro acesso |

### Como instalar no iPhone

1. Abra a URL no **Safari**
2. Toque em **Compartilhar → Adicionar à Tela de Início**
3. Pronto — ícone na home, abre como app

### Arquitetura do sistema completo

```
📱 Google Keep      → captura de ideias instantâneas
✅ Google Tasks     → sistema único de tarefas
🌐 Claude Chrome    → planejamento via /planeja-dia
📅 Google Calendar  → blocos de foco confirmados
🧠 ADHD Flow       → leitura matinal + foco
```

### Personalização

Edite no `index.html`:
- `MANTRAS = [...]` — suas frases
- `CHECKLIST = [...]` — sua rotina matinal
- Aba "Manual" — suas estratégias
- Aba "Sistema" — seu fluxo de ferramentas

---

## 🇺🇸 English

### What is it

A morning reading and daily focus system designed for people with ADHD. Works as an **installed PWA on your iPhone home screen** — 1 tap, opens fullscreen.

Replaces forgotten sticky notes, missed task manager attachments, and documents that never get opened.

### Why it exists

People with ADHD don't lack willpower — they have a dopamine deficit. The brain needs an **external system**, not more internal effort. This app puts strategies where memory fails.

### Features

| Feature | What it does |
|---------|-------------|
| **Rotating mantra** | 1 different phrase per session (20 curated) |
| **Morning checklist** | Auto-reset at midnight |
| **Pomodoro 45/10min** | Focus timer with audio alert |
| **Life hierarchy** | Health → Family → Work → Admin → Hobbies |
| **System flow** | Keep → Tasks → Claude → Calendar |
| **Claude shortcuts** | Ready-to-copy Chrome extension prompts |
| **Stuck button** | 3-step unblocking protocol |
| **Offline** | Works without internet after first load |

### Install on iPhone

1. Open the URL in **Safari**
2. Tap **Share → Add to Home Screen**
3. Done — icon on home, opens as an app

### Full system architecture

```
📱 Google Keep      → quick idea capture
✅ Google Tasks     → single task system
🌐 Claude Chrome    → daily planning via /plan-day
📅 Google Calendar  → confirmed focus blocks
🧠 ADHD Flow       → morning reading + focus tools
```

### Customize

Edit in `index.html`:
- `MANTRAS = [...]` — your phrases
- `CHECKLIST = [...]` — your morning routine
- "Manual" tab — your ADHD strategies
- "System" tab — your tool flow

---

## 🛠️ Stack

- Vanilla HTML/CSS/JS — no build, no framework
- Service Worker (offline)
- localStorage (daily checklist persistence)
- Web Audio API (Pomodoro alert)
- Web Clipboard API (copy prompts)

Total: **~1 HTML file, ~33KB**

---

## 📄 License / Licença

MIT — use, modify, share freely.
Se ajudar alguém, missão cumprida. / If it helps someone, mission accomplished.

---

## 💜 Para quem chega aqui com TDAH / For those arriving here with ADHD

**PT:** Você não é preguiçoso. Não é falta de força de vontade. Seu cérebro funciona diferente — e isso significa que o sistema precisa ser diferente também. Começar mal > não começar.

**EN:** You're not lazy. It's not a lack of willpower. Your brain works differently — which means the system needs to be different too. Starting badly > not starting.
