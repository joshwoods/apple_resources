

- Natural Language
- NLTagScheme
-  sentimentScore 

Type Property

# sentimentScore

A scheme that scores text as positive, negative, or neutral based on its sentiment polarity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let sentimentScore: NLTagScheme
```

## Discussion

The range of a sentiment score is `[-1.0, 1.0]`. A score of `1.0` is the most positive, a score of `-1.0` is the most negative, and a score of `0.0` is neutral.

```
let text = "It's pretty good."

let tagger = NLTagger(tagSchemes: [.tokenType, .sentimentScore])
tagger.string = text

tagger.enumerateTags(in: text.startIndex..

## See Also

### Schemes

static let tokenType: NLTagScheme

A scheme that classifies tokens according to their broad type: word, punctuation, or whitespace.

static let lexicalClass: NLTagScheme

A scheme that classifies tokens according to class: part of speech, type of punctuation, or whitespace.

static let nameType: NLTagScheme

A scheme that classifies tokens according to whether they are part of a named entity.

static let nameTypeOrLexicalClass: NLTagScheme

A scheme that classifies tokens corresponding to names according to nameType, and classifies all other tokens according to lexicalClass.

static let lemma: NLTagScheme

A scheme that supplies a stem form of a word token, if known.

static let language: NLTagScheme

A scheme that supplies the language for a token, if it can determine one.

static let script: NLTagScheme

A scheme that supplies the script for a token, if it can determine one.

