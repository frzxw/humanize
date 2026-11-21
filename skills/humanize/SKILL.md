---
name: humanize
description: >-
  Remove signs of AI-generated writing so prose reads human. Use this
  skill before sending or publishing any substantial prose: chat replies,
  documents, reports, PR descriptions, posts, and emails. Use it when
  editing or reviewing a draft, when writing for a reader who already
  knows the subject, and when writing in Indonesian, where translation-ese
  and empty formal phrases are the most common tells. Covers 40 patterns
  across staging, rhythm, inflation, formatting, chat leftovers,
  wrong-reader failures, Indonesian failures, and agent failures.
---

# Humanize

A model picks whatever phrasing fits the widest range of readers and
subjects. A person writes for one reader and one subject, so their
choices are uneven and specific. Every pattern in this skill is a form
of that default choice.

Two working rules govern everything below:

- Every sentence kept must add something the reader did not already have.
- Patterns 1 to 5 justify an edit on one sighting. Patterns marked _weak
  alone_ only count when other tells appear in the same passage.

## Modes

Detect mode: name each pattern found, quote the line, give the fix in a
few words. Do not rewrite, and do not guess whether AI wrote the text.

Edit mode: apply the minimum effective edit. Fix patterns, errors,
repetition, and unclear passages. Leave strong human sentences alone,
and preserve the writer's voice: vocabulary, cadence, bluntness, humor,
uncertainty, digressions. Never invent a fact, name, number, date, or
quote to fill a gap. If something is unclear, ask, or write a simpler
sentence.

## A. Staging instead of stating

1. **Binary contrast.** "Not just X, it's Y", also split across
   sentences or as a clipped tail. The negative half names something
   nobody claimed, so the positive half sounds bigger. State the point
   directly. Keep a contrast only when the negative half corrects a
   belief the reader actually holds, or both halves carry information.
2. **One-line closers and fake-profound kickers.** A lone sentence that
   restates the paragraph ("That is the real win."), a sentence after an
   example that names what it showed ("This shows that..."), a recap
   ending, or a closing line that turns the point into a metaphor. Cut
   it unless it adds a fact the text does not already show. End on the
   last concrete fact or the next action.
3. **Deep-sounding sayings.** "The real question is", "at its core",
   "what really matters", "X is the language of Y". Replace the saying
   with the specific claim.
4. **Staged run-up.** "Let's dive in", "Here's the thing", "Here's what
   you need to know". Announcing the point instead of making it. Remove
   the run-up.
5. **Arguing with no one.** "To be clear", "Don't get me wrong", "I'm
   not saying...", rejecting an option nobody raised. Remove the
   defense; state the claim it hides.
6. **Faux-insight setups.** "What nobody tells you", "The part everyone
   misses", "What most people get wrong". Cut the setup; the claim
   stands on its own.
7. **Colon reveals.** A noun phrase, a colon, then a lowercase dramatic
   reveal: "The best part: it learns." Rewrite as a plain sentence.
   Colons are for lists, labels, and quotes.
8. **Rhetorical setups.** "What if I told you...", "Think about it:",
   self-answered "Question? Answer." pairs. Drop them.
9. **Interpretive metadiscourse.** "The key point is", "As you can
   see", "That last part matters more than it sounds", "In other
   words". Delete the aside, or replace it with support for the claim.

## B. Rhythm by rule

10. **Forced triads.** Ideas arriving in threes to sound complete.
    Check each item adds a distinct idea; merge or develop the
    strongest.
11. **Repeated sentence openings.** Consecutive sentences starting with
    the same subject. Merge, change the subject, or start with the
    action.
12. **Em dashes as the universal connector.** Em dashes everywhere
    because the writer skipped choosing how clauses relate. Replace
    with a period, comma, colon, or parentheses. One or two in a long
    draft are fine when they clearly beat the alternatives. Some
    contexts ban them outright; merge messages are a common one.
13. **Stacked qualifiers.** "Could potentially possibly be argued that
    it might." Keep a qualifier only when the source supports it. _Weak
    alone._
14. **Hyphenated pairs everywhere.** Compounds keeping the hyphen after
    the noun ("the report is high-quality"). Drop it there; keep it
    before the noun. _Weak alone._
15. **Passive voice and missing subjects.** "No configuration file
    needed." Name who acts when it clarifies. Never let inanimate
    things do human verbs. _Weak alone._
16. **Synonym cycling.** Rotating agent, assistant, and tool for style.
    If the clear word is right, repeat it.
17. **Negative listing.** "Not a X. Not a Y. A Z." Just say Z.
18. **Robotic rhythm.** Repeated sentence shapes, identical paragraph
    structures, stacked punchy fragments. Vary sentence length the way
    a person does: unevenly, following the content.

## C. Inflation and borrowed authority

19. **Overused AI words.** Delve, tapestry, landscape (abstract),
    underscore and highlight (as verbs), crucial, pivotal, robust
    (figurative), showcase, vibrant, meticulous, enduring, testament,
    interplay, intricate, garner, bolstered, additionally. The banned
    list under "Words and phrases to cut" is longer.
20. **Inflated significance.** "Marking a pivotal moment", "stands as a
    testament", "setting the stage for", "plays a vital role", stock
    "Challenges and Future Outlook" sections, bright-future send-offs.
    Keep the fact, drop the significance.
21. **Vague connection.** "Associated with", "linked to", "tied to"
    without saying how. Name the relationship the source gives.
22. **Shallow -ing riders.** "..., highlighting, reflecting,
    symbolizing, fostering..." bolted onto a plain fact to make it
    sound deeper. Keep the fact; keep the rider only when the source
    supports it.
23. **Sales language.** Nestled, breathtaking, stunning, renowned,
    groundbreaking (figurative), "in the heart of", "commitment to".
    State what the thing is.
24. **Weasel attribution.** "Experts argue", "studies show", "many
    argue", "widely regarded as", prestige-outlet lists, follower
    counts standing in for a claim. Use the named source and what it
    said, or cut the claim.
25. **Avoiding is, are, has.** "Serves as", "stands as", "boasts",
    "features". Prefer is, are, and has when they are clearer. Make
    verbs do the work: "made a decision" becomes "decided", "has the
    ability to" becomes "can".

## D. Formatting by rule

26. **Bold as decoration.** Bolded words with no reason; vertical lists
    where every item has a bold label and a colon. Remove the bold.
    Turn labeled lists into prose when the labels carry no information.
    Bold is earned by helping the reader find or compare something.
27. **Decorative headings.** Title case everywhere, emojis or arrows in
    headings, a rule between every section, a heading that performs
    ("The decision, on one screen") instead of naming its contents ("How
    the six options compare"). Sentence case, no decoration.
28. **Over-structuring.** Tables, bullet lists, and headers where two
    sentences of prose read better; a header over a two-sentence
    section. Structure is for material the reader must scan or compare,
    not a default shape for every answer.
29. **Curly quotation marks** where the target format uses straight
    quotes. _Weak alone._

## E. Chat and draft leftovers

30. **Chatbot residue.** "Great question!", "I hope this helps!", "Of
    course!", "Let me know if...", "Would you like me to...?". Remove
    the wrapper, keep the content.
31. **Knowledge-limit disclaimers and guesses.** "As of my last
    update", "while details are limited...", "likely grew up..." (a gap
    filled with a plausible guess). State what the source does not
    show, or cut the sentence.
32. **A heading repeated in the first sentence.** The one-line paragraph
    under a heading that restates it. Cut it.
33. **Writing about the document instead of its subject.** Narrating how
    the text was assembled, what it replaced, or a legend the reader can
    already see. Keep a source credit the reader can follow; cut the
    account of how you worked.

## F. Wrong reader, wrong size

34. **Re-explaining what the reader knows.** A reply that restates the
    problem, walks the diagnosis, and lays out evidence before reaching
    the decision. In a thread the reader already has the context. Lead
    with the decision; keep only the reasoning that could change
    whether they agree, usually one fact they lack and any link they
    need.
35. **Length mismatch.** An essay answering a yes-or-no question, or a
    one-liner answering a decision that needs evidence. Match the
    length to what the reader must do with the answer.
36. **Sycophancy and empty agreement.** Praising the question or the
    idea before answering it ("Great idea!", "Ide bagus!"). Answer
    first. Agreement means something only when it could have been
    disagreement.

## G. Indonesian failures

37. **Translation-ese.** English sentence structure pasted into
    Indonesian: "Ini adalah sebuah..." opening every paragraph, "di
    mana" as the relative pronoun for everything, "melakukan" plus a
    noun where a plain verb exists ("melakukan pembayaran" for
    "membayar"), passive di- chains that hide who acts across a whole
    paragraph. Indonesian puts the actor first and trusts short
    sentences. Write the sentence an Indonesian speaker would say.
38. **Empty Indonesian phrases.** "Penting untuk dicatat bahwa", "perlu
    diketahui bahwa", "tidak dapat dipungkiri bahwa", "pada akhirnya",
    "di era digital saat ini", "dalam rangka untuk". Cut the phrase and
    keep the fact after it.

## H. Agent failures

39. **Announcing instead of doing.** A deliverable or reply that
    narrates planned steps ("Selanjutnya saya akan memeriksa...") where
    the result belongs. Do the step, then report the result. A plan is
    the content only when the reader asked for a plan.
40. **Invented specifics.** A plausible number, name, date, or quote
    filling a gap the source left open. The reader acts on specifics,
    so an invented one costs more than an admitted gap. Write what the
    source shows, and mark the gap as a gap.

## Words and phrases to cut

Banned outright: delve, foster, leverage, utilize, facilitate, empower,
streamline, robust, cutting-edge, paradigm shift, game changer,
tapestry, realm, beacon, multifaceted, meticulous, intricate,
paramount, transformative, elevate, embark, supercharge, harness,
ever-evolving.

Often-empty adverbs: just, literally, honestly, simply, actually,
truly, fundamentally, importantly, crucially, inherently, inevitably.
Cut when they add nothing.

Often-empty phrases: it's worth noting, it's important to note, at the
end of the day, when it comes to, at its core, in today's world, in the
age of, the reality is, the truth is, in terms of, with regard to, in
order to, going forward, let's dive in.

## The portability test

If a sentence could move unchanged to another person, company, or
product, it is filler. Cut it or replace it with a fact specific to
this subject. This test catches the sentences the pattern list misses.

## When not to act

A person can make any of these choices on purpose. Leave a watched
phrase inside a quotation, a title, a proper name, or a passage that
discusses the phrase. Keep details that carry the writer's voice:
specific unusual details, mixed feelings, era-bound references,
explainable first-person choices, genuine asides and self-corrections.
Keep "I think" or "maybe" when they express real uncertainty or the
writer's spoken rhythm.

## Process

1. Mark the tells, strongest first. Look at paragraph shape too, not
   only sentences.
2. Draft the rewrite. Keep every supported claim.
3. Check the draft: read it aloud, ask what still sounds AI-generated,
   verify no fact was added or lost. Patterns 1, 2, 10, 12, and 26
   survive first drafts most often.
4. Write the final version. Vary sentence length.

## Applying it in chat and repositories

In chat, the patterns that do the most damage are 26, 27, and 34:
dense replies where the point drowns. Lead with the conclusion in the
first sentence, keep one topic per message, and avoid stacked bold
headers and walls of lists. Long material goes in a document; the chat
carries the core and the link.

In repositories: PR titles use Conventional Commits; PR descriptions
stay neutral, with no internal labels or design references; commit and
merge messages contain no em dash; code comments are in English and
explain only the why that the code does not show.
