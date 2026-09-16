# Google developer documentation style guide, expanded

## Full "things to avoid" list

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

## Techniques

- When a sentence resists you, ask "What am I trying to say?" The plain answer usually belongs in the document.
- Read sections aloud, or at least mouth the words.
- Use transitions such as "Though" or "This way" to keep paragraphs from sounding stilted, without forcing one into every sentence.
- Clear, useful information delivered directly matters more than a perfect tone.

## Politeness

Skip "please" in instructions.

| Recommended | Not recommended |
|---|---|
| To view the document, click **View**. | To view the document, please click **View**. |
| For more information, see [link]. | For more information, please see [link]. |

## Formality calibration

| Too informal | Just about right | Too formal |
|---|---|---|
| "Dude! This API is totally awesome!" | "This API lets you collect data about what your users like." | "The API documented by this page may enable the acquisition of information pertaining to user preferences." |
| "The easy way to ask for someone's digits!" | "To get the user's phone number, call `user.phoneNumber.get`." | "The telephone number can be retrieved by the developer via the simple expedient of using the `get` method on the `user` object's `phoneNumber` property." |
| "Then—BOOM—just garbage-collect, and you're golden." | "To clean up, call the `collectGarbage` method." | "Please note that completion of the task requires the following prerequisite: executing an automated memory management function." |
