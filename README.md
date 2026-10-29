# Takallum تَكَلُّم

A free speaking-practice app for Modern Standard Arabic (fusha). Live at https://takallum.ummahapps.ai/

**Content:** 19 sentence patterns (150 sentences), 8 transform chains and 6 role-play conversations, all with full harakat.

## Features
- Swap-in drills: read the English, say the Arabic out loud, reveal and mark yourself. Missed sentences come back sooner.
- Transform chains: one sentence changes step by step (person, gender, tense, negation).
- Role-play: everyday conversations with a model reply for each turn, and an optional listen-first mode.
- Short grammar tips under most drill answers and role-play replies, shown once you reveal them.
- Plain-English grammar explanations for lam, kana and its sisters, inna and its sisters, mundhu, yajibu, alladhi, the idafa, comparatives, conditionals and numbers
- Normal and slow audio (uses the device's Arabic text-to-speech voice)
- Vowel marks can be switched off
- Practise as a man or a woman: items, chain steps and role-play turns can carry an `f` override with the feminine wording
- Previous button during drills and chains to look back at earlier sentences
- Review only the sentences already marked solid
- Progress: each sentence has a level from 0 to 5; Got it on the first try in a session adds one, Missed it resets to 0; level 2 counts as solid

## SEO and GEO
`index.html` has meta tags, Open Graph and JSON-LD (WebApplication + LearningResource + FAQPage), plus a visible About and FAQ section. `robots.txt`, `sitemap.xml` and `llms.txt` sit at the root.

## Running locally
```
node serve.js
```
Then open http://localhost:8765
