

- Natural Language
- NLTagger
-  NLTagger.Options 

Structure

# NLTagger.Options

Constants for linguistic tagger enumeration specifying which tokens to omit and whether to join names.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
struct Options
```

## Topics

### Constants

static var omitWords: NLTagger.Options

Omit tokens of type word (items considered to be words).

static var omitPunctuation: NLTagger.Options

Omit tokens of type punctuation (all punctuation).

static var omitWhitespace: NLTagger.Options

Omit tokens of type whitespace (whitespace of all sorts).

static var omitOther: NLTagger.Options

Omit tokens of type other (non-linguistic items, such as symbols).

static var joinNames: NLTagger.Options

Typically, multiple-word names will be returned as multiple tokens, following the standard tokenization practice of the tagger.

static var joinContractions: NLTagger.Options

Contractions will be returned as one token.

### Initializers

init(rawValue: UInt)

Creates the option with a raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Enumerating linguistic tags

func enumerateTags(in: Range&lt;String.Index>, unit: NLTokenUnit, scheme: NLTagScheme, options: NLTagger.Options, using: (NLTag?, Range&lt;String.Index>) -> Bool)

Enumerates a block over the tagger’s string, given a range, token unit, and tag scheme.

struct NLTag

A token type, lexical class, name, lemma, language, or script returned by a linguistic tagger for natural language text.

