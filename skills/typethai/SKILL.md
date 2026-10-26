---
name: typethai
description: Write or translate text into natural Thai that reads like a Thai person wrote it, not like machine translation. Use when writing Thai, translating English to Thai (UI copy, slides, PR descriptions, review replies, taglines), or reviewing Thai text that "feels off".
---

# Type Thai

Your default Thai is stiff and translated: you think in English shapes and swap in Thai words. Write what a Thai person would actually say.

## Core rules

1. **Translate meaning, not words.** Never map one English word to one Thai word. If a line still feels wrong after fixing words, change the structure: describe the consequence or the situation instead of translating the English noun phrase.
2. **Don't trust your own sense of "natural".** You invent slang-looking phrases (เทสฟ้อง, ทับกลับ) and then rate them as natural. Never invent colloquialisms. When unsure, use plain standard wording; slightly formal Thai is less of a giveaway than made-up slang.

## 1. Before writing

Identify the medium (title, slide, PR, chat), audience, tone, any wordplay, and any glossary. Then pick a mode:

- **Plain mode** (default): PRs, review replies, commits, tickets, docs, chat, and anything generic. Write like a Thai colleague talking: plain words, no selling.
- **Copy mode**: presentation headlines, launch slides, product pages, taglines. Crafted language is expected here, so the bar is "would this fit a Thai product page or keynote slide", not "would someone say this out loud". Set phrases (ขอแนะนำ X, มาทำความรู้จักกับ X), short punchy fragments, rhythm and rhyme, and elevated words are fine. Formality is a choice; keep it consistent within the piece.
- **Mixed** (e.g. an internal deck): headline and tagline in copy mode, body text in plain mode.

Copy mode loosens tone, not accuracy: still translate meaning, still no invented slang, still no literal metaphors. Marketing words (ปฏิวัติ, เหนือชั้น) don't belong in plain mode.

**Code-mixing.** Decide the policy now; apply it everywhere. Default for Thai tech/product teams:

- **English**: product/tool names, UI labels, output types, common dev nouns.
- **Thai**: words teams already say in Thai (มาตรฐาน, เครื่องมือ, ขั้นตอน, ระบบ).
- Story characters in Thai, products named after them in English.
- If unsure what the team says, pick one and flag it.

**Register.** Match the medium. Don't mix formal and casual within one part (a headline, a body, a message). Particles (ครับ/ค่ะ/นะ) only where a speaker would use them; ค่ะ (statement) ≠ คะ (question). คุณ is fine when addressing a customer in copy; it sounds stiff in team chat.

## 2. Write

- Write each line from its meaning, in Thai structure.
- Spend the effort on wording. Readers stop trusting text when the *words* sound machine-made; symbols, exact numbers and test names are fine.
- Thai separates clauses with spaces: replace `;` with ส่วน (switch subject) or แล้ว (and then).
- Carry allusions into the title Thai readers know (… and the Chamber of Secrets → …กับห้องแห่งความลับ). Keep a metaphor's mapped word identical in both places.

## 3. Check

Check every line against this list. For bad → better examples (same section names), read `references/examples.md` when reviewing Thai or when a line still feels off.

- **Wrong sense**: a verb that doesn't fit its subject (a file can't พา; run ≠ วิ่ง), or meaning drift (becomes ≠ คือ).
- **English verbs/adjectives in Thai verb slots** (…govern แล้ว). English nouns are fine (sync, label, PR). Don't put English into fixed Thai collocations (วางมาตรฐาน, not วาง standard).
- **Literal metaphors**: floor, ceiling, path, line, pointer, chain, compose, belongs, named → say the plain meaning.
- **English structure**: noun-phrase UI chips (describe what goes wrong instead), stacked negatives, mirrored "no longer" (name the old state: จากเดิมที่… ตอนนี้…), English clause order that shifts the subject, over-compression.
- **Missing Thai words** (แอปที่ทีม**ใช้**ทำงาน, **มา**รู้จัก).
- **Broken mechanics**: doubled words (เป็นทั้ง…และเป็นทั้ง), run-ons that parse wrong, stray spaces left by stripped formatting (Thai spaces are clause breaks).
- **Translationese markers**: extra pronouns, การ/ความ nominalizations, passive ถูก, ทำการ/ดำเนินการ, essay connectors (นอกจากนี้, อย่างไรก็ตาม), assistant voice (แน่นอน!, หวังว่าจะเป็นประโยชน์), em dashes everywhere.
- **Over-explaining**: justifying actions the reader already understands; dense parentheticals.
- **Inconsistency**: code-mixing that drifts from the policy; parallel items that aren't parallel; a mode that drifts (selling words in a PR, chat tone in a headline).
- **Phrases you can't vouch for**: replace with plainer wording.

## 4. Hand over

- Offer alternatives as candidates for the user to pick. Some choices are preference, not errors.
- Don't call any Thai natural, yours or anyone's. Point out concrete problems; leave the verdict to the native speaker.
- Flag real ambiguities in the source with an alternative, instead of silently guessing.
- Don't overclaim. Say only what was checked ("same size" is not "identical every byte").
