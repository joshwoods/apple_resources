

- Natural Language
- NLTagScheme
-  tokenType 

Type Property

# tokenType

A scheme that classifies tokens according to their broad type: word, punctuation, or whitespace.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
static let tokenType: NLTagScheme
```

## Discussion

For possible values, see Token types in NLTag.

To classify tokens by a more specific type, for example, distinguishing words between nouns and verbs, use the lexicalClass scheme.

## See Also

### Schemes

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

static let sentimentScore: NLTagScheme

A scheme that scores text as positive, negative, or neutral based on its sentiment polarity.

