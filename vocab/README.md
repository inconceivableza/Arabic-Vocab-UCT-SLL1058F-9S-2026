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
    { "arabic": "رَئِيسٌ", "plural": "رُؤَسَاءُ", "english": "president", "diptote": true }
  ]
}
```

Word fields:

| field | meaning |
|---|---|
| `arabic` | headword as printed, fully vowelled (Unicode NFC). Bracketed prepositions/notes are kept, e.g. `سَافَرَ (إِلَى)`. A bracketed lone vowel giving the present-tense stem vowel is written on a tatweel, e.g. `كَتَبَ (ـُ)`. |
| `plural` | plural given in brackets in the book (`(-ات)` is expanded to the full form) |
| `english` | gloss as printed; numbers like `(4)` are the verb form |
| `diptote` | the entry is marked `*` (diptote) in the book; in Part 2 this usually refers to the plural |
| `handwritten` | the entry was added by hand on the scan rather than printed |
| `note` | anything else, e.g. handwritten extra glosses |

Entries are listed in the book's reading order (right-hand column first, then left).
`pdf_pages` are 1-based page numbers within the PDF, not the printed page numbers.
