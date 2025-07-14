

- Foundation
- NSLinguisticTagger
- NSLinguisticTagger.Options
-  omitWhitespace 

Type Property

# omitWhitespace

Omit tokens of type whitespace (whitespace of all sorts).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var omitWhitespace: NSLinguisticTagger.Options { get }
```

## See Also

### Constants

static var omitWords: NSLinguisticTagger.Options

Omit tokens of type word (items considered to be words).

static var omitPunctuation: NSLinguisticTagger.Options

Omit tokens of type punctuation (all punctuation).

static var omitOther: NSLinguisticTagger.Options

Omit tokens of type other (non-linguistic items, such as symbols).

static var joinNames: NSLinguisticTagger.Options

Typically, multiple-word names will be returned as multiple tokens, following the standard tokenization practice of the tagger. If this option is set, then multiple-word names will be joined together and returned as a single token.

static var omitWords: NSLinguisticTagger.Options

Omit tokens of type word (items considered to be words).

static var omitPunctuation: NSLinguisticTagger.Options

Omit tokens of type punctuation (all punctuation).

static var omitOther: NSLinguisticTagger.Options

Omit tokens of type other (non-linguistic items, such as symbols).

static var joinNames: NSLinguisticTagger.Options

Typically, multiple-word names will be returned as multiple tokens, following the standard tokenization practice of the tagger. If this option is set, then multiple-word names will be joined together and returned as a single token.

