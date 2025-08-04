# Enhanced Lapis Fork

**This is a fork of the [Lapis Anki template](https://github.com/donkuri/lapis) with additional features:**

**New Features Added:**
- **Settings Panel** - Adjustable transparency and font selection for terms and readings
- **Dictionary Image Gallery** - Automatic extraction and display of images from dictionary entries with navigation
- **Enhanced Visual Design** - Glass morphism effects for containers and dictionary-themed colored borders
- **Improved Dictionary Styling** - Better visual distinction between different dictionary sources

All original Lapis functionality is preserved, except for the top container displaying frequency information, which I removed.


<div>
  <img src="assets/Lapis.gif" alt="Click cards with Lapis">
</div>

## How to use Lapis

To use Lapis, first download the example deck from [Releases](https://github.com/kiwakiwaa/lapis-extended/releases). From there, you need to change your fields settings in Yomitan. Start by selecting `Lapis` as the `Model` in Yomitan's `Configure Anki Card Format`. Here is how your fields should be set up:

| Field                 | Value                                                                                                                                                      |
|-----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Expression            | `{expression}`                                                                                                                                             |
| ExpressionFurigana    | `{furigana-plain}`                                                                                                                                         |
| ExpressionReading     | `{reading}`                                                                                                                                                |
| ExpressionAudio       | `{audio}`                                                                                                                                                  |
| SelectionText         | `{popup-selection-text}`                                                                                                                                   |
| MainDefinition        | Something like `{single-glossary-jmdict/jitendex}`. Find this by clicking the down arrow next to this field, and finding a dictionary in a similar format. |
| DefinitionPicture     | Here you can include any image you'd like to use to help *illustrate* the definition or the vocabulary term.                                               |
| Sentence              | `{cloze-prefix}<b>{cloze-body}</b>{cloze-suffix}`                                                                                                          |
| SentenceFurigana      |                                                                                                                                                            |
| SentenceAudio         |                                                                                                                                                            |
| Picture               |                                                                                                                                                            |
| Glossary              | `{glossary}`                                                                                                                                               |
| Hint                  |                                                                                                                                                            |
| IsWordAndSentenceCard |                                                                                                                                                            |
| IsClickCard           |                                                                                                                                                            |
| IsSentenceCard        |                                                                                                                                                            |
| IsAudioCard           |                                                                                                                                                            |
| PitchPosition         | `{pitch-accent-positions}`                                                                                                                                 |
| PitchCategories       | `{pitch-accent-categories}`                                                                                                                                |
| Frequency             | `{frequencies}`                                                                                                                                            |
| FreqSort              | `{frequency-harmonic-rank}`                                                                                                                                |
| MiscInfo              | `{document-title}` If you want your cards to include the title of the tab they were mined from, such as for light novels (LNs), please use this feature.   |