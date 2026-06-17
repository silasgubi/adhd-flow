# 🧠 TDAH Daily

Sistema diário de produtividade pessoal pensado para pessoas com TDAH, integrado ao ecossistema Google e ao Claude (IA da Anthropic).

**Demo:** [Acesse aqui](https://SEU-USUARIO.github.io/tdah-daily/) *(substitua pelo seu link após publicar)*

---

## ✨ O que é

Um PWA (Progressive Web App) que funciona como o "documento de leitura matinal" de quem precisa lembrar diariamente das estratégias TDAH para não cair em armadilhas comuns: perfeccionismo, multitarefa, scrolling, autocrítica.

Substitui anexos no Microsoft To Do, papéis colados na parede, ou notas perdidas no celular.

---

## 🎯 Por que existe

Pessoas com TDAH têm déficit de dopamina — o que torna difícil **manter** motivação, mesmo quando há vontade. A solução não é "força de vontade", é **design de sistema**:

- Quick wins primeiro → dopamina → momentum
- Energia gerencia ordem das tarefas, não urgência
- 1 coisa por vez, sempre
- Feito > Perfeito
- Sistema externo > memória interna

Este app codifica essas estratégias num formato que dá pra abrir todo dia, em 1 toque, do iPhone.

---

## 📱 Features

| Feature | O que faz |
|---------|-----------|
| **Mantra rotativo** | Frase diferente a cada abertura (20 frases curadas) |
| **Checklist matinal** | 8 itens com persistência local, reset automático meia-noite |
| **Pomodoro 45/10** | Timer de foco + pausa com alerta sonoro |
| **Hierarquia de vida** | Saúde → Família → Trabalho → Admin → Hobbies sempre visível |
| **Sistema completo** | Fluxo Keep → Tasks → Calendar com atalhos Chrome do Claude |
| **Manual TDAH** | Estratégias, armadilhas e rotinas diária/semanal |
| **Mantras (lista)** | 20 frases para momentos de fraqueza |
| **Botão Travado** | Modal com protocolo de 3 passos para destravar |
| **PWA offline** | Funciona sem internet após primeiro acesso |

---

## 🏗️ Arquitetura do sistema completo

Este app é uma das peças. O sistema completo:

```
📱 Google Keep         → captura de ideias instantâneas (mobile)
✅ Google Tasks        → organização única de tarefas
🌐 Claude in Chrome    → planejamento diário automatizado
📅 Google Calendar     → blocos de foco do dia
🧠 TDAH Daily (este)   → leitura matinal + ferramentas de foco
```

O Claude (com skill `tdah-productivity-manager`) lê o Google Tasks no Chrome, prioriza usando matriz de Eisenhower + nível de energia, e cria blocos de foco no Google Calendar.

A skill completa do Claude está no repositório [tdah-productivity-manager](#) *(privado)*.

---

## 🚀 Como usar

### Online (recomendado)

1. Abra [https://SEU-USUARIO.github.io/tdah-daily/](https://SEU-USUARIO.github.io/tdah-daily/) no Safari (iPhone) ou Chrome
2. Toque em **Compartilhar → Adicionar à Tela Inicial**
3. Ícone aparece como app — toque para abrir em fullscreen

### Local

```bash
git clone https://github.com/SEU-USUARIO/tdah-daily.git
cd tdah-daily
# Abrir index.html em qualquer navegador
# Ou servir local: python -m http.server 8000
```

---

## 🎨 Design

- **Mobile-first** — pensado para iPhone primeiro
- **Dark mode** — único modo (TDAH-friendly: menos estímulo visual)
- **Tipografia:** Inter (legibilidade) + JetBrains Mono (código)
- **Cores:** paleta restrita, função define cor (verde = ação, vermelho = atenção, roxo = mantra)
- **Sem dependências externas** — só CDN do Google Fonts (cacheia offline)

---

## 🔧 Tecnologia

- HTML/CSS/JS puro — sem build, sem framework
- Service Worker para offline
- localStorage para checklist diária
- Web Audio API para alerta do Pomodoro
- Web Clipboard API para copiar prompts

Tudo em **~1 arquivo HTML**. Total: ~20KB.

---

## 📋 Personalização

Para adaptar ao seu contexto, edite no `index.html`:

| Variável | O que muda |
|----------|-----------|
| `MANTRAS = [...]` | Frases que rotacionam |
| `CHECKLIST = [...]` | Itens da rotina matinal |
| `timerSeconds = 45*60` | Duração do Pomodoro |
| Aba "Sistema" | Suas ferramentas e fluxo |
| Aba "Manual" | Suas estratégias TDAH |

---

## 🤝 Inspiração e princípios

Construído sobre conceitos de:

- **GTD (Getting Things Done)** — David Allen
- **Pomodoro Technique** — Francesco Cirillo
- **Matriz de Eisenhower** — priorização Urgente × Importante
- **MVP (Minimum Viable Product)** — Eric Ries
- Pesquisa em TDAH e dopamina (Russell Barkley)

---

## 📄 Licença

MIT — use, modifique, compartilhe. Se ajudar alguém, missão cumprida.

---

## 🙏 Para quem está chegando aqui com TDAH

Você não é preguiçoso. Não falta força de vontade. Seu cérebro funciona diferente, e isso significa que o sistema precisa ser diferente também.

Comece pequeno. **Começar mal > não começar.**
