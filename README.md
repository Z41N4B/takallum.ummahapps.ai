# Takallum تَكَلُّم

A free speaking-practice app for Modern Standard Arabic (fusha). Live at https://takallum.ummahapps.ai/

**Content:** 85 swap-in sections (462 sentences): conversation phrases (greetings, Islamic phrases, phrases to a man, a woman and a group, about yourself), everyday phrases, 60 discussion words moved from Kalimat Plus with their own button and 4 sentences each, and grammar builders; 14 transform chains and 13 role-play conversations, all with full harakat.

## Features
- Swap-in drills: read the English, say the Arabic out loud, reveal and mark yourself. Missed sentences come back sooner.
- Transform chains: one sentence changes step by step (person, gender, tense, negation).
- Role-play: everyday conversations with a model reply for each turn.
- Hear without seeing the words: an option in drills, chains and role-play that hides the Arabic until you tap Show words.
- Short grammar tips under most drill answers and role-play replies, shown once you reveal them.
- Plain-English grammar explanations for lam, kana and its sisters, inna and its sisters, mundhu, yajibu, alladhi, the idafa, comparatives, conditionals and numbers
- Normal and slow audio (uses the device's Arabic text-to-speech voice)
- Vowel marks can be switched off
- Practise as a man or a woman: items, chain steps and role-play turns can carry an `f` override with the feminine wording
- Previous button during drills and chains to look back at earlier sentences
- Review only the sentences already marked solid
- I already know this: tick single sentences, whole sections or a whole group, or skip one during a lesson. Lessons skip them and they count as solid; `progress.known` keeps the level from before so unticking restores it, and missing one in review puts it back into lessons
- Up to 3 learners on one device, each with their own progress and their own man or woman choice, shared with Takallum Kids, Kalimat and Kalimat Plus. Learner p1 keeps the original `qul-progress` key. Hidden when progress saves to an account.
- Progress: each sentence has a level from 0 to 5; Got it on the first try in a session adds one, Missed it resets to 0; level 2 counts as solid. Bars count a practised sentence as a quarter, a sentence at level 1 as a half and a solid one in full, so one lesson always moves them

## Shared with the other apps
Takallum Kids, Kalimat, Kalimat Plus and Takallum share two things on the same device through `ummah.js`, which is copied into each app's folder (keep the four copies identical):
- **Learners:** name, boy or girl (man or woman), and animal, in the `ua_l` cookie on `.ummahapps.ai`. A learner added in one app appears in the others; a learner still called "Learner 1" stays in its own app until renamed.
- **Known words:** words learned in Takallum Kids and Known well words in Kalimat and Kalimat Plus go into a per-learner `ua_w_<id>` cookie as short hashes of the bare Arabic. Kalimat and Kalimat Plus offer to add words known from the other apps.

Each page also ends with the same four-app family strip. On localhost, `ummah.js` points the strip's links at the local servers (Kids 8771, Kalimat 8766, Kalimat Plus 8772, Takallum 8770).

## SEO and GEO
`index.html` has meta tags, Open Graph and JSON-LD (WebApplication + LearningResource + FAQPage), plus a visible About and FAQ section. `robots.txt`, `sitemap.xml` and `llms.txt` sit at the root.

## Running locally
```
node serve.js
```
Then open http://localhost:8765
