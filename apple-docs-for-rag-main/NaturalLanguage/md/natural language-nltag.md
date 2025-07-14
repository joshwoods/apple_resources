

- Natural Language
-  NLTag 

Structure

# NLTag

A token type, lexical class, name, lemma, language, or script returned by a linguistic tagger for natural language text.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
struct NLTag
```

## Overview

When you create a linguistic tagger, you specify one or more NLTagScheme constants that correspond to the kind of information you want to know about a selection of natural language text. When working with linguistic tags using the methods described in Getting linguistic tags and Enumerating linguistic tags in NLTagger, the returned value depends on the specified scheme. The NLTag type represents the constant values that can be returned for certain NLTagScheme values.

## Topics

### Token types

Constants representing the token type of a tag with the tokenType scheme.

static let word: NLTag

A tag indicating that the token is a word.

static let punctuation: NLTag

A tag indicating that the token is punctuation.

static let whitespace: NLTag

A tag indicating that the token is white space of any sort.

static let other: NLTag

A tag indicating that the token is a non-linguistic item, such as a symbol.

### Lexical classes

Constants specifying the lexical class of a tag with the lexicalClass or nameTypeOrLexicalClass scheme.

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

static let openQuote: NLTag

A tag indicating that the token is an open quote.

static let closeQuote: NLTag

A tag indicating that the token is a close quote.

static let openParenthesis: NLTag

A tag indicating that the token is an open parenthesis.

static let closeParenthesis: NLTag

A tag indicating that the token is a close parenthesis.

static let wordJoiner: NLTag

A tag indicating that the token is a word joiner, signifying that two tokens on each side should not be broken up.

static let dash: NLTag

A tag indicating that the token is a dash.

static let otherPunctuation: NLTag

A tag indicating that the token is punctuation other than a kind described by other lexical classes (sentence terminator, open or close quote, open or close parenthesis, word joiner, and dash).

static let paragraphBreak: NLTag

A tag indicating that the token is a paragraph break.

static let otherWhitespace: NLTag

A tag indicating that the token is whitespace other than a kind described by other lexical classes (paragraph break).

### Name types

Constants specifying the name type of a tag with the nameType or nameTypeOrLexicalClass scheme.

static let personalName: NLTag

A tag indicating that the token is a personal name.

static let organizationName: NLTag

A tag indicating that the token is an organization name.

static let placeName: NLTag

A tag indicating that the token is a place name.

### Initializers

init(String)

Creates a new tag.

init(rawValue: String)

Creates a new tag from the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerating linguistic tags

func enumerateTags(in: Range&lt;String.Index>, unit: NLTokenUnit, scheme: NLTagScheme, options: NLTagger.Options, using: (NLTag?, Range&lt;String.Index>) -> Bool)

Enumerates a block over the tagger’s string, given a range, token unit, and tag scheme.

struct Options

Constants for linguistic tagger enumeration specifying which tokens to omit and whether to join names.

