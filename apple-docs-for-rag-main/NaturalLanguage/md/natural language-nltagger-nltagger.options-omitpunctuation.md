

- Natural Language
- NLTagger
- NLTagger.Options
-  omitPunctuation 

Type Property

# omitPunctuation

Omit tokens of type punctuation (all punctuation).

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
static var omitPunctuation: NLTagger.Options { get }
```

## See Also

### Constants

static var omitWords: NLTagger.Options

Omit tokens of type word (items considered to be words).

static var omitWhitespace: NLTagger.Options

Omit tokens of type whitespace (whitespace of all sorts).

static var omitOther: NLTagger.Options

Omit tokens of type other (non-linguistic items, such as symbols).

static var joinNames: NLTagger.Options

Typically, multiple-word names will be returned as multiple tokens, following the standard tokenization practice of the tagger.

static var joinContractions: NLTagger.Options

Contractions will be returned as one token.

