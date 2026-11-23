# Lesson vocabulary lists

One file per lesson, transcribed from the "Vocabulary / المفردات" pages of the
scanned course books:

- `SLL1058F-lesson-{1..6}-vocab.json` from *INITIAL_ARABIC_TEXTBOOK_PART_1.pdf*
- `SLL1059S-lesson-{7..16}-vocab.json` from *INITIAL_ARABIC_TEXTBOOK_PART_2.pdf*

```json
{
  "course": "SLL1059S",
  "lesson": 8,
  "source": { "file": "INITIAL_ARABIC_TEXTBOOK_PART_2.pdf", "pdf_pages": [28, 29] },
  "words": [
    {
      "arabic": "نَقَلَ",
      "english": "to transmit, to transport",
      "tag": "verb",
      "verb_form": 1,
      "present_vowel": "u",
      "governs": "إِلَى",
      "image": "images/transmit.svg",
      "arabic_book": "نَقَلَ (إِلَى) (ـُ)",
      "english_book": "transmit/transport (to)"
    }
  ]
}
```

`arabic` and `english` are kept clean so they can be used directly as quiz
answers: `arabic` is the bare, fully vowelled headword (Unicode NFC), and
`english` is a comma-separated list of acceptable glosses with no bracketed
remarks. Everything else the book prints is moved to the other keys.

| field | meaning |
|---|---|
| `arabic` | headword, fully vowelled, spelling checked against standard forms |
| `english` | clean gloss(es), comma-separated alternatives |
| `tag` | word class: `noun`, `verb`, `adjective`, `adverb`, `proper noun`, `pronoun`, `demonstrative`, `interrogative`, `preposition`, `prefix` (attached particles such as بِ، لِ، فَ، سَ), `particle`, `conjunction`, `interjection`, `phrase` |
| `gender` | `m` / `f` where the book distinguishes it, or for people and nouns of fixed gender |
| `verb_form` | derived verb form 1–10 (the book's bracketed number; 1 for basic triliteral verbs). Omitted for the quadrilateral تَرْجَمَ |
| `present_vowel` | stem vowel of the present tense (`u`, `a`, `i`), given in the book as a bracketed vowel sign |
| `present_tense` | present tense form, where the book gives it in full (e.g. جَاءَ → يَجِيءُ) |
| `governs` | preposition or particle the word is used with (e.g. سَافَرَ + إِلَى) |
| `definite` | definite form, for words like اِمْرَأَةٌ → اَلْمَرْأَةُ |
| `feminine` | feminine form given alongside the headword |
| `plural` | plural from the book's brackets (`(-ات)` expanded); alternatives separated by `،` |
| `variants` | alternative spellings of the headword |
| `diptote` | entry is marked `*` (diptote) in the book; in Part 2 this usually refers to the plural |
| `note` | usage or grammar information removed from the gloss |
| `image` | icon for the word, relative to this folder |
| `arabic_book` | the Arabic exactly as printed, when it differs from `arabic` |
| `english_book` | the English gloss exactly as printed |
| `spelling_note` | why `arabic` differs from the printed spelling |
| `handwritten` | the entry was added by hand on the scan rather than printed |
| `source_note` | remarks about the scan itself (handwritten glosses, abbreviated plurals) |

Entries are listed in the book's reading order (right-hand column first, then left).
`pdf_pages` are 1-based page numbers within the PDF, not the printed page numbers.

## Images

`images/*.svg` are 64×64 icons in the same flat style as the flashcards in
`index.html`. Icons for words already in `index.html` are copied from there.
The rest are built from [Lucide](https://lucide.dev) icons (ISC licence, see
`images/LICENSE-lucide.txt`): a pastel circle with the line icon drawn on top. The colour
follows the word class (verbs teal, nouns blue, adjectives purple, proper
nouns coral, function words green, and so on). Grammatical words with no
sensible picture use a text glyph instead. A word that appears in more than
one lesson shares one image file.
