

- Foundation
- NSLinguisticTagger
-  NSLinguisticTagger.Options 

Structure

# NSLinguisticTagger.Options

Constants for linguistic tagger enumeration specifying which tokens to omit and whether to join names.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Options
```

## Topics

### Constants

static var omitWords: NSLinguisticTagger.Options

Omit tokens of type word (items considered to be words).

static var omitPunctuation: NSLinguisticTagger.Options

Omit tokens of type punctuation (all punctuation).

static var omitWhitespace: NSLinguisticTagger.Options

Omit tokens of type whitespace (whitespace of all sorts).

static var omitOther: NSLinguisticTagger.Options

Omit tokens of type other (non-linguistic items, such as symbols).

static var joinNames: NSLinguisticTagger.Options

Typically, multiple-word names will be returned as multiple tokens, following the standard tokenization practice of the tagger. If this option is set, then multiple-word names will be joined together and returned as a single token.

static var omitWords: NSLinguisticTagger.Options

Omit tokens of type word (items considered to be words).

static var omitPunctuation: NSLinguisticTagger.Options

Omit tokens of type punctuation (all punctuation).

static var omitWhitespace: NSLinguisticTagger.Options

Omit tokens of type whitespace (whitespace of all sorts).

static var omitOther: NSLinguisticTagger.Options

Omit tokens of type other (non-linguistic items, such as symbols).

static var joinNames: NSLinguisticTagger.Options

Typically, multiple-word names will be returned as multiple tokens, following the standard tokenization practice of the tagger. If this option is set, then multiple-word names will be joined together and returned as a single token.

### Initializers

init(rawValue: UInt)

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

### Enumerating Linguistic Tags

Identifying Parts of Speech

Classify nouns, verbs, adjectives, and other parts of speech in a string.

Identifying People, Places, and Organizations

Use a linguistic tagger to perform named entity recognition on a string.

func enumerateTags(in: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, using: (NSLinguisticTag?, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates over a given range of the string for a particular unit and calls the specified block for each tag.

Deprecated

func enumerateTags(in: NSRange, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, using: (NSLinguisticTag?, NSRange, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates over a given range of the string and calls the specified block for each tag.

Deprecated

class func enumerateTags(for: String, range: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, orthography: NSOrthography?, using: (NSLinguisticTag?, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates over a given string and calls the specified block for each tag.

Deprecated

