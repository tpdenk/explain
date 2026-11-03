---
name: explain
description: >
  Write explanations in ASD-STE100 Simplified Technical English. Use when the
  user asks to explain something, asks how or why something works, asks what
  something is or does, or wants to understand code, a system, a concept, an
  error, or a result.
---

# Explain

Write each explanation in ASD-STE100 Simplified Technical English (STE). An explanation tells the user what something is, how it works, or why it occurs.

## Scope

These rules apply to all prose in the explanation: paragraphs, list items, table cells, and captions. They also apply to the text after a list label, for example the text after "Cause:".

These rules do not apply to some text:

- Code, identifiers, paths, commands, and configuration keys do not follow the rules.
- Text that you quote verbatim does not follow the rules, for example errors, logs, documents, and user text.
- Headings, column headers, and list labels do not follow the rules.

## Words

- Use simple, common words. Use "use", not "utilize". Use "start", not "initiate".
- Use one word for one thing. Do not use synonyms for the same thing in one explanation.
- Use one meaning for one word. For example, use "right" only for the direction, not for "correct".
- You can use technical names (for example "mutex", "HTTP header", "garbage collector") and technical verbs (for example "compile", "hash", "parse"). If a technical name is not common, tell the reader what it means.
- Use the approved STE word if you know it. For example, write "occur", not "happen". Write "make sure", not "ensure". Write "through", not "via". Write "immediately after", not "just after".
- If you are not sure that a word is approved, replace it with a more basic word. Do not send the word and report your doubt.
- Do not use idioms, slang, metaphors, or humor.
- Do not use phrasal verbs. Write "start", not "set up". Write "find", not "figure out".
- Do not use contractions. Write "do not", not "don't".
- Do not use noun clusters of more than three words. Use prepositions to break them: write "the timeout of the request handler", not "the request handler timeout value".

## Sentences

- Write a maximum of 20 words in a procedural sentence.
- Write a maximum of 25 words in a descriptive sentence.
- Write one idea in each sentence.
- Write full sentences. Do not write fragments. Do not omit articles ("the", "a") or verbs. A phrase at the end of a sentence can also be a fragment, for example "The cache stores the result, with a timeout where possible."
- Do not write elliptical constructions. Write all the words that the reader must otherwise add. Write "A parent process can start many child processes. A child process has only one parent process", not "A parent process can start many child processes, but not the reverse". Other elliptical phrases are "where possible", "if any", "as needed", and "if so".
- Do not omit "that" before a clause. Write "The log shows that the build failed", not "The log shows the build failed". Write "the file that you edit", not "the file you edit".
- Use the active voice. Write "The parser reads the file", not "The file is read by the parser".
- Look for the passive voice in short conditions and relative clauses too. Write "If the flag is true", not "If the flag is set". Write "The client sends the failed requests again", not "The failed requests are sent again". An adjective after "is" is not passive, for example "The disk is full".
- Use the imperative for instructions. Write one instruction in each sentence.
- Put a condition before the instruction: "If the build fails, examine the log."
- Make each pronoun ("it", "this", "they") refer clearly to one noun. If the reference is not clear, repeat the noun.
- Do not use "-ing" forms as verbs or nouns. Write "When you start the server", not "When starting the server". You can use technical names that end in "-ing".

## Verb tense

Use the simple present tense by default. Use it for general facts, for system behavior, and for what the code does.

You can use the simple past tense only when the present tense makes the statement factually wrong. This occurs for actions and events that are complete:

- Correct: "I ran the tests to verify the fix." The run is complete.
- Correct: "The deploy failed at 14:02 because the disk was full." The failure occurred at a specific time.
- Incorrect: "The function returned a list." The function always returns a list. Write "The function returns a list."

Do not use other tenses (for example the present perfect or progressive tenses). Write "I changed the file", not "I have changed the file".

## Paragraphs and structure

- Write one topic in each paragraph.
- Write a maximum of six sentences in a paragraph.
- Start with the most important information: the answer first, then the details.
- Use a vertical list for a sequence of steps or for three or more parallel items.
- Write a warning or a caution before the related instruction, not after it.

## Tables

- Each table cell contains one item or one or more full sentences. An item is a name, an identifier, a type, a number, or "yes" or "no".
- Do not write a descriptive phrase in a cell. "Parser in the build step" is a fragment. Write "The parser in the build step makes this file." You can also change the column so that it contains only a name, for example "parser".

## Check

Before you send the explanation, do these steps. If a sentence fails a step, write the sentence again. Do not send an explanation with a violation that you know about.

1. Count the words in each long sentence. Count a code identifier as one word. If a sentence has more than 20 or 25 words, split it.
2. Find each form of "be" ("is", "are", "was", "were", "be", "been") that comes before a past participle. Change each passive clause to the active voice.
3. Find each fragment, each elliptical phrase, and each omitted "that". Look in list items and table cells too.
4. Find each "-ing" form, each phrasal verb, and each word that is not approved.
5. Find each verb in the past tense. If the present tense is correct, change the verb to the present tense.
