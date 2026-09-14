---
name: technical-writing
description: Writes and edits prose for documentation, slide decks, PDFs, README files, commit messages, UI copy, and other technical or scientific text. Applies Orwell's six rules, Google's developer documentation style guidance adapted for scientific communication, and Gopen and Swan's reader-expectation principles. Use when drafting or revising any user-facing or technical text, including docs, slides, PDFs, papers, error messages, button labels, tooltips, and headings.
license: MIT
---

# Technical writing

Clear writing is clear thinking. Apply this skill to any prose you write or edit: documentation, slide copy, PDF content, README files, papers, UI copy, commit messages, and comments.

## Three foundational resources

Consult them in this order. Each governs a different level of the text.

1. **Orwell's six rules**, from "Politics and the English Language" — word and phrase choices.
2. **Google's developer documentation style guide** (https://developers.google.com/style), adapted for scientific communication — voice, conventions, and formatting.
3. **Gopen and Swan's "The Science of Scientific Writing"** (https://www.cs.tufts.edu/comp/105-2015s/readings/sci.html) — sentence and paragraph structure, and where readers expect to find information.

All three sources disclaim their own authority. Orwell's sixth rule permits breaking the other five. Google calls its guide "guidelines, not rules." Gopen and Swan write that "any reader expectation can be violated to good effect." When the sources conflict, choose what the reader will understand.

## 1. Orwell's six rules

Apply these to every sentence, and let rule 6 override the rest:

1. Never use a metaphor, simile, or other figure of speech which you are used to seeing in print.
2. Never use a long word where a short one will do.
3. If it is possible to cut a word out, always cut it out.
4. Never use the passive where you can use the active.
5. Never use a foreign phrase, a scientific word, or a jargon word if you can think of an everyday English equivalent.
6. Break any of these rules sooner than say anything outright barbarous.

## 2. Google style guidance, adapted for scientific communication

**Voice and tone**
- Conversational, friendly, and respectful. Sound like a knowledgeable colleague, not a formal manual.
- Second person ("you"), not "we."
- Active voice by default, so the reader can see who performs the action.
- Write for a global audience. Avoid idioms, cultural references, and needlessly complex vocabulary.
- Put conditions before instructions: "To export the data, click **Export**."

**Avoid**
- Buzzwords and figurative language.
- Filler: "please note," "at this time," "simply," "easily," "just."
- Exclamation marks, cutesiness, and internet slang.
- "Please" in instructions.
- Choppy or long-winded sentences, and repeating the same sentence opener.

**Formatting**
- Sentence case for titles and headings.
- Numbered lists for sequences, bulleted lists otherwise.
- Serial commas.
- Code in code font; UI elements in bold.
- Unambiguous dates: "January 3, 2026," not "1/3/26."
- Descriptive link text, never "click here."

**Adapting for scientific and technical audiences**

Orwell's rule 5 and Google's warning about jargon target imprecise jargon, not precise terminology. Keep the exact technical term when it carries meaning the everyday word loses, and define it on first use. As Gopen and Swan put it, aim for clarification, not simplification: never trade away accuracy, nuance, or complexity to make a sentence shorter. Cut the words that obscure the science, not the science itself.

See [reference.md](reference.md) for expanded guidance from all three sources, including the tone examples and the full reader-expectation principles.

## 3. Reader expectations (Gopen and Swan)

Readers extract meaning from structure, not from words alone. They expect specific information in specific places, and every violation costs them effort they could have spent on the content. These principles matter most for dense or complex material.

- **Keep the subject next to its verb.** Readers wait for the verb before they can interpret anything; whatever intrudes reads as an interruption of lesser importance. Move long qualifiers out of the gap, or into their own clause.
- **Open with the topic position.** The first words tell the reader whose story the sentence is and how it connects backward. Put old, already-introduced information there.
- **Close with the stress position.** Readers naturally emphasize whatever arrives at the point of syntactic closure, so put the new information you want emphasized at the end. A colon or semicolon creates an extra stress position.
- **Put the action in the verb.** When the real action hides in a noun ("performed an analysis of"), readers are left to guess at it. Write "analyzed."
- **Give each unit one function.** A clause, sentence, section, or document should make a single point.
- **Provide context before new material.** Familiarize, then inform.
- **Match structural emphasis to substantive emphasis.** What matters most should land where readers expect emphasis.

**Sentence length**: no word count decides this. A sentence is too long when it holds more emphasis-worthy material than it has stress positions to hold it.

**Passive voice**: Orwell's rule 4 and Google both prefer the active, and that remains the default. But Gopen and Swan show the limit: "Bees disperse pollen" and "Pollen is dispersed by bees" are both good sentences, and the passive is the better one inside a paragraph telling pollen's story. Keep the passive when it puts the right topic first, and prefer the active everywhere else.

**Logical gaps**: applying these principles exposes missing connections between ideas, because the writer knew them and never wrote them down. Rearranging structure will not fix a gap. Supply the missing reasoning, or cut the material whose connection you cannot state.

## Editing workflow

Copy this checklist and work through it after drafting, or when revising existing text:

```
- [ ] Read it aloud, and rewrite whatever sounds awkward
- [ ] Reunite separated subjects and verbs
- [ ] Check each sentence's first words: is the linking, old information there?
- [ ] Check each sentence's last words: is the new, emphasized information there?
- [ ] Move buried actions into verbs
- [ ] Cut every word that carries no weight (rule 3)
- [ ] Swap long, Latinate, or jargon words for everyday ones, keeping precise terms (rules 2 and 5)
- [ ] Remove clichés and stock figures of speech (rule 1)
- [ ] Prefer the active, unless the passive keeps the right topic in front (rule 4)
- [ ] Check second person, sentence-case headings, serial commas, and descriptive links
- [ ] Name the connections the structure exposed as missing
- [ ] Reread: break any rule above rather than write something barbarous or unclear
```

## Format-specific notes

**Documentation and README files**: lead each section and paragraph with its most important sentence. Make headings a skimmable outline. Prefer short paragraphs and lists over dense prose.

**Slide decks**: slide text is a headline, not a paragraph, so cut hard (rule 3). One idea per bullet, parallel phrasing within a list, and the emphasized term at the end of the line where the eye stops. Put detail and nuance in the speaker notes.

**PDFs and papers**: the prose rules for documentation apply, and structure carries more weight because readers skim. Keep each section to its declared function, so methods stay out of results. Check that headings, alt text, and reading order stay logical for accessibility tools.

**UI copy**: labels, errors, empty states, and tooltips are the most compressed form of this style, so rules 2 and 3 dominate. State what happened, then what to do next, in the active voice: "Upload failed. Check your connection and try again," not "An error was encountered during the upload process."

## When guidance conflicts

Follow the three sources in order, then prioritize the reader's comprehension over any rule here, per Orwell's rule 6. For questions none of them answer, use Merriam-Webster for spelling, the Chicago Manual of Style for nontechnical style, and the Microsoft Writing Style Guide for technical style. Once you depart from this guidance, stay consistent within the document.
