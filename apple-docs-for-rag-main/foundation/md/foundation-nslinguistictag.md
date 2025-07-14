

- Foundation
-  NSLinguisticTag 

Structure

# NSLinguisticTag

A token, lexical class, name, lemma, language, or script returned by a linguistic tagger for natural language text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSLinguisticTag
```

## Overview

When you create a linguistic tagger, you specify one or more NSLinguisticTagScheme constants that correspond to the kind of information you want to know about a selection of natural language text. When working with linguistic tags using the methods described in Getting Linguistic Tags and Enumerating Linguistic Tags, the returned value depends on the specified scheme. The NSLinguisticTag type represents the constant values that can be returned for certain NSLinguisticTagScheme values.

## Topics

### Token Types

Constants representing the token type of a tag with the tokenType scheme. In Objective-C you may use pointer equality to compare the values with tag constants.

static let word: NSLinguisticTag

The token indicates a word.

Deprecated

static let punctuation: NSLinguisticTag

The token indicates punctuation.

Deprecated

static let whitespace: NSLinguisticTag

The token indicates white space of any sort.

Deprecated

static let other: NSLinguisticTag

The token indicates a non-linguistic item, such as a symbol.

Deprecated

### Lexical Classes

Constants specifying the lexical class of a tag with the lexicalClass or nameTypeOrLexicalClass scheme. In Objective-C you may use pointer equality to compare the values with tag constants.

static let noun: NSLinguisticTag

The token is a noun.

Deprecated

static let verb: NSLinguisticTag

This token is a verb.

Deprecated

static let adjective: NSLinguisticTag

This token is an adjective

Deprecated

static let adverb: NSLinguisticTag

This token is an adverb.

Deprecated

static let pronoun: NSLinguisticTag

This token is a pronoun.

Deprecated

static let determiner: NSLinguisticTag

This token is a determiner.

Deprecated

static let particle: NSLinguisticTag

This token is a particle.

Deprecated

static let preposition: NSLinguisticTag

This token is a preposition.

Deprecated

static let number: NSLinguisticTag

This token is a number.

Deprecated

static let conjunction: NSLinguisticTag

This token is a conjunction.

Deprecated

static let interjection: NSLinguisticTag

This token is an interjection.

Deprecated

static let classifier: NSLinguisticTag

This token is a classifier.

Deprecated

static let idiom: NSLinguisticTag

This token is an idiom.

Deprecated

static let otherWord: NSLinguisticTag

This token is a word other than a kind described by other lexical classes (noun, verb, adjective, adverb, pronoun, determiner, particle, preposition, number, conjunction, interjection, classifier, and idiom).

Deprecated

static let sentenceTerminator: NSLinguisticTag

This token is a sentence terminator.

Deprecated

static let openQuote: NSLinguisticTag

This token is an open quote.

Deprecated

static let closeQuote: NSLinguisticTag

This token is a close quote.

Deprecated

static let openParenthesis: NSLinguisticTag

This token is an open parenthesis.

Deprecated

static let closeParenthesis: NSLinguisticTag

This token is a close parenthesis.

Deprecated

static let wordJoiner: NSLinguisticTag

This token is a word joiner.

Deprecated

static let dash: NSLinguisticTag

This token is a dash.

Deprecated

static let otherPunctuation: NSLinguisticTag

This token is punctuation other than a kind described by other lexical classes (sentence terminator, open or close quote, open or close parenthesis, word joiner, and dash).

Deprecated

static let paragraphBreak: NSLinguisticTag

This token is a paragraph break.

Deprecated

static let otherWhitespace: NSLinguisticTag

This token is whitespace other than a kind described by other lexical classes (paragraph break).

Deprecated

### Name Types

Constants specifying the name type of a tag with the nameType or nameTypeOrLexicalClass scheme. In Objective-C you may use pointer equality to compare the values with tag constants.

static let personalName: NSLinguisticTag

This token is a personal name.

Deprecated

static let organizationName: NSLinguisticTag

This token is an organization name.

Deprecated

static let placeName: NSLinguisticTag

This token is a place name.

Deprecated

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting Types

struct NSLinguisticTagScheme

Constants for the tag schemes specified when initializing a linguistic tagger.

enum NSLinguisticTaggerUnit

Constants representing linguistic units.

