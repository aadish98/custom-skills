# Expanded reference

Detailed guidance from the three sources behind this skill. Read the section you need.

- [Orwell's six rules](#orwells-six-rules-in-context)
- [Google developer documentation style guide](#google-developer-documentation-style-guide)
- [Gopen and Swan on reader expectations](#gopen-and-swan-on-reader-expectations)

## Orwell's six rules, in context

Source: George Orwell, "Politics and the English Language" (1946).

Orwell's target was writing that conceals meaning, whether by habit or by intent. His rules describe symptoms of that concealment: dead metaphors used because they save the writer from thinking, long words that inflate simple claims, passives that hide who acted, and jargon that signals membership instead of conveying content.

He ranks the rules himself. The sixth rule exists because mechanical obedience to the first five produces its own kind of bad prose, so a rule yields whenever following it would make a sentence worse.

Google's guide cites that sixth rule directly as its governing philosophy:

> "Break any of these rules sooner than say anything outright barbarous." — George Orwell, "Politics and the English Language"
>
> "This guide contains guidelines, not rules. Depart from it when doing so improves your content... When you depart from this guide, be consistent throughout your document."

## Google developer documentation style guide

Full guide: https://developers.google.com/style. Fetch specific pages, such as the word list or grammar sections, for questions this file does not cover.

### Tone and content

- Be conversational and friendly without being frivolous.
- Don't pre-announce upcoming content or features.
- Use descriptive link text, not "click here" or "this page."
- Write accessibly and for a global audience. Simple, consistent writing also translates better.

### Language and grammar

- Second person ("you") rather than "we."
- Active voice, making clear who performs the action.
- Standard American spelling and punctuation.
- Conditions before instructions: "If X, do Y," not "Do Y if X."

### Formatting, punctuation, organization

- Sentence case for document titles and section headings, not Title Case.
- Numbered lists for sequences; bulleted lists for most other lists.
- Description lists for pairs of related data.
- Serial (Oxford) commas.
- Code-related text in code font (`like this`).
- UI elements in bold (**Save**, **Cancel**).
- Unambiguous date formatting: "January 3, 2026," never "1/3/26" or "3/1/26."

### Images

- Provide alt text for every image.
- Provide high-resolution or vector images when practical.

### Things to avoid

- Buzzwords or technical jargon.
- Being too cutesy.
- Figurative language, including metaphors and ableist language.
- Placeholder phrases such as "please note" and "at this time."
- Choppy or long-winded sentences.
- Starting every sentence with the same phrase ("You can...", "To do...").
- Current pop-culture references.
- Exclamation marks.
- Wackiness, zaniness, and goofiness.
- Phrasing that denigrates or insults any group.
- "Let's do something" phrasing.
- "Simply," "it's that simple," "it's easy," or "quickly" in a procedure. These judge the reader's difficulty, and they insult anyone who finds the step hard.
- Internet slang and abbreviations such as tl;dr or ymmv.

### Techniques

- When a sentence resists you, ask "What am I trying to say?" The plain answer usually belongs in the document.
- Read sections aloud, or at least mouth the words.
- Use transitions such as "Though" or "This way" to keep paragraphs from sounding stilted, without forcing one into every sentence.
- Clear, useful information delivered directly matters more than a perfect tone.

### Politeness

Skip "please" in instructions.

| Recommended | Not recommended |
|---|---|
| To view the document, click **View**. | To view the document, please click **View**. |
| For more information, see [link]. | For more information, please see [link]. |

### Formality calibration

| Too informal | Just about right | Too formal |
|---|---|---|
| "Dude! This API is totally awesome!" | "This API lets you collect data about what your users like." | "The API documented by this page may enable the acquisition of information pertaining to user preferences." |
| "The easy way to ask for someone's digits!" | "To get the user's phone number, call `user.phoneNumber.get`." | "The telephone number can be retrieved by the developer via the simple expedient of using the `get` method on the `user` object's `phoneNumber` property." |
| "Then—BOOM—just garbage-collect, and you're golden." | "To clean up, call the `collectGarbage` method." | "Please note that completion of the task requires the following prerequisite: executing an automated memory management function." |

### Reference hierarchy

1. Project-specific style guidance, if the repository or product has any.
2. Google's developer documentation style guide.
3. Third-party references by question type: Merriam-Webster for spelling, The Chicago Manual of Style (17th ed.) for nontechnical style, and the Microsoft Writing Style Guide for technical style.

## Gopen and Swan on reader expectations

Source: George D. Gopen and Judith A. Swan, "The Science of Scientific Writing," *American Scientist* 78 (1990). Full text: https://www.cs.tufts.edu/comp/105-2015s/readings/sci.html

Their premise: "If the reader is to grasp what the writer means, the writer must understand what the reader needs." Difficult science does not require difficult prose. Readers interpret structure, and when structure misleads them, they spend their effort decoding sentences instead of evaluating the work.

Their aim is clarification, not simplification. In their own revisions they neither reduced the jargon nor diluted the science.

### The seven principles

1. Follow a grammatical subject as soon as possible with its verb.
2. Place in the stress position the new information you want the reader to emphasize.
3. Place the person or thing whose story a sentence tells at the beginning, in the topic position.
4. Place appropriate old information in the topic position, for linkage backward and context forward.
5. Articulate the action of every clause or sentence in its verb.
6. Provide context for your reader before asking that reader to consider anything new.
7. Ensure that the relative emphases of the substance coincide with the relative expectations for emphasis raised by the structure.

### Topic position

The opening words establish the perspective: readers expect a unit of discourse to be a story about whoever shows up first. The topic position also supplies linkage backward and context forward, which is why old information belongs there.

Stated precisely, since every sentence mixes old and new material throughout: "Put in the topic position the old information that links backward; put in the stress position the new information you want the reader to emphasize."

Gopen and Swan call misplaced old and new information "the No. 1 problem in American professional writing today." The cause is mechanical: writers rush to record a new thought before it escapes, then add the connecting context afterward, serving their own need to unload information rather than the reader's need to receive it.

### Stress position

Readers emphasize what arrives last, at the moment of syntactic closure. Put stress-worthy material there, or readers will either emphasize the wrong thing or find nothing worth emphasizing. Colons and semicolons create additional stress positions, which is how a long sentence can stay readable.

On length: "A sentence is too long when it has more viable candidates for stress positions than there are stress positions available."

### Subject-verb separation

Readers need syntactic resolution and cannot interpret a subject until the verb arrives. Material inserted between them reads as an interruption of secondary importance, no matter how significant it actually is. Either promote that material into its own clause or cut it.

### Action in the verb

Readers expect the action of a sentence in its verb. When verbs reduce to "is," "are," or "has," the real action hides in nouns, and readers must guess at it. Naming the action in the verb often reveals that the writer never decided what the action was.

### Passive voice

Structure, not voice, decides the case: "Bees disperse pollen" and "Pollen is dispersed by bees" are both respectable sentences about the same facts. The first is about bees, the second about pollen, and the passive is superior inside a paragraph continuing pollen's story.

### Logical gaps

Applying these principles surfaces missing connections, because writers omit links that feel obvious to them. Revision then requires supplying the connection or deleting material whose relevance cannot be stated. As Gopen and Swan found, fixing structure sends the writer back into the substance: "In real and important ways, the structure of the prose becomes the structure of the scientific argument. Improving either one will improve the other."

### Rules versus principles

None of these are rules. "Our best stylists turn out to be our most skillful violators; but in order to carry this off, they must fulfill expectations most of the time, causing the violations to be perceived as exceptional moments, worthy of note."
