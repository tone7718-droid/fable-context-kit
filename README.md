# Fable Context Kit

**Slash token costs and eliminate context bloat when using Claude Fable 5.**

This kit gives you prompts, skills, and workflows — *designed to be powered by Fable 5 itself* — that directly solve the #1 pain point reported across X and Reddit right now:

> "I typed 'hey' into an old Fable 5 session and it cost me $20. 847,000 input tokens because the full history + tools + system prompt were resent."

Fable 5 is the most capable model for ambitious, long-running work. But at $10 per million input / $50 per million output tokens, every unnecessary token hurts — especially after the included usage window ends on July 7.

## The Core Problem (widely shared on X)
- Claude Code / sessions resend the **entire accumulated context** on every single message.
- Prompt cache expires after short idle periods (e.g. 5 minutes) → full price reprocessing.
- Result: one small message in a long project can cost as much as a full task.
- People burn through weekly limits in minutes when using high effort or treating Fable as a daily driver.
- Silent fallbacks and aggressive limits make the pain worse.

Popular posts with hundreds of likes and 100k+ views are full of horror stories and "how I cut costs 70-80%" advice.

## The Solution This Kit Provides
Turn Fable 5 (the model that understands 1M context best) into your **Context Engineer**.

It will:
- Intelligently compact bloated history while preserving 100% of the value.
- Extract structured, reusable memory (decisions, state, facts).
- Generate tiny "carry-forward" prompts so you can start fresh sessions cheaply.
- Recommend effort levels, task routing (Fable = architect, cheaper models = executor), and when to reset.
- Self-verify its own compaction so nothing important is lost.

Use the expensive model once to create efficiency that saves money on every future turn — and even on cheaper models after July 7.

## Quick Start — Use Immediately with Fable 5

1. Go to claude.ai or Claude Code and select **Fable 5**.
2. Start a **new chat** (best) or use the session you want to clean.
3. Open `CONTEXT_OPTIMIZER_SKILL.md` from this repo and copy its full content.
4. Paste the skill, then add:
   ```
   Compact and optimize the following session history using the rules above.
   [paste your full current conversation or the last major chunk here]
   ```
5. Let Fable 5 run. It will output:
   - Clean session summary
   - Ready-to-save memory files (`PROJECT_CONTEXT.md`, `DECISIONS.md`, `NEXT_STEPS.md`, etc.)
   - A lean carry-forward prompt (aim < 1-2k tokens)
   - Cost analysis + recommendations

6. **Start a fresh session**, load the memory files + carry-forward prompt, and continue. You will immediately see much lower token usage.

Repeat periodically or when context feels heavy.

**Pro tip:** Do this *before* July 7 while Fable 5 is still included in your plan. The artifacts it creates will keep working on Opus, Sonnet, or other models.

## Files in This Kit

- `CONTEXT_OPTIMIZER_SKILL.md` — The main weapon. A complete, self-contained prompt/skill you load into Fable 5.
- `templates/` — Example structured memory files you can copy and fill (or let Fable generate).
- This README + usage guidance.

## Why This Works So Well with Fable 5
- 1M context window + exceptional long-horizon understanding.
- Built for self-verification (it can check its own compaction quality).
- Superior at planning, decomposition, and turning messy work into clean artifacts.
- Community consensus: Use Fable for the hard thinking and distillation; run the results on cheaper models.

Many high-engagement posts already recommend "make Fable write skills for the future" and "Fable as architect only". This kit systematizes and supercharges that advice.

## Extra Tips from the Community (integrated into the skill)
- Drop effort level unless the task truly needs it (low/medium Fable often beats max Opus).
- Never let Fable both plan *and* execute everything.
- Keep one persistent memory file that accumulates learnings.
- Start fresh sessions more often than you think.
- Use advisor mode or explicit routing.

## Contributing & Improving the Kit
The best improvements will come from using Fable 5 *with this kit*.

1. Load the optimizer skill.
2. Ask it to review and upgrade the skill itself or the templates.
3. Open a PR with the improved version.

Issues and real usage stories (especially before/after token counts) are very welcome.

## Links & Credits
- Inspired by dozens of viral X posts about Fable 5 costs (the "$20 hey", limit burning, fallback complaints, Ponytail skill, architect patterns, etc.).
- Built to be used with Anthropic's Claude Fable 5 (claude-fable-5).

---

Use Fable 5 to solve the problems Fable 5 creates for its users. That's the meta move.

Start compacting. Your wallet (and weekly limits) will thank you.