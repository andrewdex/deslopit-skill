---
name: deslopit
description: Clean AI slop from HUMAN WRITING (posts, emails, copy, replies). Use when text reads machine-generated and you want it to sound like a person wrote it.
---

# DeSlop — write like a human, not an LLM

## When to use
Before you send any text that could pass as machine-written: posts, emails, product copy, docs, replies, landing pages, bios. If a line reads like it came from a language model, it is not finished yet.

## Why this matters
Readers can smell AI slop instantly. Clear, blunt, human writing cuts through. This skill turns LLM-flavored prose into something a person would actually say.

## What to strip (mechanical, safe)
1. Filler phrases: "in today's rapidly evolving digital landscape", "it is crucial to", "it is important to note", "at the end of the day", "when it comes to", "in conclusion", "ultimately".
2. Corporate/AI buzzwords: leverage, harness the power of, cutting-edge, seamless / seamlessly, unprecedented, game-changing, best-in-class, innovative, robust, empower, foster, drive, unlock, elevate, revolutionize, think outside the box, synergy.
3. Empty transitions: "furthermore", "moreover", "in addition", "as an AI language model".
4. Repetition: if the writer said the same idea in three ways, keep one.
5. **Em dashes ( — )** : replace with comma, period, or restructure. No exceptions.
6. AI tells: perfect parallelism (not X not Y just Z), neat little epigrams that close too cleanly, triads ("this, that, and the other"), unsupported bold claims.

## The safety rule (never break meaning)
This pass is MECHANICAL. It removes filler and tells; it does NOT rewrite the meaning, tone, or argument. Rules:
- Keep every fact, number, negations (not, never), modal strength (must/should/can), and possessive constructs.
- Do not "improve" the writer's actual point. If a rewrite would change what was said, leave it alone and flag it instead.
- Never fabricate statistics, quotes, citations, or evidence to fill a gap. If it is not verifiable, cut it or mark it unverified.

## Procedure
1. Paste the text through the cuts above (or run it in de-slop tooling: local model / the de-slop API).
2. Read the result out loud as a person.
3. Pinch test: does it read like a human texting a friend, or like a LinkedIn post? Human = done. LinkedIn/bot = cut more.

## Verification
- No em dashes remain.
- No filler or buzzword survived.
- No fact or meaning was changed.
- It reads like a person wrote it.
