Fiendly Words
=================

You can use this product to generate default names for projects, groups, objects eg. Think `sinister-brainslug`, `slothful-coven`, `depraved-busywork`, or even `default-default`.  It's inspired by, and forked from, the original _friendly_ words lists by Glitch. Obviously, and in the spirit of this project, I obliterated them all. Too friendly, nice, feelgood, easy-listening for my rubbish lair.

Usage
---

```
const fiendlyWords = require('fiendly-words');

fiendlyWords.predicates;
> ["evil","slimey","sinister","unctuous","tedious","slothful",...

fiendlyWords.objects;
> ["eye-of-newt","pain","conspiracy","lair","shark","laser",...

fiendlyWords.teams;
> ["coven","gang","band","cult","plot",

fiendlyWords.collections;
> ["mess","nightmarefuel","rubbish","boxful",...
```


The Words
---------

The words are pulled from curated files. We want the words and their pairings to be fiendish, evil, humorous, absurd, forgettable, etc.  They should also be words that most people can't easily remember and spell.

All of the words and their generated pairings should be safe for entertainment. We still don't permit word pairings that invoke to hate speech, hostility, derogatory terms, etc. We like our evil with a healthy dose of humour and humanity.

Despite our best efforts, it's easy for a pair of fiendish words to be combined into something inappropriate. Whenever we notice a generated pair that is problematic, we'll remove at least one of the words from that pair so that it won't reoccur. We'll err on the side of trusting reports and removing potentially inappropriate words rather than defending the appropriate uses of a word.

When adding words to the list, an abundance of empathy is required. If it could be offensive or disparaging, nope.

The Word Files
--------------

Our word lists are highly-opinionated lists of *predicates* and *direct objects*.  This structure allows us to put together word pairs that are more likely to make grammatical sense, and therefore tend to be easier to say, type, and remember.

`words/objects.txt`

> The direct object receives the action of the sentence. The direct object is usually a noun or pronoun.

`words/predicates.txt`

> The predicate expresses action or being within the sentence. The simple predicate contains the verb and can also contain modifying words, phrases, or clauses.

`words/teams.txt`

> This is a list of synonyms for "team".  They're a special subset of objects.

`words/collections.txt`

> This is a list of synonyms for "collection".

For our purposes, the predicates are mostly verbs and adjectives.

It's OK for a word to be duplicated between the objects and predicates lists so long as that word is valid in both contexts,  e.g. "buffalo-buffalo" or "lavender-lavender".

Within a given file, the words should be alphabetized, distinct, and contain only lower-case alphabetic ASCII characters.  These constraints are checked at build time.

