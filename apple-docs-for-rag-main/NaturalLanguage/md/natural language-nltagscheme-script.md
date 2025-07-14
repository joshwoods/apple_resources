

- Natural Language
- NLTagScheme
-  script 

Type Property

# script

A scheme that supplies the script for a token, if it can determine one.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
static let script: NLTagScheme
```

## Discussion

Each value for this tag scheme is an ISO 15924 script identifier. For example, the identifier for Latin script is “Latn” and the identifier for Simplified Chinese script is “Hans”. The identifier “Zyyy” is used if a specific script cannot be determined.

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

static let sentimentScore: NLTagScheme

A scheme that scores text as positive, negative, or neutral based on its sentiment polarity.

