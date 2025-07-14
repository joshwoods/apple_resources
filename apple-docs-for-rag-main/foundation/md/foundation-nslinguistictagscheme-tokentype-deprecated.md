

- Foundation
- NSLinguisticTagScheme
-  tokenType Deprecated

Type Property

# tokenType

Classifies tokens according to their broad type: word, punctuation, or whitespace.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
static let tokenType: NSLinguisticTagScheme
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Mentioned in 

Tokenizing Natural Language Text

## Discussion

For possible values, see Token Types.

To classify tokens by a more specific type, for example, distinguishing words between nouns and verbs, use the lexicalClass scheme.

## See Also

### Schemes

static let lexicalClass: NSLinguisticTagScheme

Classifies tokens according to class: part of speech, type of punctuation, or whitespace.

Deprecated

static let nameType: NSLinguisticTagScheme

Classifies tokens according to whether they are part of a named entity.

Deprecated

static let nameTypeOrLexicalClass: NSLinguisticTagScheme

Classifies tokens corresponding to names according to nameType, and classifies all other tokens according to lexicalClass.

Deprecated

static let lemma: NSLinguisticTagScheme

Supplies a stem form of a word token, if known.

Deprecated

static let language: NSLinguisticTagScheme

Supplies the language for a token, if one can be determined.

Deprecated

static let script: NSLinguisticTagScheme

Supplies the script for a token, if one can be determined.

Deprecated

