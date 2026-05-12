# Neurosovet (Нейросовет)

### Multi-Model AI Arbitration Methodology

**Author:** Andrew Meingardt (Андрей Майнгардт)
**Published:** May 12, 2026 · Moscow
**Affiliation:** [NEUROMEIN](https://t.me/neuromein) × [WMT AI](https://wmt-ai.ru)

---

🇷🇺 **[Читать на русском](README_RU.md)**

---

## What is Neurosovet?

Neurosovet is a structured methodology for conducting multi-model AI debates with iterative arbitration. Instead of simply comparing answers from different AI models, it implements a rigorous protocol with:

- **Iterative rounds** (2–4) where models critique and refine each other's positions
- **Anti-sycophancy protocol** (8 rules) preventing models from blindly agreeing with the arbiter
- **Delta-analysis** classifying each model's response to criticism into 4 types: Integration, Sycophancy, Stable Position, and Reasoned Disagreement
- **Arbiter self-correction** — the arbiter is required to reconsider when models push back with strong arguments
- **Cultural-methodological filter** accounting for differences between Western, Chinese, and Russian AI models
- **Convergence signals** indicating when to stop or continue rounds
- **Mandatory web search** for the arbiter model on factual and time-sensitive questions
- **Factual contradiction verification** — explicit protocol for handling conflicting facts between models

## How It Works

1. You ask the same question to 3–5 AI models, each running the **participant prompt**
2. You read all responses (this is critical — you are the orchestrator, not a courier)
3. An **arbiter model** analyzes responses using a strict protocol: task classification → individual evaluation → comparison matrix → blind spot detection → cultural analysis → final synthesis
4. The verdict goes back to participant models — they must justify any position changes with specific citations
5. The arbiter performs **delta-analysis**: who genuinely improved, who just agreed without substance, who held their ground, who pushed back with arguments
6. Repeat for 2–4 rounds. In practice, 2–3 rounds capture 80–90% of the value

## What Makes This Different

| Feature | Neurosovet | Perplexity Council | AI Council Framework | Microsoft Council | MoA (Together) |
|---|---|---|---|---|---|
| Iterative rounds | 2–4 | 1 | Up to 3 | 1 | Many layers |
| Anti-sycophancy protocol | 8 rules | No | Basic | No | No |
| Delta-analysis | 4 types | No | No | No | No |
| Arbiter self-correction | Yes | No | No | No | No |
| Cultural analysis | Yes | No | No | No | No |
| Human orchestrator | Required | No | Yes | No | No |
| Convergence signals | 3 levels | No | No | No | No |
| Different AI models | Any | 3 fixed | Any | 2 fixed | Any |
| Automation | Manual | Full | Full | Full | Full |

## Repository Structure

```
neurosovet/
├── README.md                    # This file (English)
├── README_RU.md                 # Russian version
├── LICENSE                      # CC BY-NC-SA 4.0
├── guide/
│   └── neurosovet-guide.pdf     # Full methodology guide (Russian)
├── prompts/
│   ├── ru/
│   │   ├── 01_arbiter.md        # Arbiter prompt (Russian, original)
│   │   └── 02_participant.md    # Participant prompt (Russian, original)
│   └── en/
│       ├── 01_arbiter.md        # Arbiter prompt (English)
│       └── 02_participant.md    # Participant prompt (English)
└── CHANGELOG.md                 # Version history
```

## Quick Start

### 1. Set Up the Arbiter

Choose the strongest available model (check [LMSYS Leaderboard](https://arena.ai) for current rankings). The arbiter must have web search enabled.

- **Claude** (recommended as of May 2026): Create a Project in Claude, paste the arbiter prompt into Custom Instructions
- **Gemini**: Create a Gem with the arbiter prompt
- **ChatGPT**: Create a Custom GPT or paste into each chat

### 2. Set Up Participants

Open a new chat in each AI model (3–5 recommended). Paste the participant prompt + your question into each chat.

**Recommended models:** ChatGPT, Claude, Gemini, Grok, DeepSeek, Qwen. For Russian-specific questions, add GigaChat or YandexGPT.

### 3. Run the Council

1. Collect all responses
2. Read every response fully
3. Copy all responses to the arbiter chat
4. Get the verdict
5. Send the verdict back to each participant
6. Collect updated responses → send to arbiter
7. Repeat for 2–3 rounds

## Use Cases

- **Strategic decisions** — market entry, build vs buy, competitive response
- **Forecasting and risk assessment** — market evolution, regulatory impact, technology trends
- **Complex analysis with incomplete information** — why a superior product loses to an inferior one
- **Public speaking preparation** — stress-testing arguments, anticipating counterarguments
- **Investment and hiring decisions** — acqui-hire evaluation, infrastructure choices
- **Research questions** — resolving contradictory studies, evaluating AI Safety approaches

## Not For

- Simple factual questions (one model is enough)
- Tasks with a single correct answer
- Urgent questions (no time for 3 rounds)
- Routine tasks (writing, translation, editing)
- Purely subjective tasks (taste can't be arbitrated)

## Time Investment

3 rounds × 4–5 models = 12–15 copy operations. For a complex question: 30–60 minutes. This is a deliberate choice — the method is optimized for quality, not speed.

## Version

Current: **v1.0** (May 2026)

## Citation

If you use this methodology in research or publications:

```
Meingardt, A. (2026). Neurosovet: A Methodology for Multi-Model AI
Arbitration. NEUROMEIN × WMT AI. https://github.com/neuromein/neurosovet
```

## License

This work is licensed under [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/).

You are free to share and adapt this material for non-commercial purposes, as long as you give appropriate credit and distribute your contributions under the same license.

For commercial licensing inquiries: ameinhardt@wmtgroup.ru

## Author

**Andrew Meingardt** (Андрей Майнгардт)
AI Strategist · NEUROMEIN × WMT AI

- Telegram: [@Andrew_meinhardt](https://t.me/Andrew_meinhardt)
- Email: ameinhardt@wmtgroup.ru
- Blog: [NEUROMEIN](https://t.me/neuromein)
- Company: [wmt-ai.ru](https://wmt-ai.ru)
