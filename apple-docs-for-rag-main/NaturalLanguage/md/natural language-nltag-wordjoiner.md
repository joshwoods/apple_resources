

- Natural Language
- NLTag
-  wordJoiner 

Type Property

# wordJoiner

A tag indicating that the token is a word joiner, signifying that two tokens on each side should not be broken up.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
static let wordJoiner: NLTag
```

## Discussion

Word joiners are typically used in languages that do not use explicit spaces.

## See Also

### Lexical classes

static let noun: NLTag

A tag indicating that the token is a noun.

static let verb: NLTag

A tag indicating that the token is a verb.

static let adjective: NLTag

A tag indicating that the token is an adjective

static let adverb: NLTag

A tag indicating that the token is an adverb.

static let pronoun: NLTag

A tag indicating that the token is a pronoun.

static let determiner: NLTag

A tag indicating that the token is a determiner.

static let particle: NLTag

A tag indicating that the token is a particle.

static let preposition: NLTag

A tag indicating that the token is a preposition.

static let number: NLTag

A tag indicating that the token is a number.

static let conjunction: NLTag

A tag indicating that the token is a conjunction.

static let interjection: NLTag

A tag indicating that the token is an interjection.

static let classifier: NLTag

A tag indicating that the token is a classifier.

static let idiom: NLTag

A tag indicating that the token is an idiom.

static let otherWord: NLTag

A tag indicating that the token is a word other than a kind described by other lexical classes (noun, verb, adjective, adverb, pronoun, determiner, particle, preposition, number, conjunction, interjection, classifier, and idiom).

static let sentenceTerminator: NLTag

A tag indicating that the token is punctuation at the end of a sentence.

