# Les phrases

French grammar (Grammaire 7P): types and forms of sentences. Self-contained —
`index.html` plus an icon, no build step.

## Sections

| Section | What it does |
|---|---|
| La théorie | Reference cards: the 4 types, the 2 forms, and the négatif → positif table |
| Quel type de phrase ? | 56 sentences; tap déclarative / interrogative / impérative / exclamative |
| Le verbe est-il à l'impératif ? | 20 sentences; oui or non — separates "Monte !" from "Tu peux monter" |
| Positive ou négative ? | 20 sentences; tap the form |
| Transformer | 18 written answers: to the negative, to the imperative, to the exclamative, to the declarative, and questions to fit a given answer |

Every section uses the same pile: a right answer removes the sentence, a wrong one
sends it back a few places on, so the round only ends when everything has been
answered correctly. A wrong tap shows the rule that applies, not just the answer.

## About the written section

Free-text French can't be marked perfectly. Accents, capitals, punctuation and
apostrophe style are ignored, and each item carries a list of acceptable answers —
but a valid sentence that isn't on the list will be marked wrong. That's why there's
a **« C'était juste aussi »** button: it overrides the marking and clears the sentence.
If a particular answer keeps coming up, add it to that item's `r` list.

## Adding or changing content

All the content is in named arrays at the top of the `<script>` block:

- `PHRASES` — `["sentence", "D" | "IN" | "IM" | "E"]`
- `IMPERATIF` — `["sentence", "oui" | "non"]`
- `FORMES` — `["sentence", "P" | "N"]`
- `TRANSFORME` — `{c: instruction, q: sentence, r: [accepted answers]}`

Adding a line to any of them is enough; nothing else needs changing. Interface wording
sits in the same block, in `TYPES` and in the `EXOS` menu list.

## Publishing

The `francais` folder sits in the repository root:

    https://flc-lab-projects.github.io/Revision/francais/

Open in Safari, then Share → Add to Home Screen.
